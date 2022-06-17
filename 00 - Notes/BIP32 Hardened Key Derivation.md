---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC HD Wallet]]
tags:: #lang/th #type/thing

# BIP32 Hardened Key Derivation
*BIP32 Hardened Key Derivation* คือ การสร้าง Child Private Key วิธีการจะคล้ายกับการสร้าง Child Private Key ใน [[BIP32 Normal Key Derivation]] โดยนำ Parent Private Key, Parent Chain Code, Index ไปเข้า [[Hash Function]] แบบ HMAC-SHA512 แต่จะแตกต่างตรงที่ จะใช้ Parent Private Key แทนการใช้ Parent Public Key 
- หลักการแบบ Hardened มีความปลอดภัยกว่าแบบ Normal  ตรงที่เราไม่สามารถใช้ Parent Public Key ในการสร้าง Child Public Key ได้ เนื่องจากว่าจะต้องใช้ Parent Private Key เท่านั้นในการสร้าง ค่า IL 

---

## See also
- [[Type-2 BIP32 Hierarchical Deterministic Wallet]]

## References
- [[A deeper look into Hierarchical Deterministic Wallets|Anakorn Kyavatanakij,"A deeper look into Hierarchical Deterministic Wallets,"2022.]]
