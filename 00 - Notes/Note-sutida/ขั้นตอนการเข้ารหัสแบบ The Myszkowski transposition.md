---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ The Myszkowski transposition
1. กำหนดข้อความที่ต้องการเข้ารหัส  เช่น *A COLLABORATIVE SPACE FOR PEOPLE TO LEARN WEB THREE*
2. กำหนดคีย์ เช่น *HASHPIRE*
3. คำนวณตาราง โดยเอาจำนวนตัวอักษรในข้อความหารด้วยจำตัวอักษรในคีย์ เช่น จำนวนตัวอักษรในข้อความคือ 39 ตัว และตัวอักษรในคีย์คือ 8 ตัว จะได้ 39/8 เท่ากับ 5 ตารางจะเป็นเเบบ 8 คอลัมน์ 5 เเถว และสร้างตารางตามที่คำนวณไว้
4. นำข้อความต้นฉบับไปใส่ในตารางโดยเรียงจากซ้ายไปขวา(ใส่คีย์ไว้บนหัวตาราง)  
  (เเต่หากข้อความไม่สามารถคำนวณได้ลงตัวตารางที่ว่างสามารถใส่ค่า null ลงไปได้) ดังรูปที่ 1
       ![[The Myszkowski transposition.png|300]]
5. เมื่อใส่ตัวอักษรจนครบ ให้ทำการเข้ารหัส ตามลำดับตัวอักษรของคีย์ เเล้วนำตัวอักษรในแต่ละแถวที่อยู่ใต้คอลัมน์คีย์ออกมาเขียน จะได้เป็นรหัสที่ต้องการ 
6. จากรูปที่ 1 จะเห็นว่ามีเส้นปะโยงจากคอลัมน์ที่มีคีย์ซ้ำกัน ให้จับคู่อักษรในแถวใต้คอลัมน์ไปคู่กัน จะได้ *ALRIAFOEAWRX*
7. เข้ารหัสตามลำดับตัวอักษรของคีย์ทั้งหมดได้เป็น *CACPR EOPEE HXALR IAFOE AWRXA EROBX LVOTE XBSPL TXOTE LNE* ซึ่งเราสามารถเขียนรหัสเรียงติดกันทั้งหมดหรือเขียนเป็นกลุ่มละ 5 ตัวอักษรก็ได้
---
## See also
- [[The Myszkowski transposition]]
- [[ขั้นตอนการถอดรหัสแบบ The Myszkowski transposition]]
## References
 - ["Myszkowski Transposition Cipher"](https://crypto.interactive-maths.com/myszkowski-transposition-cipher.html)
- [Wikipedia,"Myszkowski transposition,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Myszkowski_transposition)
