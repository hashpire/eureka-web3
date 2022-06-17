---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC Cryptographic Primitives & Math]]
tags:: #lang/th #type/thing 

# Elliptic Curve (EC)
- *Elliptic Curve (EC)*  เป็นกราฟเส้นโค้งที่ถูกกำหนดด้วยสมการ Weierstrass  $y^2= x^3 + az+b$ และ [[Point at infinity O|Point at infinity ]] $O$ เมื่อค่าคงที่ $a$ และ $b$ มีค่าเท่ากับ $4a^3 + 27b^2 \neq 0$
    - สมการนี้ตั้งชื่อตามนักคณิตศาสตร์ Karl Weierstrass ซึ่งศึกษาและเผยเเพร่เกี่ยวกับ Elliptic Curve (EC) ในช่วงศตวรรษที่ 19
- คุณสมบัติหลักๆ ของ Elliptic Curve
	- กราฟแนวนอนจะสมมาตรกัน
	- ถ้าเราวาดเส้นตัดบนกราฟจะตัดกับกราฟเส้นโค้งมากที่สุดสามจุด
---
## See also
- [[Elliptic Curve Cryptography(TH)]]
- [[Elliptic Curve Arithmetic(TH)]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.