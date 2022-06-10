---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัสแบบ Rail fence cipher
1. เราจะต้องทราบ รหัสลับและคีย์ที่ใช้ในการเข้ารหัส 
2. ทำการสร้างตารางขึ้นมา โดยให้คีย์เป็นตัวกำหนดจำนวนแถว และจำนวนตัวอักษรในรหัสลับเป็นตัวกำหนดจำนวนคอลัมน์  
3. นำตัวอักษรตัวแรกในรหัสลับไปใส่ไว้ในตารางที่มุมบนด้านซ้าย จากนั้นให้ทำการขีดเส้นทแยงเรียงจากบนลงล่าง และล่างขึ้นบนจนครบ ดังรูปที่ 2 
     ![[Rail fence cipher-2.png|500]]
4. นำรหัสลับใส่ลงในตาราง ตามช่องที่ได้ขีดเส้นไว้ ดังรูปที่ 3
![[Rail fence cipher-3.png|500]]
5. ใส่รหัสลงในตารางจนครบ จะได้ดังรูปที่ 4
![[Rail fence cipher-4.png|500]]
6. นำตัวอักษรมาเรียงต่อกัน โดยเรียงตามแนวทแยงบนลงล่าง และล่างขึ้นบนจะได้ ข้อความก่อนเข้ารหัส คือ *WE ARE DISCOVERED FLEE AT ONCE* 
---
## See also
- [[Rail fence cipher]]
- [[ขั้นตอนการเข้ารหัสแบบ Rail fence cipher]]
## References
- [Wikipedia,"Rail Fence cipher,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Rail_Fence_cipher)
