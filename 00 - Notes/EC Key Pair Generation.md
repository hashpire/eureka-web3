---
version: "0.0.0"
published: true
---
uplinks:: [[EC Key Pair]]
tags:: #lang/en 
# EC Key Pair Generation
Let $G$ be the base point of an elliptic curve $E$ and $n$ be the order of $G$

1. Randomly generate $d \in [1, n-1]$
2. Compute $P = d \cdot G$
3. Key Pair = $(PublicKey, Private Key) = (P, d)$
## References

## See Also
- [[RSA Key Pair Generation]]