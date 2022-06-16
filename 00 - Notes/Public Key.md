---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [MOC Blockchain Keys and Addresses](./MOC%20Blockchain%20Keys%20and%20Addresses)
tags:: #lang/th #type/thing 

# Public Key
- *Public Key: (dG)*  สร้างได้จากการนำเอา [Private Key](./Private%20Key)  (d) ที่เราคำนวณออกมาไปทำ Point Scalar Multiplication  โดยการคูณกับค่า G ซึ่งเป็นค่า base point บน [Elliptic Curve (EC)](./Elliptic%20Curve%20(EC)) ที่ถูกกำหนดค่ามาแล้ว เช่น [Bitcoin](./Bitcoin) จะมีค่า G คือ $secp256k1: y^2= x^3 + 7$ จากนั้นนำค่า G ที่ได้มาทำการบวกกันตามจำนวนครั้งที่ได้จากค่า d เช่น d=2022 จะได้ dG=2022G 
- Public Key มีความปลอดภัยสูงมาก เนื่องจากค่าที่ได้มาจะไม่มีโอกาสซ้ำกันได้ เพราะ Private Key ที่ใช้ไม่ซ้ำกัน และนอกจากนั้น คือ เราไม่สามารถทำการหาค่า d ออกมาได้ แม้ว่าเราจะทราบ จุด G และ dG ก็ตาม 
- Public Key จะมีขนาดความยาวที่ 65 Bytes

---
## See also
- [Address](./Address)
## References