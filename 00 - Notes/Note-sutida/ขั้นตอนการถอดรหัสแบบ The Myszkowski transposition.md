---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัสแบบ The Myszkowski transposition
1. การถอดรหัสเราจะต้องทราบคีย์ในการถอดรหัสเเละรหัสที่ต้องการถอด
2. คำนวณตาราง โดยการเอาจำนวนตัวอักษรในรหัสที่ได้รับหารกับตัวอักษรในคีย์ 
3. สร้างตารางเเล้วนำเอาคีย์ไปใส่ที่หัวตารางโดยเรียงตามลำดับตัวอักษรและใส่รหัสลงในแถวจากบนลงล่าง ตรงส่วนนี้อย่าลืมว่าตอนที่นำรหัสมาใส่ในตาราง คอลัมน์ที่คีย์เหมือนกันจะต้องใส่มันเป็นคู่พร้อมกันเรียงจนครบตาราง ห้ามใส่ที่ละเเถวเด็ดขาด ดังรูปที่ 2
4. จากนั้นสลับตำแหน่งให้ตาราง โดยการเรียงคีย์ให้กลับไปเป็นรูปแบบเดิม ดังรูปที่ 2
![[The Myszkowski transposition-2.png]]
5. จากในรูปที่ 2 จะได้ตารางก่อนในรูปแบบก่อนที่จะทำการเข้ารหัสออกมา และถอดรหัสได้เป็น  *A COLLABORATIVE SPACE FOR PEOPLE TO LEARN WEB THREE*
---
## See also
- [[The Myszkowski transposition]]
- [[ขั้นตอนการเข้ารหัสแบบ The Myszkowski transposition]]
## References
- ["Myszkowski Transposition Cipher"](https://crypto.interactive-maths.com/myszkowski-transposition-cipher.html)
- [Wikipedia,"Myszkowski transposition,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Myszkowski_transposition)
