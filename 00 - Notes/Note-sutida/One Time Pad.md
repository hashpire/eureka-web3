
---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/term 

# One Time Pad
- *One Time Pad* คือการเข้ารหัสเเบบสุ่มคีย์แล้วใช้ครั้งเดียว เป็นการเข้ารหัสรูปแบบเดียวกับ [[Vigenère cipher]] ผู้รับเเละผู้ส่งจะต้องใช้คีย์อันเดียวกันทั้งการเข้ารหัสเเละการถอดรหัส
- ข้อความที่ถูกเข้ารหัสเเบบ One Time Pad  มีข้อได้เปรียบในทางทฤษฎี เพราะคีย์ที่ใช้เป็นการสุ่มเเบบใช้ครั้งเดียว การเข้ารหัสเเต่ละครั้งจะไม่เกี่ยวข้องกัน ทำให้ไม่สามารถวิเคราะห์รูปแบบการเข้ารหัสได้
- ปัญหาที่เกิดขึ้นจากการเข้ารหัสนี้คือเมื่อทั้งฝ่ายจะต้องใช้คีย์เดียวกันคือการรักษาความปลอดภัยไม่ให้คีย์ถูกขโมยไปเพราะหากคีย์ถูกขโมยข้อความลับที่เข้ารหัสจะถูกถอดรหัสได้โดยง่าย

---
## See also

## References
- ["One Time Pad Cipher,"](https://www.tutorialspoint.com/cryptography_with_python/cryptography_with_python_one_time_pad_cipher.htm)