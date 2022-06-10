---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Homophonic substitution cipher
1. กำหนดคีย์ที่จะใช้ในการเข้ารหัสเป็นได้ทั้งตัวอักษรและตัวเลข ตัวอย่างเช่น *CRYTOGRAM56789*
2. นำคีย์ที่กำหนดไปใส่แทนที่ตัวอักษรภาษาอังกฤษและตัวเลข 1-9 โดยใส่คีย์ไว้ที่หน้าสุดของตัวอักษรทั้งหมด เมื่อใส่คีย์ลงไปแทนที่เเล้วตัวอักษรเดิมจะถูกนำออกไป ดังตัวอย่างรูปที่ 1 
![[Homophonic substitution cipher -1.png]]
จากตารางในรูปที่ 1 จะเห็นว่าเราจะให้ ตัวอักษรอย่าง A, E, I, O, U มีจำนวนตัวอักษรแทนที่เยอะกว่าตัวอักษรตัวอื่น เนื่องจากเป็นตัวสระในภาษาอังกฤษที่การใช้งานบ่อย 
3. กำหนดข้อความที่ต้องการเข้ารหัส ดังรูปที่ 2 แล้วแทนที่โดยใช้ Cipher Text  Alphabet จากตารางในรูปที่ 1
![[Homophonic substitution cipher-2.png|500]]
4. จะเข้ารหัสได้เป็น *HRAFA FCFTY E2H7V FF1GZ*  ซึ่งโดยปกติเราจะไม่เขียนตัวอักษรแล้วเว้นตามข้อความปกติ แต่สามารถเขียนรหัสเรียงติดกันทั้งหมดหรือเขียนเป็นกลุ่มละ 5 ตัวอักษรได้ 
---
## See also
- [[Homophonic substitution cipher]]
- [[ขั้นตอนการถอดรหัสแบบ  Homophonic substitution cipher]]
## References
- [Wikipedia,"Homophonic Substitution,"2022.](https://en.wikipedia.org/wiki/Substitution_cipher#Homophonic_substitution)
- ["The Homophonic Substitution Cipher"](https://www.simonsingh.net/The_Black_Chamber/homophonic_cipher.html)