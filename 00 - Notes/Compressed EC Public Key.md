---
version: "0.0.0"
published: true
---
uplinks::[EC Key Pair](./EC Key Pair.md)
tags:: #lang/en 
# Compressed EC Public Key
- Due to the nature of an[Elliptic Curve](./Elliptic Curve.md) an EC public key, which is an EC point, can be represented with the $x$-coordinate and one extra bit for $y$ or $-y$
- Compresed public keys in[Bitcoin](./Bitcoin.md)are 33 bytes,  consisting of a prefix either $\text{0x02}$ or $\text{0x03}$, followed by a 32-byte $x$-coordinate integer
	- $\text{0x02}$ if $y$ is even
	- $\text{0x03}$ if $y$ is odd

## See Also
1.[Uncompressed EC Public Key](./Uncompressed EC Public Key.md)
