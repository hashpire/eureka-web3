---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]

---
uplinks:[MOC Type of HD Wallet](./MOC Type of HD Wallet.md)
tags:: #lang/th #type/thing

# Type-1 Deterministic Wallet
*Type-1 Deterministic Wallet* คือ[Deterministic Wallet](./Deterministic Wallet.md)รุ่นแรก 
- สร้าง[Private key](./Private key.md)ดยการใช้ key derivation function (KDF) $Private Key_i = H(i||Seed||Type)$ ซึ่งประกอบด้วย  
	-  Identifier (id) ค่าเลขทั่วๆ ไป ที่เป็นค่า Pubilc เช่น ถ้า i=1 จะได้ Private key 1,  i=2 จะได้ Private key 2 เป็นต้น 
	-[Deterministic Wallet|Seed ค่าตัวเลขสุ่ม](./Deterministic Wallet|Seed ค่าตัวเลขสุ่ม.md)
	- Type ตัวที่ใช้ในการแยกประเภท เป็นค่า Pubilc เช่น Type Bitcoin , Type Ethereum เป็นต้น
จากนั้นนำไปเข้[Hash Function](./Hash Function.md)จะได้ Private key ออกมา
---
## See also
-[Problems and Shortcomings of Type-1 deterministic Wallet](./Problems and Shortcomings of Type-1 deterministic Wallet.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A deeper look into Hierarchical Deterministic Wallets.md)"2022.
