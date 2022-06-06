---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Transposition cipher-MOC]]
tags:: #lang/th #type/term 

# Disrupted transposition
- *Disrupted transposition* เป็นการเข้ารหัสโดยการย้ายคอลัมน์ที่มีความซับซ้อนมาก เนื่องจากจะมีการกำหนดคีย์ในการเข้ารหัส 2 ตัว คือคีย์ที่ใช้ในการเข้ารหัสและ Disrupted key ที่ใช้ในการกำหนดช่องว่าง
- คีย์ปกติจะใช้ในการกำหนดคอลัมน์และแถวของการเข้ารหัส เช่นคำว่า *CRYPTO* เรียงลำดับตัวอักษร จะได้ C=1, R=4, Y=6, P=3, T=5, O=2
- Disrupted key จะใช้ในการกำหนดช่องว่างของตาราง โดยกำหนดจากลำดับตัวอักษรในคีย์นั้น ๆ เช่นคำว่า *SECRET* เรียงตามลำดับตัวอักษร จะได้ S=5 , E=2, C=1, R=4, E=3, T=6 ตัวอย่างดังรูปที่ 1 
![[Disrupted transposition.png|400]]
- จากรูปที่ 1 เราจะเข้ารหัสโดยการเรียงตามลำดับตัวอักษรของคีย์ปกติ จะได้เป็น *WCEEO ERETR IVFCE ODNSE LEADA* 
---
## See also
## References
- [Wikipedia,"Disrupted Transposition,"2022.](https://en.wikipedia.org/wiki/Transposition_cipher#Disrupted_transposition)
