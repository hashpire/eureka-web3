---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Web 3]]
tags:: #lang/th #type/term

# Secret Key Cryptography
*Secret Key Cryptography*หรือ *Symmetric-Key Cryptography* คือ ระบบการเข้ารหัสแบบสมมาตร เป็นการเข้ารหัสด้วยกุญแจ (Key) เดียวกันทั้งผู้ส่งและผู้รับ โดยวิธีการนี้ผู้รับกับผู้ส่งต้องตกลงกันก่อนว่าจะใช้รูปแบบใดในการเข้ารหัส
- *ข้อดี* คือ สามารถเข้าเเละถอดรหัสได้รวดเร็ว เมื่อเปรียบเทียบกับแบบ[[Public Key Cryptography]]
- *ข้อเสีย* คือ การบริหารจัดการกุญแจทำได้ยาก เนื่องจากผู้ใช้ต้องใช้กุญแจ 1 ดอกสำหรับติดต่อกับบุคคล 1 คน ดังนั้น หากเราติดต่อบุคคลจำนวนมากจะต้องมีกุญแจจำนวนมากตามไปด้วย รวมถึงการส่งกุญแจไปยังบุคคลที่ติดต่ออาจเสี่ยงในการถูกขโมยกุญแจได้
- *ตัวอย่าง* เช่น AES, Blowfish, DES, Triple DES เป็นต้น
---
## See also
- [[Encryption]]
- [[Decryption]]
## References
- ["บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล,"2560.](https://www.nrca.go.th/content/02-1.html)
- ["Chapter 6: Cryptography"](https://sites.google.com/site/suxkarsxnkarraksakhwamplxdphay/chapter-6-cryptography)
