---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Type of HD Wallet](./MOC%20Type%20of%20HD%20Wallet.md)
tags:: #lang/th #type/thing

# Type-2 BIP32 Hierarchical Deterministic Wallet
*Type-2 BIP32 Hierarchical Deterministic Wallet* หรือ *HD Wallet* คือ[Deterministic Wallet](./Deterministic%20Wallet.md)รุ่นที่ 2 ที่ออกมาเพื่อแก้ปัญหาของกระเป๋าตังค์รุ่นแรกอย่าง[Type-1 Deterministic Wallet](./Type-1%20Deterministi%20Wallet.md)และเป็นกระเป๋าที่มีการใช้งานอยู่ในปัจจุบัน คิคค้นโดย Gregory Maxwell
- สามารถสร้าง[Private Key](./Private%20Key.md)ได้ 2 วิธี คือ
	1.[BIP32 Normal Key Derivation|Normal / Soft / Non-hardened ](./BIP32 Normal Key Derivation|Normal / Soft / Non-hardened .md)
	2.[BIP32 Hardened Key Derivation|Hardened / Hard](./BIP32 Hardened Key Derivation|Hardened / Hard.md)
- นำ Chain Code มาใช้เพื่อแก้ปัญหาด้านความปลอดภัยจากกระเป๋ารุ่นที่ 1 โดยมีหลักการดังนี้ 
   -  Extended Private Key = Private Key + Chain Code 
   -  Extended Public Key = Public Key + Chain Code  
   - ถ้าหาก Extended Private Key และ Extended Public Key เป็นคู่ (Key Pair) กัน Chain Code ที่ใช้จะมีค่าเท่ากัน
- สามารถสร้าง Master Private Key, Public Key และ Chain Code  ได้โดยการสุ่มตัวเลขขึ้นมาชุดหนึ่ง เรียกว่า " Root Seed " จากนั้นนำไปเข้า[Hash Function](./Hash%20Function.md)แบบ HMAC-SHA512 จะได้ Output แบ่งออกเป็นด้านซ้าย 256 Bit เป็น Master Private Key นำไปคูณกับค่า G[Public Key|ค่า base point บน Elliptic Curve (EC)](./Public%20Key|ค่า%20base%20point%20บน%20Elliptic%20Curve%20(EC).md)จะได้เป็น Master Public Key ส่วนด้านขวา 256 Bit จะเป็น Master Chain Code
-  สามารถสร้าง Parent key และ Child key จาก Master key อันเดียวได้
---
## See also

## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A%20deeper%20look%20into%20Hierarchical%20Deterministic%20Wallets.md)"2022.