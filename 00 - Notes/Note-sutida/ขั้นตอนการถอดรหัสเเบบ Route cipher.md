---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัสเเบบ Route cipher
1. การถอดรหัสเราจะต้องทราบขนาดของตาราง และรูปแบบทิศทางการเข้ารหัสที่กำหนด
2. นำรหัสที่ได้มาเขียนลงในตาราง โดยเรียงจากรูปแบบทิศทางการเข้ารหัสนั้น เช่น  อ่านจากมุมบนขวามือ ทิศทางตามเข็มนาฬิกา วนเข้าด้านใน  ดังรูปที่ 2
![[Route cipher-2.png]]
3. เมื่อเขียนรหัสลงในตารางจนครบ เราก็จะสามารถถอดข้อความที่เข้ารหัสไว้ออกมาได้ โดยการเริ่มอ่านจากคอลัมน์ซ้ายมือบนลงล่าง และล่างขึ้นบน ดังในรูปที่ 2 จะได้ข้อความว่า *WE ARE DISCOVERED FLEE AT ONCE* 
4. *ข้อควรระวัง* คือต้องเลือกรูปแบบตาราง และรูปแบบทิศทางการเข้ารหัสให้เหมาะสม เพราะตารางและรูปแบบทิศทางที่ไม่เหมาะกับจำนวนของตัวอักษร อาจจะทำให้จำนวนคีย์ที่ได้รับมากจนเกินไปและยากต่อการส่งต่อข้อมูล

---
## See also
- [[Route cipher]]
- [[ขั้นตอนการเข้ารหัสแบบ Route cipher]]
## References
- [Wikipedia,"Route cipher,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Route_cipher)
- ["Route Cipher"](https://crypto.interactive-maths.com/route-cipher.html)
