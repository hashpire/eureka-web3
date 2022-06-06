---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/concept 

# Vigenère cipher
 *Vigenère cipher* คือ การเข้ารหัสเเบบแทนที่ตัวอักษร ที่ใช้พื้นฐานมาจากการเข้ารหัสเเบบ [[Caesar cipher]] และรูปแบบการเเทนที่ตัวอักษรแบบ[[Polyalphabetic substitution cipher]] โดยการนำคีย์มาเขียนให้ยาวเท่ากับข้อความธรรมดา เขียนซ้ำไปมาจนครบ จากนั้นนำคีย์และตัวข้อความธรรมดาที่เท่ากันไปเข้ารหัสโดยการใช้[ตารางของ Vigenère Cipher ที่เป็นเเบบ 26x26 ตัวอักษร](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher#/media/File:Vigen%C3%A8re_square_shading.svg) การเข้ารหัสจะทำโดยการหาจุดตัดของตัวคีย์ (แกนเเนวนอนของตาราง) และข้อความธรรมดา (แกนเเนวตั้งของตาราง) จะได้ รหัสที่ต้องการออกมา 

---
## See also
## References
- [Wikipedia,"Vigenère cipher,"2022.](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher)
- [Thanin Muangpool,"Chapter7 Cryptography"](http://pws.npru.ac.th/signal/data/files/Chapter7_Cryptography.pdf)
