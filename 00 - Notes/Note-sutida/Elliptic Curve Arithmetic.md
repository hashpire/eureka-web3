---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC Cryptographic Primitives & Math]]
tags:: #lang/th #type/concept

# Elliptic Curve Arithmetic
การออกแบบที่มี Concept คือการนำจุดที่อยู่บน กราฟเส้นโค้งมาบวกกัน แบ่งเป็น
- *Point Addition*  คือ การนำจุด 2 จุดที่อยู่บนกราฟเส้นโค้งมาบวกกัน ดังรูปที่ 1 เมื่อเรามีจุด P และจุด Q เป็นจุด 2 จุดอยู่บนกราฟเส้นโค้ง ให้เราออกแบบ Concept  ของการบวกจุด 2 จุด โดย ทำการลากเส้นตัดผ่านจุด P และ Q จะได้จุด -(P+Q) จากนั้นทำการลากเส้นตัดผ่านจุด -(P+Q) อีกครั้งจะได้จุด P+Q
![[Elliptic Curve Arithmetic-1.png|300]]
- *Point Scalar Multiplication* คือ การนำจุดไปบวกกันหลายๆ ครั้ง  ดังรูปที่ 2 เมื่อเรามีจุด P หากเราต้องการจุด 2P  ให้เราออกแบบ Concept  ของการบวกจุด โดยให้ลากเส้นตัดผ่านจุด -[2]P แล้วลากเส้นตัดผ่านจุด -[2]P อีกครั้ง เราก็จะได้จุด 2P ออกมา
   จาก $$ kP=P+P+P+....+P $$ 
   ![[Elliptic Curve Arithmetic-2.png|300]]
---
## See also
## References