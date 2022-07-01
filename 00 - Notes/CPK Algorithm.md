---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC Type of HD Wallet]]
tags:: #lang/th #type/thing

# CPK Algorithm

- วิธีการสร้าง Private key 
 $$
\begin{align}
ComposedPrivKey_i &= \sum_{j=1}^{k}a_id_i \pmod{n} \\
\end{align}
$$
   นำ Identier (ค่า id ) ไปเข้า Mapping Function เช่น SHA256 จะได้ Selector Sequence ออกมาเป็นค่า $a_1,a_2,\dots,a_k$ ซึ่งมาจากการนำ 256 Bit ไปแบ่ง โดย 8 ตัวเเรกเป็น $a_1$ , 8 ตัวที่สอง เป็น $a_2$ ไปเรื่อยๆ จนครบ จากนั้นจะมีการนำ Private Sequence $(d_1,d_2,\dots,d_𝑘)$  เข้ามาใช้ โดยนำ Selector Sequence และ Private Sequence ไปเข้าฟังก์ชั่น Modular Multiplication ได้ออกมาเป็น $a_1d_1,a_2d_2,\dots,a_kd_k$ นำค่าที่ได้  ไปเข้าฟังก์ชั่น Modular Sum ได้ $a_1d_1 + a_2d_2+...+a_kd_k (mod n)$ และจะได้เป็น Composed Private key ออกมา
- วิธีการสร้าง Public Key
 $$
\begin{align}
ComposedPubKey_i &= \sum_{j=1}^{k}a_iP_i
\end{align}
$$

  ขั้นตอนคล้ายกับการสร้าง Private key แต่จะแตกต่างกันตรงที่ใช้ Public Sequence $(P_1,P_2,..,P_𝑘)=(d_1𝐺,d_2𝐺,\dots,d_𝑘𝐺)$ แทน Private Sequence และใช้ฟังก์ชั่น Point Scalar  Multiplication แทน Modular Multiplication  ได้เป็น $a_1P_1, a_2P_2,...,a_kP_k$ นำค่าที่ได้  ไปเข้าฟังก์ชั่น Point Sum ได้ $a_1P_1+a_2P_2+...+a_kP_k$ และจะได้เป็น Composed  Public key ออกมา

 ---

## See also
- [[CPK-based Wallets]]
- [[CPK Security]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.