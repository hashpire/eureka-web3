---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/term 

# Monoalphabetic substitution cipher
- *Monoalphabetic substitution cipher* หรือ *Monoalphabetic cipher*  คือ การเข้ารหัสเเบบเเทนที่ 1 ต่อ 1 ไม่ใช่การเลื่อนตำแหน่ง เป็นวิธีการที่คิดค้นโดยชาวอาหรับ ในยุคเเรกๆ คือ การเข้ารหัสเเบบ *Atbash* ใช้การเเทนที่ ดังรูปที่ 1 เป็นแบบตายตัว
![[Atbash.png]]
- การถอดรหัส วิธีการเข้ารหัสแบบ Monoalphabetic cipher นั้นสามารถทำได้โดยการวิเคราะห์ความถี่ของตัวอักษร (Frequency Analysis) โดยเริ่มจากการหาตัวอักษรที่ซ้ำ ๆ กัน และพิจารณาตัวอักษร 3 ตัวเเรกของประโยค ซึ่งตัวที่ 2 และ 3 จะเป็นสระ (A, E, I, O, U) เสมอ หรือพิจารณาตัวอักษรที่มีความถี่ปรากฏในคำภาษาอังกฤษบ่อยที่สุด 
- เนื่องจากการเข้ารหัสเเบบ Monoalphabetic cipher นั้นสามารถที่จะถอดรหัสได้ไม่ยาก จากการใช้ Frequency Analysis  จึงมีการพัฒนาการเข้ารหัสเเบบ [[Polyalphabetic substitution cipher]] เพื่อเเก้ปัญหาที่เกิดขึ้นนี้อีกด้วย

---
## See also
## References
- [Thanin Muangpool,"Chapter7 Cryptography,"](http://pws.npru.ac.th/signal/data/files/Chapter7_Cryptography.pdf)
- ["mono-alphabetic-substitution-cipher,"2019.](https://www.101computing.net/mono-alphabetic-substitution-cipher/)
