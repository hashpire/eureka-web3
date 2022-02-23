---
version: "0.0.0"
published: true
---
uplinks:: [[Cryptographic Primitives]]
tags:: #lang/en #type/term 
# Cryptographic Hash Function
A [[Hash Function]] that is:
1. Pre-image resistant (One-way property)
	- Given h = H(M), it is computationally infeasible to find M
2. Second pre-image resistant (Weak collision resistant)
	- Given h = H(M), it is computationally infeasible to find M’ that H(M’) = h
3. Collision resistant (Strong collision resistant)
	- It is computationally infeasible to find any M1, M2 that H(M1) = H(M2)


## References
1. [[Peking University Introduction to Information Security Class]]
