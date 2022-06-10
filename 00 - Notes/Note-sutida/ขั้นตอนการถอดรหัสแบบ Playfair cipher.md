---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัสแบบ Playfair cipher
1. เราจะต้องทราบคีย์ที่จะใช้ในการเข้ารหัส
2. นำคีย์ใส่ตารางขนาด 5 x 5 เเล้วใส่ตัวอักษรภาษาอังกฤษที่ไม่ซ้ำกับคีย์จนครบ (ยกเว้น J หากเจอในข้อความธรรมดาให้ใช้ตัว I แทน)
3. นำรหัสที่ได้รับไปเทียบกับตาราง โดยให้มองเป็นสี่เหลี่ยมแล้วเลือกเอาตัวอักษรที่อยู่มุมสี่เหลี่ยมสองตัว เช่น รูปที่ 2
![[Playfair cipher-2.png|400]]
4. จากรูปที่ 2 ถอดรหัสได้เป็นคำว่า *IM FINE*
---
## See also
- [[Playfair cipher]]
- [[ขั้นตอนการเข้ารหัสแบบ Playfair cipher]]
## References
- [เก่ง จันทร์นวล,"เพลย์แฟร์ไซเฟอร,"](http://blog.bru.ac.th/wp-content/uploads/2020/09/flayfair.pdf)
- ["Substitution cipher,"](https://cryptography.fandom.com/wiki/Substitution_cipher#Polygraphic_substitution)
