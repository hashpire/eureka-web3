---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Route cipher
1. กำหนดข้อความที่ต้องการจะเข้ารหัส เช่น *WE ARE DISCOVERED FLEE AT ONCE*
2. ออกแบบตารางที่เหมาะสมกับข้อความที่กำหนดไว้ สามารถคำนวณจากจำนวนตัวอักษรในข้อความได้ เช่น ข้อความมี 27 ตัวอักษร เป็น 27/3 จะได้ตารางเป็น 9 คอลัมน์ 3 แถว (เเต่หากข้อความไม่สามารถคำนวณได้ลงตัวตารางที่ว่างสามารถใส่ค่า null ลงไปได้) 
3. นำข้อความมาเขียนลงในตาราง โดยเขียนเรียงจากซ้ายไปขวาจนครบ
4. กำหนดรูปแบบทิศทางการเข้ารหัส เช่น อ่านจากมุมบนขวามือ ทิศทางตามเข็มนาฬิกา วนเข้าด้านใน  ดังตัวอย่าง รูปที่ 1
![[Route cipher-1.png|400]]
5. นำข้อความที่ได้จากรูปแบบการเข้ารหัส ออกมาเขียนเป็นรหัสลับ ซึ่งเราสามารถเขียนรหัสเรียงติดกันทั้งหมดหรือเขียนเป็นกลุ่มละ 5 ตัวอักษรก็ได้ จะได้เป็น  **EJXCT EDECD ADAEW RIORF EONAL EVSEE**
---
## See also
- [[Route cipher]]
- [[ขั้นตอนการถอดรหัสเเบบ Route cipher ]]
## References
- [Wikipedia,"Route cipher,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Route_cipher)
- ["Route Cipher"](https://crypto.interactive-maths.com/route-cipher.html)
