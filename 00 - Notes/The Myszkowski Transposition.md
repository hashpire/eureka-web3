---
version: "0.0.0"
published: true
cover_image:
---
uplinks:: [[Transposition Cipher]]
tags:: #type/note #lang/th #people/Sutida 
# The Myszkowski Transposition
- *Myszkowski Transposition* คือการเข้ารหัสรูปแบบหนึ่งที่เหมือนกับ [[Columnar Transposition]] 
- ถูกเสนอโดย Émile Victor Théodore Myszkowski ในปี 1902
- Myszkowski Transposition จะใช้วิธีการย้ายคอลัมน์ เหมือนกับใน Columnar Transposition ที่จะมีข้อความธรรมดาอยู่ในเเถวเเละมีคีย์อยู่บนหัวตารางเป็นคอลัมน์ 
- *ข้อเเตกต่างของ Myszkowski Transposition* กับ  Columnar Transposition มีเพียงอย่างเดียว คือ เมื่อมีตัวอักษรซ้ำกันในคีย์ตำแหน่งเลขเดียวกันหากเป็นใน Columnar Transposition เราจะมีการเรียงลำดับให้ตัวเเรกในคีย์มาก่อน เเต่ใน Myszkowski Transposition เราจะอ่านคอลัมน์ที่มีตัวอักษรซ้ำกันไปพร้อมกัน คือ อ่านตัวอักษรในคอลัมน์คู่กันจนครบ
 - **ขั้นตอนการเข้ารหัสเเบบ Myszkowski Transposition**
	1. กำหนดข้อความที่ต้องการเข้ารหัส คือ *A COLLABORATIVE SPACE FOR PEOPLE TO LEARN WEB THREE*
	2. กำหนดคีย์ คือคำว่า *HASHPIRE*
	3. คำนวณตารางโดยเอาจำนวนตัวอักษรในข้อความหารด้วยจำตัวอักษรในคีย์ คือ 39/8 เท่ากับ 5 จะได้ตารางเป็นเเบบ 8 คอลัมน์ 5 เเถว
	4. สร้างตารางตามที่คำนวณไว้
	5.  นำข้อความต้นฉบับไปใส่ในตารางโดยเรียงจากซ้ายไปขวา(ใส่คีย์ไว้บนหัวตาราง)
	6. เมื่อใส่ตัวอักษรจนครบให้ทำการเรียงคีย์ตามลำดับตัวอักษรเเล้วนำตัวอักษรในแต่ละคอลัมน์ที่อยู่ใต้คีย์ออกมาเขียนจะได้เป็นรหัสที่ต้องการ 
	![[The Myszkowski Transposition-1.png|700]]
	7. ในกรณีที่ตัวอักษรไม่ครบตามตารางให้ใส่ตัวอักษรที่ไม่มีความหมายหรือทำไม่ให้ข้อความผิดเพี้ยนไปเเทนไว้ เช่น ตัว X แบบในตัวอย่าง
	8. ในกรอบเส้นประสีเเดงในรูปคือตัวอักษรที่อยู่ในคอลัมน์ที่มีคีย์ซ้ำกัน คือ H ให้จับคู่ตัวอักษรในคอลัมน์นั้น เช่นในตัวอย่าง เป็น *ALRIAFOEAWRX*
	9. จะเข้ารหัสได้เป็น *CACPREOPEEHXALRIAFOEAWRXAEROBXLVOTEXBSPLTXOTELNE*
---
- **ขั้นตอนการถอดรหัส Myszkowski Transposition**
    1. การถอดรหัสเราจะต้องทราบคีย์ในการถอดรหัสเเละรหัสที่ต้องการถอด
	2. คำนวณตารางโดยการเอารหัสที่ได้รับหารกับคีย์ 39/8 เท่ากับ 5 จะได้         
       ตารางเเบบ 8 คอลัมน์ 5 เเถว
	3. สร้างตารางเเล้วนำเอาคีย์ไปใส่ที่หัวตารางโดยเรียงตามลำดับตัวอักษร
	4. จากนั้นสลับตำแหน่งให้ตารางโดยการเรียงคีย์ให้กลับไปเป็นรูปแบบเดิม คือ  
     *AEHHIPRS* เป็น *HASHPIRE*
	5. จะได้ตารางก่อนในรูปแบบก่อนที่จะทำการเข้ารหัสออกมา *ตรงส่วนนี้อย่าลืมว่าตอนที่นำรหัสมาใส่ในตารางคอลัมน์ที่คีย์เหมือนกันจะต้องใส่มันเป็นคู่กันพร้อมกันเรียงจนครบตาราง ห้ามใส่ที่ละเเถวเด็ดขาด*
     ![[The Myszkowski Transposition-2.png|700]]
	  6. จะได้เป็นข้อความต้นฉบับก่อนเข้ารหัส *A COLLABORATIVE SPACE FOR PEOPLE TO LEARN WEB THREE*
---
การเข้ารหัสเเบบ Myszkowski Transposition นั้นเหมือนกับ Columnar Transposition ทุกประการยกเว้นเรื่องเดียวคือการจับคู่คอลัมน์ของตัวคีย์ที่ซ้ำกัน ซึ่งต้องระมัดระวังในการทำส่วนนี้เพราะอาจจะทำให้เกิดความซ้ำสนได้ง่าย

---
## References
- [The Myszkowski Transposition Cipher](https://crypto.interactive-maths.com/myszkowski-transposition-cipher.html)
- [Myszkowski-Transposition](https://en.wikipedia.org/wiki/Transposition_cipher#Myszkowski_transposition)
## See Also