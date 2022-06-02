---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Substitution ciphers-MOC]]
tags:: #lang/th #type/term 

# Caesar cipher
- *Caesar cipher* หรือ *รหัสซีซาร์*  เป็นการเขารหัสแบบ Secret Key หรือ Symmetric Key Cryptography คิดค้นโดยกษัตริย์ Julius Caesar
- จุดประสงค์ของรหัสซีซาร์คือ ใช้สื่อสารกับทหารในกองทัพและป้องกันไม่ให้ข่าวสารรั่วไหลไปถึงศัตรู
- การเข้ารหัสเเบบซีซาร์ตัวอักษรจะถูกแทนที่ด้วยตัวอักษรตัวที่ 3 นับจากตัวมัน เช่น A จะเเทนด้วย D , B จะเเทนด้วย E , C จะเเทนด้วย F , X จะเเทนด้วย A , Y จะเเทนด้วย B และ Z จะเเทนด้วย C เป็นต้น ดังรูปที่ 1 
![[caesar-cipher-left-shift-of-3-1.png|300]]
- การเข้ารหัสแบบ  Caesar cipher เราสามารถใช้หลักการทางคณิตศาสตร์ในการเข้าและถอดรหัสได้ โดยการเเปลงตัวอักษรเป็นตัวเลขก่อน ตามรูปแบบ A=0, B=1, C=2, X=24, Y=25, Z=26 เป็นต้น จากนั้นทำตามสูตรดังรูปที่ 2 
![[caesar-cipher-2.png|300]]
- โดย X มาจากตำแหน่งของตัวอักษรและ  n มาจากตำแหน่งของการเลื่อน เช่น เป็นการเลื่อนซ้าย 3 ตำแหน่ง คือ n=3 เป็นต้น ในการคำนวณหากผลบวกหรือลบออกมาเกิน mod26 เราจะต้องนำเอาเลขที่ได้มาลบกับ 26 ก่อนจึงจะได้คำตอบออกมา
---
## See also

## References
- [Wikipedia,"Caesar Cipher,"2022.](https://en.wikipedia.org/wiki/Caesar_cipher)
- ["Shift (Caesar) Ciphers,"](https://math.asu.edu/sites/default/files/shift.pdf)
- ["Caesar Cipher in Python,"](https://w3cschoool.com/caesar-cipher-in-python)