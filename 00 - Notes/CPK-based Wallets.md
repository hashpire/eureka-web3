---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC Type of HD Wallet]]
tags:: #lang/th #type/thing

# CPK-based Wallets
*CPK (Combined Public Key)* เป็นอัลกอรึทึม ในการทำ identity-based large-scale key management  คิดค้นและเผยแพร่ โดย Nan Xianghao นักวิชาการชาวจีน ในปี 1999 
- สามารถใช้กับ Public Key Cryptosystem ที่มี [[ECC Composite Property|Composite Property]] ได้
- วิธีการจะคล้ายกับ [[Type-2 BIP32 Hierarchical Deterministic Wallet]] ที่สามารถส้ราง private keys และ public keys แยกกันได้ 
- สามารถใช้ [[BIP32 Public Key Generation|Public Key Generation]] พร้อมกับ [[Hierarchical Tree of Keys|Hierarchical Tree Structure.]] โดยไม่ต้องกลัวว่าจะเกิดปัญหาแบบ  [[BIP32 Problems and Shortcomings]] เนื่องจากใน ระบบแบบ CPK จะต้องมี Key หลุดออกไปจำนวนมาก จึงจะสามารถเข้าถึงกระเป๋าตังค์ของเราได้

---
## See also
- [[CPK Algorithm]]
- [[CPK Security]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.
