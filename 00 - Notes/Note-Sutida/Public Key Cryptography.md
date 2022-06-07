---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Web 3]]
tags:: #lang/th #type/term

# Public Key Cryptography
- *Public Key Cryptography* หรือ *Asymmetric Key Cryptography* คือ การเข้ารหัสเเบบอสมมาตร เป็นระบบกุญแจคู่ (Key Pair) ประกอบด้วย 
	- **กุญแจส่วนตัว** (Private Key) หมายความถึง กุญแจที่ใช้ในการสร้างลายมือชื่อดิจิทัล 
	- **กุญแจสาธารณะ** (Public Key) หมายความถึง กุญแจที่ใช้ในการตรวจสอบลายมือชื่อดิจิทัล
- การเก็บรักษากุญแจ คือ กุญเเจส่วนตัวห้ามให้บุคคลอื่นทราบ แต่กุญแจสาธารณะสามารถเปิดเผยให้บุคคลสืบค้นได้
- การเข้ารหัสจะต้องใช้กุญแจคู่กันโดย
	- หากใช้กุญแจสาธารณะในการเข้ารหัสลับ ก็จะต้องใช้กุญแจส่วนตัวในการถอดรหัสลับ  
	- หากใช้กุญแจส่วนตัวในการเข้ารหัสลับ ก็จะต้องใช้กุญแจสาธารณะในการถอดรหัสลับ
	- การเลือกรูปแบบการใช้ขึ้นอยู่กับวัตถุประสงค์ของการใช้งาน เช่น [[Encryption]], [[Digital Signature]] เป็นต้น
- *ข้อดี* เจ้าของกุญแจไม่ต้องเก็บกุญเเจจำนวนมาก ทำให้การบริหารจัดการกุญเเจทำง่ายและเป็นระบบมากขึ้น
- *ข้อเสีย* เข้า/ถอดรหัสได้ช้า เมื่อเปรียบเทียบกับแบบ [[Secret Key Cryptography]]
- *ตัวอย่าง* เช่น RSA ซึ่งเป็นระบบเเรกของ Public Key Cryptography คิดค้นโดย Rivest, Shamir และ Adleman ซึ่งเผยแพร่ในปี 1978 เป็นต้น 
---
## See also
- [[Encryption]]
- [[Decryption]]
## References
- ["บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล,"2560.](https://www.nrca.go.th/content/02-1.html)
- ["Chapter 6: Cryptography"](https://sites.google.com/site/suxkarsxnkarraksakhwamplxdphay/chapter-6-cryptography)
