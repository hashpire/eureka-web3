---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]

---
uplinks::[[MOC Type of HD Wallet]]
tags:: #lang/th #type/thing

# Type-1 Deterministic Wallet
*Type-1 Deterministic Wallet* คือ [[Deterministic Wallet]] รุ่นแรก 
- สร้าง [[Private key]]โดยการใช้ key derivation function (KDF) $Private Key_i = H(i||Seed||Type)$ ซึ่งประกอบด้วย  
	-  Identifier (id) ค่าเลขทั่วๆ ไป ที่เป็นค่า Pubilc เช่น ถ้า i=1 จะได้ Private key 1,  i=2 จะได้ Private key 2 เป็นต้น 
	- [[Deterministic Wallet|Seed ค่าตัวเลขสุ่ม]]
	- Type ตัวที่ใช้ในการแยกประเภท เป็นค่า Pubilc เช่น Type Bitcoin , Type Ethereum เป็นต้น
จากนั้นนำไปเข้า[[Hash Function]] จะได้ Private key ออกมา
---
## See also
- [[Problems and Shortcomings of Type-1 deterministic Wallet]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.
