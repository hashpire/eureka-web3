---
version: "0.0.0"
published: true
---
uplinks::[Digital Signature](./Digital%20Signature.md)
tags:: #lang/en #type/term 
# Digital Signature Scheme

A digital signature scheme typically consists of three algorithms:
- A key generation algorithm that selects a private key uniformly at random from a set of possible private keys. The algorithm outputs the private key and a corresponding public key.
- A signing algorithm that, given a message and a private key, produces a signature.
- A signature verifying algorithm that, given the message, public key and signature, either accepts or rejects the message's claim to authenticity.

## Common Schemes
- RSA
- DSA
- ECDSA
- EdDSA
- Schnorr
-[BLS Signatures](./BLS%20Signatures.md)
- ElGamal signature scheme

## See Also
1.[Signature Aggregation](./Signature%20Aggregation.md)

## References
1. https://en.wikipedia.org/wiki/Digital_signature