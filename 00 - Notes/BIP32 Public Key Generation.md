---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC HD Wallet]]
tags:: #lang/th #type/thing

# BIP32 Public Key Generation
*BIP32 Public Key Generation* ใน [[BIP32 Normal Key Derivation]] มีคุณสมบัติอีกอย่างหนึ่งก็คือ สามารถใช้ Parent Public Key ในการสร้าง  Child Public Key ได้เลยโดย 

- การสร้าง Child Public Key วิธีการเหมือนกับการทำ Child Private Key แต่จะแตกต่างกันตรงที่ ในขั้นแรกไม่ได้ใช้  Parent Private Key ไปคูณกับค่า G มาก่อน แต่ใช้ Parent Public Key โดยตรง และในขั้นตอนสุดท้าย ด้านซ้ายจะนำ Parent Public Key และ 256 Bit (IL)  ไปเข้าฟังก์ชัน Point Addition จะได้เป็น Child Public Key  ซึ่งในกรณีนี้กระเป๋าตังค์ที่เราสร้างขึ้นมาจะสามารถรับเงินได้อย่างเดียว แต่ไม่สามารถโอนเงินออกได้ 
- Child Public Key + Child Chain Code รวมกันเป็น Extended Public Key
- ตัวอย่างการนำไปใช้งานและข้อดี  
   - สามารถนำ Parent Public Key ไปวางบน Web Server ได้ โดยไม่ต้องกังวลว่าหาก Web Server โดนแฮกแล้วเราจะสูญเสียเงินทั้งหมด เพราะว่าบนเว็บของเรามีแค่  Parent Public Key ที่บอกเพียงแค่จำนวนเงินที่เรามีอยู่ แต่ไม่มี Parent Private Key ที่จะทำให้บุคคลอื่นสามารถเข้าถึงเงินของเราได้
   - กรณีการใช้งานในองค์กร สามารถนำ Parent Public Key ให้กับบริษัทที่เรามีการทำธุรกรรมร่วมกันไว้ได้เลย ทำให้อีกบริษัทสามารถที่จะสร้าง Child Public Key แล้วโอนเงินให้เราได้เลย
   - สามารถส่ง Master Public Key ให้กับบริษัทที่เข้ามาตรวจสอบบัญชีได้เลย เพราะจะแสดงจำนวนเงินทั้งหมดที่เรามีอยู่ในนั้น  

---
## See also
- [[Type-2 BIP32 Hierarchical Deterministic Wallet]]
- [[Deterministic Wallet]]
- [[BIP32 Hardened Key Derivation]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.
