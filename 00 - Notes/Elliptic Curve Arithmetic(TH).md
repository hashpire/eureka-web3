---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC Cryptographic Primitives & Math]]
tags:: #lang/th #type/thing 

# Elliptic Curve Arithmetic
การออกแบบที่มี Concept คือ การนำจุดที่อยู่บน กราฟเส้นโค้ง [[Elliptic Curve (EC)]] มาบวกกัน แบ่งเป็น
- *Point Addition*  คือ การนำจุด 2 จุดที่อยู่บนกราฟเส้นโค้งมาบวกกัน  เมื่อเรามีจุด P และจุด Q เป็นจุด 2 จุดอยู่บนกราฟเส้นโค้ง ให้เราบวกจุด 2 จุด โดย ทำการลากเส้นตัดผ่านจุด P และ Q จะได้จุด -(P+Q) จากนั้นทำการลากเส้นแนวตั้งตัดผ่านจุด -(P+Q) อีกครั้งจะได้จุด P+Q

- *Point Scalar Multiplication* คือ การนำจุดบนกราฟเส้นโค้งไปบวกกันหลายๆ ครั้ง เมื่อเรามีจุด P หากเราต้องการหาจุด 2P  ให้เราลากเส้นตัดผ่านจุด -[2]P แล้วลากเส้นตัดแนวตั้งผ่านจุด -[2]P อีกครั้ง เราก็จะได้จุด 2P ออกมา สมการคือ  $kP=P+P+P+....+P$ 
 
---
## See also
- [[Modular Arithmetic (TH)]]
- [[Elliptic Curve Arithmetic(TH)]]
## References