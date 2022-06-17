---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC HD Wallet]]
tags:: #lang/th #type/thing

# BIP32 Problems and Shortcomings
การใช้วิธีแบบ [[BIP32 Normal Key Derivation]] ไม่สามารถที่จะใช้ [[BIP32 Public Key Generation]] และ [[Hierarchical Tree of Keys]] พร้อมกันได้ เพราะหากมีกรณีที่บุคคลอื่นรู้ Parent Public Key, Parent Chain Code หรือ Child Private Key ของเรา จะสามารถคำนวณ Parent Private Key ออกมาและเข้าถึงเงินทั้งหมดของเราได้ จึงทำให้ต้องมีการใช้วิธีแบบ [[BIP32 Hardened Key Derivation]] เข้ามาเพื่อป้องกันในกรณีดังกล่าว แต่การใช้วิธีแบบ Hardened จะทำให้เราสูญเสียคุณสมบัติในการทำ [[BIP32 Public Key Generation]] ไปด้วย

---
## See also
- [[Type-2 BIP32 Hierarchical Deterministic Wallet]]
- [[Deterministic Wallet]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.
