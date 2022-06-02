---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Columnar transposition]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัส Columnar transposition
1. การถอดรหัสเราจะต้องทราบคีย์ที่จะใช้ในการถอดรหัส
2. คำนวณตารางโดยเอาจำนวนตัวอักษรในรหัสหารด้วยจำตัวอักษรในคีย์
3. นำคีย์ที่ได้ไปเขียนลงในคอลัมน์หัวตารางตามลำดับตัวอักษรจากนั้นเขียนรหัสลงในเเถวใต้คีย์เรียงจากบนลงล่างจนครบ
4. สลับคีย์ให้อยู่ในรูปแบบเดิมที่เป็นคำภาษาอังกฤษ 
5. อ่านข้อความในเเถวจะได้เป็นข้อความก่อนที่จะเข้ารหัส

---
## See also
- [[ขั้นตอนการเข้ารหัสแบบ Columnar transposition]]
## References
- [Wikipedia,"Columnar transposition,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Columnar_transposition)
- [Chris Christensen,"Columnar transposition,"2015.](https://www.nku.edu/~christensen/1402%20Columnar%20transposition.pdf)
- ["Columnar Transposition Cipher,"2019.](https://www.geeksforgeeks.org/columnar-transposition-cipher/)