---
version: "0.0.0"
published: true
---
# EdDSA vs ECDSA vs Schnorr

EdDSA is _not_ ECDSA over a different curve. Rather, it is a type of Schnorr signature. Indeed the name is very confusing, and I'm pretty sure that it was chosen in order to give this impression, since Schnorr is less well known.

[Schnorr](https://en.wikipedia.org/wiki/Schnorr_signature) is essentially a zero-knowledge proof of knowledge of the discrete log of the public key, obtained via the Fiat-Shamir paradigm applied to the classic Schnorr Sigma protocol.

ECDSA is a completely different signature scheme, which was designed specifically to bypass Schnorr's patent (at least, this is the understanding in the field).

If it's faster to compute ECDSA over Curve25519 and you specifically want ECDSA, then why not? However, Schnorr is better theoretically and it's faster. So, if you don't need legacy ECDSA, I don't see why you would want to do th


---

Ed25519 is a specific instance of the [EdDSA family of signature schemes](https://en.wikipedia.org/wiki/EdDSA "Wikipedia: EdDSA.  Retrieved 2018-04-15."). Ed25519 is specified in [RFC 8032](https://www.rfc-editor.org/rfc/rfc8032 "S. Josefsson and I. Liusvaara, ‘Edwards-Curve Digital Signature Algorithm (EdDSA)’, IETF RFC 8032, January 2017.") and widely used. The only other instance of EdDSA that anyone cares about is Ed448, which is slower, not widely used, and also specified in RFC 8032. _Keys_ and _signatures_ in one instance of EdDSA are not meaningful in another instance of EdDSA: Ed25519 and Ed448 are different signature schemes.

The [ECDSA family of signature schemes](https://en.wikipedia.org/wiki/ECDSA "Wikipedia: ECDSA.  Retrieved 2018-04-15.") is not related to EdDSA, except in that the mathematics behind it [also involves elliptic curves](https://blog.cr.yp.to/20140323-ecdsa.html "Daniel J. Bernstein, ‘How to design an elliptic-curve signature system’, blog.cr.yp.to, 2014-03-23."). Any particular instance of ECDSA, such as ECDSA over the curve secp256k1 with SHA-256 (as Bitcoin uses), is incompatible with any other instance of it, such as ECDSA over the curve nistp521 with SHA-512.

On a practical level, what a _user_ might need to know is that Ed25519 keys are not compatible in any meaningful sense with keys in any instance of ECDSA. So, _e.g._, in the ssh protocol, an `ssh-ed25519` key is not compatible with an `ecdsa-sha2-nistp521` key, which is why they are marked with different types. Similarly, an `ssh-ed448` key, for Ed448, is incompatible, which is why it is also marked with a different type.

On a technical level, what a _protocol designer_ should know is that the ECDSA family of signature schemes is an archaic slow design that encourages security-destroying implementation errors, while the EdDSA family of signature schemes is a modern design that avoids those errors.

---

The main reason is historical (and a bit sad).

==ECDSA can be seen as a repurposed authentication mechanism. The private key owner wants to prove knowledge of the private key 𝑥x that matches a given public key 𝑄=𝑥𝐺Q=xG, but without revealing that private key. Thus, this is organized as a three-step protocol:==

1.  The prover makes a _commitment_ on a newly generated random value 𝑘k; the commitment is the point 𝑘𝐺kG (value 𝑟r is basically the X coordinate of that point).
2.  The verifier issues a challenge (let's call it 𝑒e).
3.  The prover responds to the challenge with a value 𝑠s, which is such that the verifier can check that the prover knew a value derived from 𝑘k and 𝑥x, but without actually revealing 𝑥x.

This authentication scheme is then turned into a signature scheme by making the signer play the protocol against himself: the challenge is computed deterministically from the commitment, making the physical presence of the verifier unnecessary. The signer can play the protocol by himself, and the transcript of the protocol (the pair (𝑟,𝑠)(r,s)) can be verified non-interactively afterwards.

Now, in the 1980s, there was a nice protocol fitting that mechanism, known as [Schnorr signatures](https://en.wikipedia.org/wiki/Schnorr_signature). In a Schnorr signature, the challenge 𝑒e is computed as a hash value over the signed message and the commitment, and the response is computed as 𝑠=𝑘−𝑥𝑒s=k−xe (some variants make it 𝑠=𝑘+𝑥𝑒s=k+xe). However, Schnorr had filed a patent on that algorithm. When the US federal government looked for an algorithm to standardize for all US federal organizations, they wanted to avoid patents as much as possible (otherwise, they would have used RSA, which was also patented). Thus, they looked for a more-or-less Schnorr-like protocol that would be nonetheless different enough so as not to infringe on the patent. They thus lifted the [ElGamal signature scheme](https://en.wikipedia.org/wiki/ElGamal_signature_scheme), which was not patented (at that time! Certicom filed patents afterwards, for ElGamal adapted to elliptic curves). It was ElGamal that introduced the modular inversion of 𝑘k, which is cumbersome to implement. The result of the adaptation of ElGamal into a US standard was called DSA. ECDSA was later defined as DSA applied on elliptic curves.

==Thus, you can say that the specific formula of DSA and ECDSA, with the 𝑘−1, was chosen for patent avoidance reasons, not for any cryptographic advantage.== Indeed, that formula sucks: it makes implementation more complicated, it prevents some security proofs, and it makes the signatures somewhat malleable (if (𝑟,𝑠)(r,s) is a valid ECDSA signature, then (𝑟,−𝑠)(r,−s) is also a valid ECDSA signature on the same message with the same key), a property which has induced some occasional trouble (namely, transaction replay attacks in Bitcoin).



## References
1. https://bitcoincore.org/en/2017/03/23/schnorr-signature-aggregation/
2. https://wiki.polkadot.network/docs/learn-cryptography
3. https://en.wikipedia.org/wiki/Curve25519
4. https://medium.com/asecuritysite-when-bob-met-alice/whats-the-difference-between-ecdsa-and-eddsa-e3a16ee0c966
5. https://crypto.stackexchange.com/questions/86467/how-is-eddsa-different-from-ecdsa-with-a-custom-curve
6. https://crypto.stackexchange.com/questions/58380/ecdsa-eddsa-and-ed25519-relationship-compatibility?rq=1
7. https://crypto.stackexchange.com/questions/64826/why-ecdsa-has-its-form/64852#64852
8. https://www.youtube.com/watch?v=S77ES52AGVg
## See Also
