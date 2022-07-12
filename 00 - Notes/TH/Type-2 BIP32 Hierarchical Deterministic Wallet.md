---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC Type of HD Wallet]]
tags:: #lang/th #type/thing

# Type-2 BIP32 Hierarchical Deterministic Wallet
*Type-2 BIP32 Hierarchical Deterministic Wallet* หรือ *HD Wallet* คือ [[Deterministic Wallet]] รุ่นที่ 2 ที่ออกมาเพื่อแก้ปัญหาของกระเป๋าตังค์รุ่นแรกอย่าง [[Type-1 Deterministic Wallet]] และเป็นกระเป๋าที่มีการใช้งานอยู่ในปัจจุบัน คิคค้นโดย Gregory Maxwell
- สามารถสร้าง [[Private Key]] ได้ 2 วิธี คือ
	1. [[BIP32 Normal Key Derivation|Normal / Soft / Non-hardened ]]
	2. [[BIP32 Hardened Key Derivation|Hardened / Hard]]
- นำ Chain Code มาใช้เพื่อแก้ปัญหาด้านความปลอดภัยจากกระเป๋ารุ่นที่ 1 โดยมีหลักการดังนี้ 
   -  Extended Private Key = Private Key + Chain Code 
   -  Extended Public Key = Public Key + Chain Code  
   - ถ้าหาก Extended Private Key และ Extended Public Key เป็นคู่ (Key Pair) กัน Chain Code ที่ใช้จะมีค่าเท่ากัน
- สามารถสร้าง Master Private Key, Public Key และ Chain Code  ได้โดยการสุ่มตัวเลขขึ้นมาชุดหนึ่ง เรียกว่า " Root Seed " จากนั้นนำไปเข้า [[Hash Function]] แบบ HMAC-SHA512 จะได้ Output แบ่งออกเป็นด้านซ้าย 256 Bit เป็น Master Private Key นำไปคูณกับค่า G [[Public Key|ค่า base point บน Elliptic Curve (EC)]] จะได้เป็น Master Public Key ส่วนด้านขวา 256 Bit จะเป็น Master Chain Code
-  สามารถสร้าง Parent key และ Child key จาก Master key อันเดียวได้
---
## See also

## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.