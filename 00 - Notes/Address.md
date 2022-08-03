---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]

---
uplinks::[MOC Blockchain Keys and Addresses](./MOC Blockchain Keys and Addresses.md)
tags:: #lang/th #type/thing 

# Address
- *Address: H(dG)* เปรียบเทียบได้กับเลขสมุดบัญชี ที่เราส่งให้กับบุคคลอื่น เวลาที่มีการทำธุรกรรมร่วมกัน
- Address สร้างได้จากการนำ จุด $dG$ ที่ได้จากการทำ[Public Key](./Public Key.md)าใส่[Hash Function](./Hash Function.md)และเนื่องจากตัว Public Key นั้นมีความยาวมาก จึงต้องนำมา Encoded ค่า ให้ออกมาในรูปแบบที่สามารถอ่านได้  อย่างใน[Bitcoin](./Bitcoin.md)ะใช้ Hash Function SHA-256 ที่ใช้ชุดตัวอักษร base 58 ขนาดความยาว 33-34 Bytes  ซึ่ง base 58 จะตัดตัวอักษรที่ซ้ำกัน คือ 0:เลขศูนย์, O:ตัวโอพิมพ์ใหญ่, I: ตัวไอพิมพ์ใหญ่, l: ตัวแอลพิมพ์เล็กออก เพราะบางตัวอักษรที่คล้ายกันมาก อาจจะทำให้แยกได้ยากและเกิดใช้งานผิดพลาดได้
- ตัวอย่าง Address เช่น  bc1qk3uzwdhkq39z2g2vqedk k42n6e27koaeecg4gd

---
## See also
-[Private Key](./Private Key.md)
## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A deeper look into Hierarchical Deterministic Wallets.md)"2022.