---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัส Columnar transposition
1. เราจะต้องทราบคีย์ที่จะใช้ในการถอดรหัส 
2. คำนวณตาราง โดยเอาจำนวนตัวอักษรในรหัสหารด้วยจำตัวอักษรในคีย์
3. นำคีย์ที่ได้ไปเขียนลงในคอลัมน์หัวตารางตามลำดับตัวอักษร จากนั้นเขียนรหัสลงในเเถวใต้คีย์เรียงจากบนลงล่างจนครบ ดังรูปที่ 2
4. สลับคีย์ให้อยู่ในรูปแบบเดิม ดังรูปที่ 2
![[Columnar Transposition-2.png]]
5. อ่านข้อความในเเถวเรียงจากซ้ายไปขวา จะได้เป็นข้อความก่อนที่จะเข้ารหัส เป็น *THE  CENTRAL INTELLIGENCE AGENCY*

---
## See also
- [[Columnar transposition]]
- [[ขั้นตอนการเข้ารหัสแบบ Columnar transposition]]
## References
- [Wikipedia,"Columnar transposition,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Columnar_transposition)
- [Chris Christensen,"Columnar transposition,"2015.](https://www.nku.edu/~christensen/1402%20Columnar%20transposition.pdf)
- ["Columnar Transposition Cipher,"2019.](https://www.geeksforgeeks.org/columnar-transposition-cipher/)
