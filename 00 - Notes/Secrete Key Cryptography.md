## version: "0.0.0"
uplinks:: [[Cryptography]]
tags:: [#type/note](app://obsidian.md/index.html#type/note) [#lang/th](app://obsidian.md/index.html#lang/th) [#people/Sutida](app://obsidian.md/index.html#people/Sutida)

# Secrete Key Cryptography
ระบบรหัสแบบสมมาตร (Secrete Key Cryptography หรือ Symmetric-key Cryptography)
- คือการเข้ารหัสข้อมูลด้วยกุญแจเดี่ยว ทั้งผู้ส่งและผู้รับ โดยวิธีการนี้ผู้รับกับผู้ส่งต้องตกลงกันก่อนว่าจะใช้รูปแบบไหนในการเข้ารหัสข้อมูล
- ผู้ส่งและผู้รับ จะใช้กุญเเจที่เหมือนกัน หรือสมมาตรกันทั้งสองฝั่ง
- กุญแจซึ่งอยู่ในรูปรหัสคอมพิวเตอร์นี้เป็นตัวแปรสำคัญสำหรับการเข้าและถอดรหัสลับข้อมูล ซึ่งขนาดของกุญแจ (มีหน่วยเป็นบิต : bit) จำนวนบิตสูงจะทำให้การเข้ารหัสมีความปลอดภัยมากยิ่งขึ้น
- ข้อดี สามารถเข้าเเละถอดรหัสได้รวดเร็ว เมื่อเปรียบเทียบกับแบบ Public Key Cryptography
- ข้อเสีย คือ การบริหารจัดการกุญเเจทำได้ยากเนื่องจากผู้ใช้ต้องใช้กุญเเจ 1 ดอกสำหรับติดต่อกับบุคคล 1 คน ดังนั้นหากเราติดต่อบุคคลจำนวนมากจะต้องมีกุญเเจจำนวนมากตามไปด้วย รวมถึงการส่งกุญเเจไปยังบุคคลที่ติดต่ออาจเสี่ยงในการถูกขโมยกุญเเจได้
- ตัวอย่างวิธีที่ใช้ในระบบรหัสแบบสมมาตร อาทิเช่น AES, Blowfish, DES, Triple DES เป็นต้น

## References
- [บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล](https://www.nrca.go.th/content/02-1.html)
- [Chapter 6: Cryptography](https://sites.google.com/site/suxkarsxnkarraksakhwamplxdphay/chapter-6-cryptography)

## See Also
- [[Public Key Cryptography]]