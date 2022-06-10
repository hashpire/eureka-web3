---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการเข้ารหัสแบบ Alberti cipher
1. กำหนดข้อความที่ต้องการจะเข้ารหัส เช่น *VENETIAN CRVPTOGRAPFIES* (CRVPTOGRAPFIES มีการปรับมาจาก CRYPTOGRAPHIES เพื่อให้ตรงกับตัวอักษรที่มีในวงแหวนรอบนอก)
2.  หากข้อความมีช่องว่างสามารถ ใส่ค่า Null แบบสุ่ม ลงไปในช่องว่างระหว่างตัวอักษรได้
3. กำหนดตัวอักษรเริ่มต้นของวงแหวนด้านในเป็น m และวงแหวนรอบนอกเป็น T สำหรับข้อความแรก และสำหรับข้อความหลังเป็น F  จะได้ *mVENETIAN mCRVPTOGRAPFIES* 
4. หมุนตัวอักษร T วงแหวนด้านนอกให้ตรงกับ m ตัวอักษรเริ่มต้นที่กำหนด ดังรูปที่ 2 
![[Alberti cipher-2.png|250]]
5. T จะกลายเป็นอักษรตัวแรกของข้อความเข้ารหัสของเรา เพื่อแสดงให้เห็นว่า เวลาถอดรหัสต้องเริ่มต้นจากที่ใด
6. เทียบข้อความที่ต้องการเข้ารหัส โดย เทียบกับวงแหวนด้านนอกแล้วเขียนรหัสจากวงแหวนด้านใน  ข้อความคือ VENETIAN จะได้ *Tblzlmrcz*
7.  จากนั้นที่ข้อความหลัง จุดเริ่มต้นเป็น m หมุนตัวอักษร F ให้ตรงกับ m  ดังนั้น F จะเป็นตัวขึ้นต้นข้อความหลัง ดังรูปที่ 3 
![[Alberti cipher-3.png|250]]
8. เทียบข้อความเข้ารหัส ข้อความคือ CRVPTOGRAPFIES จะได้ *Fyelakbqe&amiog*  
9. ดังนั้นข้อความ  *mVENETIAN mCRVPTOGRAPFIES*  จะเข้ารหัสได้เป็น *TblzlmrczFyelakbqe&amiog*
---
## See also
- [[Alberti cipher]]
- [[ขั้นตอนการถอดรหัสแบบ Alberti cipher]]
## References
- ["Alberti cipher"](https://vcrypto.tonyo.info/venetian_crypto/website/index.php/alberti)
 