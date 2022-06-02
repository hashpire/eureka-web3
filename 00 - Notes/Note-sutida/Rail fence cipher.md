---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/term 

# Rail fence cipher
- *Rail fence cipher* คือ การเข้ารหัสลับโดยการนำข้อความต้นฉบับไปเขียนลงในตารางตามเเนวทเเยงต่อเนื่องกันบนลงล่างเเละล่างขึ้นบน ซึ่งมีรูปแบบเปรียบเสมือนเป็นรั้วและรางที่เชื่อมต่อกัน ดังรูปที่ 1 
![[Rail fence cipher.png]]
- เมื่อเข้ารหัสแล้วจะได้เป็นกลุ่มคำ 5 กลุ่ม กลุ่มล่ะ 5 ตัวอักษรเพื่อให้ง่ายต่อการจำและการเขียน การเว้นช่องของข้อความเเต่ละกลุ่มคำจะไม่เกี่ยวข้องกับช่องว่างของข้อความในต้นฉบับ
- ตัวอย่างจากรูปที่ 1 จะเป็นแบบ 3 ราง(แถว) และข้อความคือ *WE ARE DISCOVERED FLEE AT ONCE* 
  นำมาเรียงต่อกันโดยเรียงจากซ้ายไปขวาตามเเต่ละแถว(ราง) จาก*WE ARE DISCOVERED FLEE AT ONCE*  จะเข้ารหัสได้เป็น *WECRL TEERD SOEEF EAOCA IVDEN*

---
## See also

## References
- [Wikipedia,"Rail Fence cipher,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Rail_Fence_cipher)












**นำมาเรียงต่อกันโดยเรียงจากซ้ายไปขวาตามเเต่ละบรรทัด(ราง) จาก*WE ARE DISCOVERED FLEE AT ONCE*

จะเข้ารหัสได้เป็น *WECRL TEERD SOEEF EAOCA IVDEN *