---
version: "0.0.0"
published: true
---
uplinks:: [[Cryptography]]
tags:: #type/note #lang/th #people/Sutida

# Secrete Key Cryptography
**ระบบรหัสแบบสมมาตร** (Secrete Key Cryptography หรือ Symmetric-Key Cryptography)
- คือการเข้ารหัสข้อมูลด้วยกุญแจ (Key) เดียวทั้งผู้ส่งและผู้รับโดยวิธีการนี้ผู้รับกับผู้ส่งต้องตกลงกันก่อนว่าจะใช้รูปแบบไหนในการเข้ารหัสข้อมูล
- ผู้ส่งและผู้รับจะใช้กุญเเจที่เหมือนกันหรือสมมาตรกันทั้งสองฝั่ง
- กุญแจ ซึ่งอยู่ในรูปรหัสคอมพิวเตอร์นี้เป็นตัวแปรสำคัญสำหรับการเข้าและถอดรหัสลับข้อมูล ซึ่งขนาดของกุญแจ (มีหน่วยเป็นบิต : bit) จำนวนบิตสูงจะทำให้การเข้ารหัสมีความปลอดภัยมากยิ่งขึ้น
- **ข้อดี** สามารถเข้าเเละถอดรหัสได้รวดเร็ว เมื่อเปรียบเทียบกับแบบ Public Key Cryptography
- **ข้อเสีย** คือการบริหารจัดการกุญเเจ ทำได้ยากเนื่องจากผู้ใช้ต้องใช้กุญเเจ 1 ดอกสำหรับติดต่อกับบุคคล 1 คน ดังนั้นหากเราติดต่อบุคคลจำนวนมากจะต้องมีกุญเเจ จำนวนมากตามไปด้วย รวมถึงการส่งกุญเเจไปยังบุคคลที่ติดต่ออาจเสี่ยงในการถูกขโมยกุญเเจ ได้
- **ตัวอย่าง** วิธีที่ใช้ในระบบรหัสแบบสมมาตร อาทิเช่น AES, Blowfish, DES, Triple DES เป็นต้น

## References
- [บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล](https://www.nrca.go.th/content/02-1.html)
- [Chapter 6: Cryptography](https://sites.google.com/site/suxkarsxnkarraksakhwamplxdphay/chapter-6-cryptography)

## See Also
- [[Public Key Cryptography]]