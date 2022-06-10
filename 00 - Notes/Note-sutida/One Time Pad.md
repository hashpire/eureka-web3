
---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/term 

# One Time Pad
- *One Time Pad*  (OTP) คือ การเข้ารหัสเเบบสุ่มคีย์ แล้วใช้ครั้งเดียว เป็นการเข้ารหัสรูปแบบเดียวกับ [[Vigenère cipher]] ผู้รับเเละผู้ส่งจะต้องใช้คีย์อันเดียวกันทั้งการเข้ารหัสเเละการถอดรหัส
- ข้อความที่ถูกเข้ารหัสเเบบ One Time Pad  มีข้อได้เปรียบในทางทฤษฎี เพราะคีย์ที่ใช้เป็นการสุ่มเเบบใช้ครั้งเดียว การเข้ารหัสเเต่ละครั้งจะไม่เกี่ยวข้องกัน ทำให้ไม่สามารถวิเคราะห์รูปแบบการเข้ารหัสได้
- ปัญหาที่เกิดจากการเข้ารหัสแบบ OTP คือ ในโลกความเป็นจริง การเข้ารหัสแบบ OTP นั้นเป็นกระบวนการที่ค่อนข้างยากลำบาก เนื่องจากคีย์ที่ใช้มีขนาดเท่ากับข้อความธรรมดา ทำให้การเข้ารหัสทำได้ช้า และมีความลำบากในการส่ง
---
## See also
## References
- ["One Time Pad Cipher,"](https://www.tutorialspoint.com/cryptography_with_python/cryptography_with_python_one_time_pad_cipher.htm)
