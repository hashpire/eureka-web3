---
version: "0.0.0"
published: true
---
# Combined Public Key Algorithm
- The combined public key algorithm (CPK) is an identity-based large-scale key management algorithm. 
- It can be used on any system that uses public key cryptography that has a special composite property. 
- Because typical blockchain systems use elliptic curve cryptography, which has this special composite property, the combined public-key algorithm can be applied to blockchain wallets to solve large-scale key management problems.

 ## Algorithm
 Let
 $$
\begin{align}
PrivateSequence &= (d_1,d_2,\dots,d_𝑘) \\
PublicSequence &= (P_1,P_2,..,P_𝑘)=(d_1𝐺,d_2𝐺,\dots,d_𝑘𝐺) \\
T &= Identifier \\
SelectorSequence &= (a_1,a_2,\dots,a_k) = Mapping(T)\\
\end{align}
$$
Then
 $$
\begin{align}
ComposedPrivKey_i &= \sum_{j=1}^{k}a_id_i \pmod{n} \\
ComposedPubKey_i &= \sum_{j=1}^{k}a_iP_i
\end{align}
$$


---
## Flowchart
### Composed Private Key Generation
```mermaid
graph TD;
	sseq[/"Private Sequence<br/>(d1,d2,...,dk)"/]
	id[/Identifier/]-->mfunc[Mapping Function]
	mfunc-->selseq[/"Selector Sequence<br/>(a1,a2,...,ak)"/]
	pmul["Modular Multiplication<br/> (a1d1, a2d2,...,akdk)"]
	psum["Modular Sum<br/> a1d1 + a2d2 + ...+ akdk (mod n)"]
	sseq-->pmul
	selseq-->pmul
	pmul-->psum
	psum-->cpk[/Composed Private Key/]
```
### Composed Public Key Generation

```mermaid
graph TD;
	pseq[/"PubSeq<br/>(P1,P2,...,Pk)"/]
	id[/Identifier/]-->mfunc[Mapping Function]
	mfunc-->selseq[/"Selector Sequence<br/>(a1,a2,...,ak)"/]
	pmul["Point Scalar Multiplication<br/> (a1P1, a2P2,...,akPk)"]
	psum["Point Sum<br/> a1P1 + a2P2 + ...+ akPk"]
	pseq-->pmul
	selseq-->pmul
	pmul-->psum
	psum-->cpk[/Composed Public Key/]
```


## See Also
1.[CPK Blockchain Wallets](./CPK%20Blockchai%20Wallets.md)