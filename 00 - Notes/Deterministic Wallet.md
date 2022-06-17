---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [MOC HD Wallet](./MOC%20HD%20Wallet)
tags:: #lang/th #type/thing

# Deterministic Wallet
*Deterministic Wallet* คือ กระเป๋าตังค์[(Blockchain Wallets)](./Blockchain%20Wallets)ที่ถูกออกแบบมาเพื่อแก้ปัญหาที่เกิดขึ้นจากการใช้กระเป๋าตังค์รุ่นแรกอย่าง[Non-deterministic Wallet](./Non-deterministic%20Wallet) 
- การสร้าง [Private key](./Private%20key) จะทำโดยการสุ่มตัวเลขที่ขนาดใหญ่และต้องเก็บเป็นความลับ ขึ้นมา 1 ชุด เรียกว่า "Seed" จากนั้นนำไปเข้า key derivation function (KDF) เพื่อให้ได้ Private key ออกมา
- จุดเด่นของ Deterministic Wallet คือ มันจะกำหนด [Private Key](./Private%20Key) และ [Address](./Address) ให้ล่วงหน้าแล้ว 
- ข้อดี คือ เราจะสำรองข้อมูลเพียงเเค่ Seed อย่างเดียว จะเท่ากับเราสำรองข้อมูลทั้งหมดของกระเป๋าตังค์ไว้แล้ว
- ตัวอย่าง การใช้ค่า Seed สร้าง Private Key ใน [MetaMask](./MetaMask) ค่า Seed จะถูกกำหนดมาจาก human-writeable words หรือ mnemonic code (BIP39) เป็นคำศัพท์ภาษาอังกฤษ 12 คำ ที่ถูกสุ่มมาจากคำศัพท์ทั้งหมดใน Wordlists (Seed มีหลายภาษา แต่แนะนำให้ใช้ภาษาอังกฤษ) ซึ่งการทำให้ seed อยู่ในรูปแบบคำศัพท์ จะทำให้ไม่ต้องจำค่าที่เป็นตัวเลขจำนวนมาก และป้องกันการผิดพลาดในการใช้งานได้

## See also
- [[Type-1 Deterministic Wallet]]
- [[Type-2 BIP32 Hierarchical Deterministic Wallet]]
## References
- [[A deeper look into Hierarchical Deterministic Wallets|Anakorn Kyavatanakij,"A deeper look into Hierarchical Deterministic Wallets,"2022.]]

