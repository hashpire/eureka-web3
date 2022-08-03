---
version: "0.0.0"
published: true
---
uplinks::[Elliptic Curve](./Elliptic Curve.md)
tags:: #lang/en
# Elliptic Curve Arithmetic

## Point Addition
- A point addition is the operation of adding two elliptic curve points
- there is a natural way to take two points on an elliptic

---
Let 
- $E: Y^2 = X^3 + AX + B$ be an[Elliptic Curve](./Elliptic Curve.md)
- $O$ as[Point at Infinity (EC)|point at infinity](./Point at Infinity (EC)|point at infinity.md)
-  $P_1 = (x_1,y_1)$ and $P_2 = (x_2,y_2)$ be points on $E$

If $P_1 = O$, then $P_1 + P_2 = P_2$ 
If $P_2 = O$, then $P_1 + P_2 = P_1$ 
If $x_1 = x_2$ and $y_1 = -y_2$ , then $P_1 + P_2 = O$
Else, let 

$$
\lambda = 
\begin{cases}
  \frac{y_2 - y_1}{x_2 - x_1}, & \text{if } P_2 \neq P_2, \\
  \frac{3x_1^2 + A}{2y_1}, & \text{if } P_1 = P_2,
\end{cases}

$$
and let 
$$
x_3 = \lambda^2 - x_1 - x_2 \qquad\text{and}\qquad y_3 = \lambda(x_1 - x_3) - y_1
$$
Then $P_1 + P_2 = (x_3,y_3)$

## Point Scalar Multiplication
A point scalar multiplication is the operation of adding a point along an elliptic curve to itself repeatedly.

---
Let $E: Y^2 = X^3 + AX + B$ be an[Elliptic Curve](./Elliptic Curve.md)
Let $P$ be a point on $E$

$$
\begin{gather}
kP = P + P + P +  \dots + P \\
k\text{ times point double/addition}
\end{gather}
$$

---
This is similar to modular exponentiation:
$$
\begin{gather}
g^k \equiv g \cdot g \cdot g \cdots g \pmod{p} \\
k \text{ times modular multiplication}
\end{gather}
$$

## See Also
1.[Modular Arithmetic](./Modular Arithmetic.md)

## References
1.[Peking University Introduction to Information Security Class](./Peking University Introduction to Information Security Class.md)