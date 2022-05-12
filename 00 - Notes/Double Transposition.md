---
version: "0.0.0"
published: true
cover_image:
---
uplinks:: [[Transposition Cipher]]
tags:: #type/note #lang/th #people/Sutida 
# Double Transposition
- *Double Transposition* คือรูปแบบการเข้ารหัสที่เป็นการทำ [[Columnar Transposition]] 2 ครั้ง 
- คือเราจะทำการเข้ารหัสโดยการย้ายคอลัมน์ 2 ครั้งเเละทั้งสองครั้งจะใช้คีย์ที่เเตกต่างกันไป
- Double Transposition เป็นหนึ่งในการเข้ารหัสที่ถือว่าปลอดภัยมากเเละยังเคยถูกใช้ในสงครามโลกครั้งที่ 2 อีกด้วย
- **ขั้นตอนการเข้ารหัสแบบ Double Transposition จะทำเหมือนกับการทำ Columnar Transposition** 
	1. กำหนดข้อความที่ต้องการเข้ารหัส คือ *DOUBLE TRANSPOSITION CIPHER*
	2. กำหนดคีย์ คือคำว่า *AVOID*
	3. คำนวณตารางโดยเอาจำนวนตัวอักษรในข้อความหารด้วยจำตัวอักษรในคีย์ คือ 25/5 เท่ากับ 5 จะได้ตารางเป็นเเบบ 5 คอลัมน์ 5 เเถว
	4. สร้างตารางตามที่คำนวณไว้
	5.  นำข้อความต้นฉบับไปใส่ในตารางโดยเรียงจากซ้ายไปขวา(ใส่คีย์ไว้บนหัวตาราง)
	6. เมื่อใส่ตัวอักษรจนครบให้ทำการเรียงคีย์ตามลำดับตัวอักษรเเล้วนำตัวอักษรในแต่ละคอลัมน์ที่อยู่ใต้คีย์ออกมาเขียนจะได้เป็นรหัสที่ต้องการ (การเรียงลำดับตัวอักษรหากมีตัวที่ซ้ำกันให้เลือกตัวที่มาก่อนในคำนั้นเป็นลำดับเเรก)
	    ![[Double Transposition-1.png|500]]
	7.  เข้ารหัสครั้งที่ 1 จะได้ *DESTILNICRBASNEUROOHOTPIP*
	8. จากนั้นทำการเข้ารหัสครั้งที่ 2 โดยกำหนดคีย์ใหม่ คือคำว่า *BLIND*
	9. นำรหัสที่ได้จากครั้งที่ 1 ใส่ลงในตาราง เรียงตามเเถวจากซ้ายไปขวา
	10. ทำตามขั้นตอนที่ 6 เรียงตัวอักษรตามลำดับ
	 ![[Double Transposition-2.png|500]]
	10. เข้ารหัสครั้งที่ 2 จะได้ *DLBUOIREHPSISOPENARTTCNOI*
---
- **ขั้นตอนการถอดรหัส Double Transposition**
  คือการทำขั้นตอนขั้นรหัสจากหลังไปหน้า 2 ครั้ง
    1. การถอดรหัสเราจะต้องทราบคีย์ในการถอดรหัสเเละรหัสที่ต้องการถอด
	2. คำนวณตารางโดยการเอารหัสที่ได้รับหารกับคีย์ 25/5 เท่ากับ 5 จะได้         
       ตารางเเบบ 5 คอลัมน์ 5 เเถว
	3. สร้างตารางเเล้วนำเอาคีย์ไปใส่ที่หัวตารางโดยเรียงตามลำดับตัวอักษร
	4. จากนั้นสลับตำแหน่งให้ตารางโดยการเรียงคีย์ให้กลับไปเป็นรูปแบบเดิม คือ   *BLIND* เป็น *BLIND* 
	5. จะได้ตารางก่อนในรูปแบบก่อนที่จะทำการเข้ารหัสครั้งที่ 2
       ![[Double Transposition-4.png|500]]
	6.  จะได้รหัสของการเข้ารหัสครั้งที่ 2 ออกมา คือ *DLBUOIREHPSISOPENARTTCNOI*
	7. ทำขั้นตอนที่ 1-4 ซ้ำอีกครั้งโดยใช้คีย์ *ADIOV* และสลับเป็น *AVOID*
      ![[Double Transposition-3.png|500]]
	6. จะได้ข้อความก่อนเข้ารหัสออกมา เป็น *DOUBLE TRANSPOSITION CIPHER*
---
## References
- [Double Transposition](https://crypto.interactive-maths.com/columnar-transposition-cipher.html)
- [Double_transposition](https://en.wikipedia.org/wiki/Transposition_cipher#Double_transposition)
- [The Double Transposition Cipher](https://www.pbs.org/wgbh/nova/decoding/doubtrans.html)
## See Also
