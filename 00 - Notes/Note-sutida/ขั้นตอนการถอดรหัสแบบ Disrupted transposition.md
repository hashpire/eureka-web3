---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/concept

# ขั้นตอนการถอดรหัสแบบ Disrupted transposition
1. เราต้องทราบ คีย์ปกติและ Disrupted Key ที่ใช้ในการเข้ารหัส 
2. นำคีย์ปกติใส่บนหัวตาราง จากนั้นทำการหาตำแหน่งการเว้นช่องว่างจากลำดับตัวอักษรใน Disrupted Key  ในตัวอย่าง ดังรูปที่ 2 เป็นคำว่า *SECRET*  เรียงตามลำดับตัวอักษร จะได้ S=5 , E=2, C=1, R=4, E=3, T=6 
![[Disrupted transposition-2.png|250]]
3. นำรหัสที่ได้รับมาใส่ลงในตาราง โดยเรียงตามลำดับตัวอักษรในคีย์ปกติจากบนลงล่าง จนครบ ดังรูปที่ 3 
![[Disrupted transposition-3.png|500]]
4. ถอดรหัสข้อความจากรูปที่ 3 เรียงจากซ้ายไปขวา จะได้ *WE ARE DISCOVERED, FLEE AT ONCE*
---
## See also
- [[Disrupted transposition]]
- [[ขั้นตอนการเข้ารหัสแบบ Disrupted transposition]]
## References