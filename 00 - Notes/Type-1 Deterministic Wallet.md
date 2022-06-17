---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [MOC HD Wallet](./MOC%20HD%20Wallet)
tags:: #lang/th #type/thing

# Type-1 Deterministic Wallet
*Type-1 Deterministic Wallet* คือ [Deterministic Wallet](./Deterministic%20Wallet) รุ่นแรก 
- สร้าง [Private key](./Private%20key) โดยการใช้ key derivation function (KDF) $Private Key_i = H(i||Seed||Type)$ ซึ่งประกอบด้วย  
	-  Identifier (id) ค่าเลขทั่วๆ ไป ที่เป็นค่า Pubilc เช่น ถ้า i=1 จะได้ Private key 1,  i=2 จะได้ Private key 2 เป็นต้น 
	- [Seed ค่าตัวเลขสุ่ม](./Deterministic%20Wallet)
	- Type ตัวที่ใช้ในการแยกประเภท เป็นค่า Pubilc เช่น Type Bitcoin , Type Ethereum เป็นต้น
จากนั้นนำไปเข้า [Hash Function](Hash%20Function.md) จะได้ Private key ออกมา
---
## See also
- [Problems and Shortcomings of Type-1 deterministic Wallet](Problems%20and%20Shortcomings%20of%20Type-1%20deterministic%20Wallet.md)
## References