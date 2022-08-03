---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]

---
uplinks::[MOC Type of HD Wallet](./MOC Type of HD Wallet.md)
tags:: #lang/th #type/thing

# Deterministic Wallet
*Deterministic Wallet* คือ กระเป๋าตังค[Blockchain Wallets|(Blockchain Wallets)](./Blockchain Wallets|(Blockchain Wallets).md)ี่ถูกออกแบบมาเพื่อแก้ปัญหาที่เกิดขึ้นจากการใช้กระเป๋าตังค์รุ่นแรกอย่า[Non-deterministic Wallet](./Non-deterministic Wallet.md)
- การสร้าง[Private key](./Private key.md)จะทำโดยการสุ่มตัวเลขที่ขนาดใหญ่และต้องเก็บเป็นความลับ ขึ้นมา 1 ชุด เรียกว่า "Seed" จากนั้นนำไปเข้า key derivation function (KDF) เพื่อให้ได้ Private key ออกมา
- จุดเด่นของ Deterministic Wallet คือ มันจะกำหน[Private Key](./Private Key.md)และ[Address](./Address.md)ให้ล่วงหน้าแล้ว 
- ข้อดี คือ เราจะสำรองข้อมูลเพียงเเค่ Seed อย่างเดียว จะเท่ากับเราสำรองข้อมูลทั้งหมดของกระเป๋าตังค์ไว้แล้ว
- ตัวอย่าง การใช้ค่า Seed สร้าง Private Key ใน[MetaMask](./MetaMask.md)ค่า Seed จะถูกกำหนดมาจาก human-writeable words หรือ mnemonic code (BIP39) เป็นคำศัพท์ภาษาอังกฤษ 12 คำ ที่ถูกสุ่มมาจากคำศัพท์ทั้งหมดใน Wordlists (Seed มีหลายภาษา แต่แนะนำให้ใช้ภาษาอังกฤษ) ซึ่งการทำให้ seed อยู่ในรูปแบบคำศัพท์ จะทำให้ไม่ต้องจำค่าที่เป็นตัวเลขจำนวนมาก และป้องกันการผิดพลาดในการใช้งานได้

## See also
-[Type-1 Deterministic Wallet](./Type-1 Deterministic Wallet.md)
-[Type-2 BIP32 Hierarchical Deterministic Wallet](./Type-2 BIP32 Hierarchical Deterministic Wallet.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A deeper look into Hierarchical Deterministic Wallets.md)"2022.

