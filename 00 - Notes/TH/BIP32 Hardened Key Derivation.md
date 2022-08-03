---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Type of HD Wallet](./MOC%20Type%20of%20HD%20Wallet.md)
tags:: #lang/th #type/thing

# BIP32 Hardened Key Derivation
*BIP32 Hardened Key Derivation* คือ การสร้าง Child Private Key วิธีการจะคล้ายกับการสร้าง Child Private Key ใน[BIP32 Normal Key Derivation](./BIP32%20Normal%20Key%20Derivation.md)โดยนำ Parent Private Key, Parent Chain Code, Index ไปเข้า[Hash Function](./Hash%20Function.md)แบบ HMAC-SHA512 แต่จะแตกต่างตรงที่ จะใช้ Parent Private Key แทนการใช้ Parent Public Key 
- หลักการแบบ Hardened มีความปลอดภัยกว่าแบบ Normal  ตรงที่เราไม่สามารถใช้ Parent Public Key ในการสร้าง Child Public Key ได้ เนื่องจากว่าจะต้องใช้ Parent Private Key เท่านั้นในการสร้าง ค่า IL 

---

## See also
-[Type-2 BIP32 Hierarchical Deterministic Wallet](./Type-2%20BIP32%20Hierarchical%20Deterministic%20Wallet.md)

## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A%20deeper%20look%20into%20Hierarchical%20Deterministic%20Wallets.md)"2022.
