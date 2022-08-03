---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Blockchain Keys and Addresses](./MOC Blockchain Keys and Addresses.md)
tags:: #lang/th #type/thing

# ECC Composite Property
- *ECC Composite Property* เป็นคุณสมบัติหนึ่งของ[Elliptic Curve (EC)](./Elliptic Curve (EC).md)คือ เราสามารถสร้าง  $Public Key_C$ ได้โดยไม่จำเป็นต้องสร้างผ่าน $Private Key_C$ แต่สร้างผ่าน $Public Key_A + Public Key_B$  ได้เลย นอกจากนี้ เรายังสามารถสร้าง $Private Key_C$ จากการนำ $Private Key_A + Private Key_B (mod n)$ ได้อีกด้วย ซึ่งค่า $n$ เป็นค่าคงที่ ที่มีความสัมพันธ์กับค่า $G$ ที่เป็น [Public Key|ค่า base point บน Elliptic Curve (EC)](./Public Key|ค่า base point บน Elliptic Curve (EC).md)
- การสร้าง $Public Key$ อื่นๆ 
	- $Private Key_A \cdot G > Public Key_A$
	- $Private Key_B \cdot G > Public Key_B$
	- $Private Key_C \cdot G > Public Key_C$

---
## See also
-[Private Key](./Private Key.md)
-[Public Key](./Public Key.md)
-[Address](./Address.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A deeper look into Hierarchical Deterministic Wallets.md)"2022.