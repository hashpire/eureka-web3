---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Type of HD Wallet](./MOC Type of HD Wallet.md)
tags:: #lang/th #type/thing

# BIP32 Problems and Shortcomings
การใช้วิธีแบบ[BIP32 Normal Key Derivation](./BIP32 Normal Key Derivation.md)ไม่สามารถที่จะใช้[BIP32 Public Key Generation](./BIP32 Public Key Generation.md)และ[Hierarchical Tree of Keys](./Hierarchical Tree of Keys.md)พร้อมกันได้ เพราะหากมีในกรณีที่บุคคลอื่น รู้ Parent Public Key, Parent Chain Code หรือ Child Private Key  ของเรา จะสามารถคำนวณ Parent Private Key ออกมาและเข้าถึงเงินทั้งหมดของเราได้  จึงทำให้ต้องมีการใช้วิธีแบบ[BIP32 Hardened Key Derivation](./BIP32 Hardened Key Derivation.md)เข้ามาเพื่อป้องกันในกรณีดังกล่าว แต่การใช้วิธีแบบ Hardened จะทำให้เราสูญเสียคุณสมบัติในการทำ[BIP32 Public Key Generation](./BIP32 Public Key Generation.md)ไปด้วย

---
## See also
-[Type-2 BIP32 Hierarchical Deterministic Wallet](./Type-2 BIP32 Hierarchical Deterministic Wallet.md)
-[Deterministic Wallet](./Deterministic Wallet.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A deeper look into Hierarchical Deterministic Wallets.md)"2022.