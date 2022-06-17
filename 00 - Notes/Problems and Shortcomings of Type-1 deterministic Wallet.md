---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::  [MOC HD Wallet](./MOC%20HD%20Wallet)
tags:: #lang/th #type/thing

# Problems and Shortcomings of Type-1 deterministic Wallet
- ยังไม่สามารถแก้ปัญหาเรื่องการแชร์กระเป๋าตังค์ [[Blockchain Wallets|(Blockchain Wallets)]] ได้ เนื่องจาก ข้อมูลทั้งหมดของกระเป๋าตังค์เราจะอยู่ใน Seed หากเราแชร์ Seed ให้บุคคลอื่น หมายความว่าบุคคลอื่นสามารถเข้าถึงกระเป๋าตังค์ของเราได้ทั้งหมด แต่หากเราไม่แชร์ Seed เท่ากับว่าเราไม่สามารถแชร์อะไรได้เลย
- ปัญหาด้านความปลอดภัย หากในกรณีที่เราเปิดร้านค้าออนไลน์ แล้วต้องนำ Seed ของเราไปไว้บน Web Server เพื่อใช้ในการรับเงิน ถ้า Web Server ของเราโดนแฮก หมายความว่า เราจะสูญเสียเงินทั้งหมดที่อยู่ในกระเป๋าตังค์ของไป

---
## See also
- [[Type-1 Deterministic Wallet]]
- [[Deterministic Wallet]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.
