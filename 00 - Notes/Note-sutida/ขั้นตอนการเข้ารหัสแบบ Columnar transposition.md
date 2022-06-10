---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Columnar transposition
1. กำหนดข้อความที่ต้องการเข้ารหัส เช่น *THE CENTRAL INTELLIGENCE AGENCY.*
2. กำหนดคีย์จากคำภาษาอังกฤษ เช่น *ANALYST* และนำตัวอักษรในคำมาเรียงตามลำดับ จะได้  A=1, N=4, A=2, L=3, Y=7, S=5, T=6 
3. กำหนดตาราง โดยขนาดของตารางสามารถคำนวณได้จากจำนวนของตัวอักษรในข้อความหารด้วยจำนวณของตัวอักษรในคีย์ เช่น ถ้าข้อความมี 20 ตัวอักษร เเละคีย์มี 5 ตัวอักษร เป็น 20/5 จะได้ ตารางแบบ 5 คอลัมน์ 4 แถว (เเต่หากข้อความไม่สามารถคำนวณได้ลงตัวตารางที่ว่างสามารถใส่ค่า null ลงไปได้)
4. นำคีย์และลำดับตัวอักษรของคีย์แต่ละตัวไปใส่ไว้ที่คอลัมน์บนหัวตาราง ดังรูปที่ 1
5. เขียนข้อความลงในตารางใต้คอลัมน์คีย์เรียงจากซ้ายไปขวาจนครบ ดังรูปที่ 1
6. นำตัวอักษรที่อยู่ในเเถวใต้คอลัมน์คีย์เรียงตามลำดับตัวอักษรของคีย์ออกมาเขียน จะได้เป็นรหัสลับ ซึ่งเราสามารถเขียนรหัสเรียงติดกันทั้งหมดหรือเขียนเป็นกลุ่มละ 5 ตัวอักษรก็ได้
![[Columnar Transposition.png|400]]
จากตัวอย่างในรูปที่ 1 จะเข้ารหัสได้เป็น *TRLEE LIGCI GEHAL ANTNC TECYE NEN*

---
## See also
- [[Columnar transposition]]
- [[ขั้นตอนการถอดรหัส Columnar transposition]]
## References
- [Wikipedia,"Columnar transposition,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Columnar_transposition)
- [Chris Christensen,"Columnar transposition,"2015.](https://www.nku.edu/~christensen/1402%20Columnar%20transposition.pdf)
- ["Columnar Transposition Cipher,"2019.](https://www.geeksforgeeks.org/columnar-transposition-cipher/)
