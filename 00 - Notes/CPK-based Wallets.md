---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Type of HD Wallet](./MOC%20Type%20of%20HD%20Wallet.md)
tags:: #lang/th #type/thing

# CPK-based Wallets
*CPK (Combined Public Key)* เป็นอัลกอรึทึม ในการทำ identity-based large-scale key management  คิดค้นและเผยแพร่ โดย Nan Xianghao นักวิชาการชาวจีน ในปี 1999 
- สามารถใช้กับ Public Key Cryptosystem ที่มี[ECC Composite Property|Composite Property](./ECC%20Composite%20Property|Composite%20Property.md)ได้
- วิธีการจะคล้ายกับ[Type-2 BIP32 Hierarchical Deterministic Wallet](./Type-2%20BIP32%20Hierarchical%20Deterministic%20Wallet.md)ที่สามารถส้ราง private keys และ public keys แยกกันได้ 
- สามารถใช้[BIP32 Public Key Generation|Public Key Generation](./BIP32%20Public%20Key%20Generation|Public%20Key%20Generation.md)พร้อมกับ[Hierarchical Tree of Keys|Hierarchical Tree Structure.](./Hierarchical%20Tree%20of%20Keys|Hierarchical%20Tree%20Structure..md)โดยไม่ต้องกลัวว่าจะเกิดปัญหาแบบ [BIP32 Problems and Shortcomings](./BIP32%20Problems%20and%20Shortcomings.md)เนื่องจากใน ระบบแบบ CPK จะต้องมี Key หลุดออกไปจำนวนมาก จึงจะสามารถเข้าถึงกระเป๋าตังค์ของเราได้

---
## See also
-[CPK Algorithm](./CPK%20Algorithm.md)
-[CPK Security](./CPK%20Security.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A%20deeper%20look%20into%20Hierarchical%20Deterministic%20Wallets.md)"2022.
