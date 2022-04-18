## version: "0.0.0"
uplinks:: [[Cryptographic primitives in blockchains]]
tags:: [#type/note](app://obsidian.md/index.html#type/note) [#lang/th](app://obsidian.md/index.html#lang/th) [#people/Sutida](app://obsidian.md/index.html#people/Sutida)

#  Crytography
- วิทยาการเข้ารหัสลับเกี่ยวกับการเข้ารหัสลับคือการแปลงข้อความปกติให้กลายเป็นข้อความลับ 
- ข้อความลับคือข้อความที่ผู้อื่น นอกเหนือจากคู่สนทนาที่ต้องการ ไม่สามารถเข้าใจได้เป็นกระบวนการสำหรับการแปรรูปข้อมูลอิเล็กทรอนิกส์ธรรมดาให้อยู่ในรูปที่บุคคลทั่วไปไม่สามารถอ่านเข้าใจได้ 
- โดยทั่วไปแล้วการเข้ารหัสจะกระทำก่อนการจัดเก็บข้อมูลหรือก่อนการส่งข้อมูล โดยการนำข้อมูลอิเล็กทรอนิกส์ธรรมดากับกุญแจ (key) ซึ่งเป็นตัวเลขสุ่มใดๆ มาผ่านกระบวนการทางคณิตศาสตร์ ผลที่ได้ก็คือข้อมูลที่เข้ารหัส ขั้นตอนที่กล่าวมานี้จะเรียกว่า “การเข้ารหัส” (encryption) 
- เมื่อต้องการอ่านข้อมูล ก็นำเอาข้อมูลที่เข้ารหัสกับกุญแจมาผ่านกระบวนการทางคณิตศาสตร์ ผลลัพธ์ที่ได้ก็คือข้อมูลดั้งเดิม ซึ่งขั้นตอนนี้จะเรียกว่า “การถอดรหัส” (decryption) ระบบเข้ารหัสสามารถแบ่งตามวิธีการใช้กุญแจได้เป็น 2 วิธี 
	- [[Secrete Key Cryptography]] (Symmetric Key Cryptography)
	- [[Public Key Cryptography]] (Asymmetric Key Cryptography)

## References
- [บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล](https://www.nrca.go.th/content/02-1.html)
- [Cryptography (การเข้ารหัสข้อมูล)](https://medium.com/@winyou.info/%E0%B8%88%E0%B8%B0%E0%B8%87%E0%B9%88%E0%B8%B2%E0%B8%A2%E0%B9%84%E0%B8%9B%E0%B9%84%E0%B8%AB%E0%B8%99-cryptography-%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%80%E0%B8%82%E0%B9%89%E0%B8%B2%E0%B8%A3%E0%B8%AB%E0%B8%B1%E0%B8%AA%E0%B8%82%E0%B9%89%E0%B8%AD%E0%B8%A1%E0%B8%B9%E0%B8%A5-1c2df888863f)
- [Chapter 6: Cryptography](https://sites.google.com/site/suxkarsxnkarraksakhwamplxdphay/chapter-6-cryptography)

## See Also