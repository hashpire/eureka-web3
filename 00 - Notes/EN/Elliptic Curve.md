---
version: "0.0.0"
published: true
---
uplinks::[Algebra](./Algebra.md)[[Geometry]]
tags:: #lang/en #type/term #note/tidy 
# Elliptic Curve
- An elliptic curve $E$ is a plane algebraic curve defined as the set of points to the Weierstrass equation  $y^2 = x^3 + ax + b$ and an extra[Point at Infinity (EC)|point at infinity](./Point at Infinity (EC)|point at infinity.md)$O$ , where the constants $a$ and $b$ must satisfy $4a^3 + 27b^2 \neq 0$
	- The equation was named after the mathematician Karl Weierstrass,  who studied elliptic curves extensively during the 19th century

> There are other representations of elliptic curves, but technically an elliptic curve is the set points satisfying an equation in two variables with degree two in one of the variables and three in the other. — Cloudflare

## Properties
-  Non-singular
	- no cusps or self-intersections
- Horizontal symmetric. 
	- Any point on the curve can be reflected over the x axis and remain the same curve. 
- Any non-vertical line will intersect the curve in at most three places.

## Examples
$E_1 : y^2 = x^3 − x$
$E_2: y^2 = x^3 + \frac{1}{4}x + \frac{5}{4}$

#todo/picture

## See Also
1.[Common Elliptiic Curves in Blockchains](./Common Elliptiic Curves in Blockchains.md)
2.[Elliptic Curve Cryptography](./Elliptic Curve Cryptography.md)
3.[Elliptic Curve Arithmetic](./Elliptic Curve Arithmetic.md)

## References
1.[Peking University Introduction to Information Security Class](./Peking University Introduction to Information Security Class.md)
2. https://crypto.stackexchange.com/questions/26329/what-are-the-differences-between-the-elliptic-curve-equations #todo/read 
3. https://safecurves.cr.yp.to/equation.html #todo/read 
4. https://blog.cloudflare.com/a-relatively-easy-to-understand-primer-on-elliptic-curve-cryptography/