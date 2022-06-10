---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Simple substitution cipher
1. กำหนดคีย์ เช่นคำว่า *ZEBRAS* จากนั้นนำคีย์ไปใส่เเทนที่ในตัวอักษรภาษาอังกฤษ โดยใส่คีย์ไว้ที่หน้าสุดของตัวอักษรทั้งหมด เมื่อใส่คีย์ลงไปแทนที่เเล้วตัวอักษรเดิมจะถูกนำออกไป ดังตัวอย่างรูปที่ 1
 ![[Simple substitution cipher.png]]
2. กำหนดข้อความที่ต้องการเข้ารหัส เช่น *FLEE AT ONCE. WE ARE DISCOVERED!* 
3. นำเอาตัวอักษรที่เข้ารหัสเเล้วจากตัวอย่างรูปที่ 1 มาเเทนที่ข้อความ ดังรูปที่ 2
![[Simple substitution cipher-2.png|500]]
4. สามารถเข้ารหัสได้ ดังรูปที่ 2 ซึ่งเราจะไม่เขียนตัวอักษรแล้วเว้นตามข้อความปกติแต่สามารถเขียนรหัสเรียงติดกันทั้งหมดหรือเขียนเป็นกลุ่มละ 5 ตัวอักษร (*SIAAZ QLKBA VAZOA RFPBL UAOAR*) ได้
---
## See also
- [[Simple substitution cipher]]
- [[ขั้นตอนการถอดรหัสแบบ Simple substitution cipher]]
## References
- [Wikipedia,"Simple substitution cipher,"2022.](https://en.wikipedia.org/wiki/Substitution_cipher#Simple_substitution)
