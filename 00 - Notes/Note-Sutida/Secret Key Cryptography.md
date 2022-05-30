---
version: "0.0.1"
cover_image:
published: "ture"
contributors: ["Sutida"]
---
uplinks:: [[Cryptography]] 
tags:: #lang/th #type/concept

# Secret Key Cryptography
*Secret Key Cryptography*หรือ *Symmetric-Key Cryptography* คือระบบการเข้ารหัสแบบสมมาตร เป็นการเข้ารหัสด้วยกุญแจ (Key) เดียวกันทั้งผู้ส่งและผู้รับโดยวิธีการนี้ผู้รับกับผู้ส่งต้องตกลงกันก่อนว่าจะใช้รูปแบบไหนในการเข้ารหัส
- *ข้อดี* คือสามารถเข้าเเละถอดรหัสได้รวดเร็วเมื่อเปรียบเทียบกับแบบ[[Public Key Cryptography]]
- *ข้อเสีย* คือการบริหารจัดการกุญแจทำได้ยากเนื่องจากผู้ใช้ต้องใช้กุญแจ 1 ดอกสำหรับติดต่อกับบุคคล 1 คน ดังนั้นหากเราติดต่อบุคคลจำนวนมากจะต้องมีกุญแจจำนวนมากตามไปด้วยรวมถึงการส่งกุญแจไปยังบุคคลที่ติดต่ออาจเสี่ยงในการถูกขโมยกุญแจได้
- *ตัวอย่าง* เช่น AES, Blowfish, DES, Triple DES เป็นต้น
---
## References
- ["บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล,"2560.](https://www.nrca.go.th/content/02-1.html)
- ["Chapter 6: Cryptography"](https://sites.google.com/site/suxkarsxnkarraksakhwamplxdphay/chapter-6-cryptography)
## See also
- [[Encryption]]
- [[Decryption]]
