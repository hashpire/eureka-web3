---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Type of HD Wallet](./MOC%20Type%20of%20HD%20Wallet.md)
tags:: #lang/th #type/thing

# BIP32 Normal Key Derivation
 *BIP32 Normal Key Derivation* คือ การสร้าง Child Private Key และ[BIP32 Public Key Generation|Child Public Key ](./BIP32 Public Key Generation|Child Public Key .md)
 
 - การสร้าง Child Private Key  โดยนำ
    - Parent Public Key, Parent Chain Code,  Index  ไปเข้า[Hash Function](./Hash%20Function.md)แบบ HMAC-SHA512 จะได้ Output แบ่งออกเป็น 
	    - ด้านซ้าย 256 Bit (IL) ทำการนำ Parent Private Key และ IL ไปเข้าฟังก์ชั่น  Modular Addition  จะได้เป็น Child Private Key 
	    - ด้านขวา 256 Bit (IR) โดยจะเรียกส่วนนี้ว่าเป็น Child Chain Code 
	    -  Child Private Key + Child Chain Code  รวมกันเป็น Extended Private Key
	
> - Parent Public Key ได้มาจากการนำ Parent Private Key (คือ Master Private Key จากใน[Type-2 BIP32 Hierarchical Deterministic Wallet](./Type-2%20BIP32%20Hierarchical%20Deterministic%20Wallet.md)) นำไปคูณกับค่า G
> - Parent Chain Code (คือ Master Chain Code จากใน[Type-2 BIP32 Hierarchical Deterministic Wallet](./Type-2%20BIP32%20Hierarchical%20Deterministic%20Wallet.md))
> -  Index ค่าที่บอกว่าเราจะสร้าง Key ตัวใด

---
## See also
-[BIP32 Hardened Key Derivation](./BIP32%20Hardened%20Key%20Derivation.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A%20deeper%20look%20into%20Hierarchical%20Deterministic%20Wallets.md)"2022.