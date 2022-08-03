---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Rail fence cipher
1. กำหนดข้อความที่ต้องการเข้ารหัส เช่น *WE ARE DISCOVERED FLEE AT ONCE*
2. กำหนดคีย์ ในที่นี้ คือการกำหนด จำนวนแถว เช่น ในตัวอย่างรูปที่ 1 เป็นแบบ 3  แถว และคำนวณคอลัมน์จาก จำนวนของตัวอักษรในข้อความธรรมดาที่ต้องการเข้ารหัส
3. นำข้อความที่กำหนดไปใส่ลงในตาราง ตามแนวทแยงเริ่มจากด้านซ้ายบนลงล่าง และล่างขึ้นบนจนครบ ดังรูปที่ 1
![[Rail fence cipher.png|500]]
3. นำตัวอักษรมาเรียงต่อกัน โดยเรียงจากซ้ายไปขวาตามเเต่ละแถว(ราง) จาก*WE ARE DISCOVERED FLEE AT ONCE*  จะเข้ารหัสได้เป็น *WECRL TEERD SOEEF EAOCA IVDEN*
4. ในการเข้ารหัสลับ เราสามารถเขียนรหัสเรียงติดกัน โดยไม่ต้องเว้นช่องว่างได้ แต่เพื่อให้ง่ายต่อการจำและการเขียน ส่วนใหญ่ จึงเขียนเป็นกลุ่มตัวอักษร กลุ่มล่ะ 5 ตัว จำนวนกลุ่มขึ้นอยู่กับจำนวนของตัวอักษรทั้งหมด

---
## See also
- [[Rail fence cipher]]
- [[ขั้นตอนการถอดรหัสแบบ Rail fence cipher]]
## References
- [Wikipedia,"Rail Fence cipher,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Rail_Fence_cipher)


