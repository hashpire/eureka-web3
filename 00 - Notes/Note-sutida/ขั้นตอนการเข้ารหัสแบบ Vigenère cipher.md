---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Vigenère cipher
1. กำหนดข้อความที่ต้องการเข้ารหัส เช่น *ATTACK AT DAWN*
2. กำหนดคีย์ที่ใช้ในการเข้ารหัส เช่น *LEMON*
3. นำคีย์ที่กำหนดมาเขียนให้ความยาวเท่ากับข้อความที่ต้องการเข้ารหัส ดังรูปที่ 2
   ![[Vigenère Cipher-2.png|500]]
5. นำคีย์และข้อความเข้ารหัสที่ตรงกันไปหาจุดตัดบนตารางในรูปที่ 1 โดยการหาจุดตัดของตัวคีย์ (แกนเเนวนอนของตาราง) และข้อความธรรมดา (แกนเเนวตั้งของตาราง)  ให้ครบทุกตัว จะได้รหัสลับออกมา ดังรูปที่ 2
 ![[Vigenère Cipher.png|300]]
---
## See also
- [[Vigenère cipher]]
- [[ขั้นตอนการถอดรหัสแบบ Vigenère cipher]]

## References
- [Wikipedia,"Vigenère cipher,"2022.](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher)
- [Thanin Muangpool,"Chapter7 Cryptography"](http://pws.npru.ac.th/signal/data/files/Chapter7_Cryptography.pdf)

