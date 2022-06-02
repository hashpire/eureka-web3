---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/term 

# Polygraphic substitution cipher
- *Polygraphic substitution cipher* คือการเข้ารหัสโดยการเเทนที่ข้อความธรรมดาเป็นคู่ตัวอักษรแบบไม่คงที่ เช่น เเทนที่ AN ด้วย QX เป็นต้น 
- การเเทนแบบ Polygraphic substitution cipher จะใช้ตัวอักษรทดแทน 676 (26^2=676) แบบเหมือนกับในหนังสือการเข้ารหัสลับ _De Furtivis Literarum Notis_ เขียนโดย della Porta
- ตัวอย่างการเเทนที่ เช่น คำว่า *AN ANT AT STATS* 
	1. จะจัดตัวอักษรให้คู่กัน ได้เป็น *AN AN TA TS TA TS* 
	2. เเทนที่ตัวอักษรโดยสมมุติให้ AN เเทนด้วย QZ , TA แทนด้วย WS, TS แทนด้วย ED 
	3. เมื่อเเทนที่ตามรูปแบบที่กำหนดไว้ในข้อที่ 3 จะเข้ารหัสได้เป็น *QZ QZ WS ED WS ED* 
	4. ข้อสังเกต จะเห็นได้ว่า *A* แต่ละตัวเเทนที่ด้วยตัวอักษรเเตกต่างกันไป ขึ้นอยู่กับว่ามันอยู่คู่กับตัวอะไร

---
## See also
- [[Polyalphabetic substitution cipher]]
- [[Monoalphabetic substitution cipher]]
## References
- [Wikipedia,"Polygraphic substitution,"2022.](https://en.wikipedia.org/wiki/Polygraphic_substitution)
