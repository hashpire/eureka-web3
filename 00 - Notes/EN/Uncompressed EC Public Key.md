---
version: "0.0.0"
published: true
---
uplinks::[EC Key Pair](./EC Key Pair.md)
tags:: #lang/en 
# Uncompressed EC Public Key
- An uncompressed EC public key is 65 bytes, consisting of a constant prefix $\text{0x04}$, followed by the $x$ coordinate (32-byte integer) and the $y$ coordinate (32-byte integer) of the public key (EC Point).

## References

## See Also
1.[Compressed EC Public Key](./Compressed EC Public Key.md)
