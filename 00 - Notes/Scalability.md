## version: "0.0.0"
uplinks:: [[Blockchain Trilemma คือ]]
tags:: [#type/note](app://obsidian.md/index.html#type/note) [#lang/th](app://obsidian.md/index.html#lang/th) [#people/Sutida](app://obsidian.md/index.html#people/Sutida)

# Scalability
ความสามารถขยายเครือข่าย หมายถึง เครือ Blockchain สามารถรองรับจำนวนผู้ใช้หรือธุรกรรมที่เพิ่มสูงขึ้นได้อย่างมีประสิทธิภาพ โดยไม่เกิด*ปัญหาคอขวด*เมื่อมีจำนวนผู้ใช้งานในเครือข่ายสูง


ตัวอย่างปัญหาและการแก้ปัญหา Scalability ของ Bitcoin 
ปัญหาคือการไม่สามารถทำธุรกรรมได้อย่างรวดเร็วเนื่องจากการใช้งานหรือการทำธุรกรรมจำนวนมาก ซึ่งเป็นเหตุมาจากการเติบโตของจำนวนผู้ใช้งานที่เพิ่มสูงขึ้น จึงเกิด *ภาวะคอขวดในการตรวจสอบธุรกรรม* เนื่องจาก Bitcoin สามารถรองรับธุรกรรมได้เพียง 7 ธุรกรรมต่อวินาที เเละในช่วงที่มีการทำธุรกรรมจำนวนค่าธรรมเนียมในการโอนจะสูงขึ้นอย่างมากเช่นกัน

**วิธีการแก้ปัญหาได้ถูกพูดถึงมาอย่างยาวนาน โดยมีการเสนอวิธีต่างๆหลายวิธี** ตัวอย่าง เช่น 

**Lightning Network (LN)** เป็นเทคโนโลยีเครือข่ายที่ออกแบบมาเพื่อแก้ไขปัญหาในความล่าช้าของ Blockchain ใน Bitcoin จากการประมวลผลธุรกรรมขนาดมหาศาล (Scalability Problem) โดยเป็นการทำธุรกรรมนอกเครือข่าย Blockchain หรือที่เรียกันว่า [[Off-Chain Scaling]] แล้วจึงค่อยนำผลลัพธ์ที่รวมกัน กลับเข้าสู่เครือข่ายหลักในภายหลัง
*หลักการทำงาน* คือ การสร้าง Channel ระหว่าง User ไปเรื่อยๆ โดยไม่ต้องแจ้ง Transaction ทีละ Transaction กับ Blockchain หลักแต่จะรวมหลายๆธุรกรรมมาแล้วแจ้งทีเดียว โดยจะนำเข้าสู่ Blockchain หลักเมื่อ User ปลายทางทั้งสองตกลงที่จะปิด Transaction Channel นี้ ซึ่งเมื่อปิดแล้วยอดคงเหลือใน wallet ของ User ล่าสุดจะถูกแจ้งไปยัง Blockchain หลักทีเดียวและยิ่งมี Channel มากขึ้นเท่าไหร่ก็จะทำให้ Transaction ใน Chain เร็วมากเท่านั้นซึ่งนี้ก็จะช่วยแก้ปัญหาเรื่อง Scalability

## References
- [รู้จัก Blockchain Trilemma กำแพง 3 ชั้นสู่ Mass Adoption](https://www.finnomena.com/bitkub/blockchain-trilemma/)
- [Scalability](https://www.blockdit.com/posts/61964330e8655f0d7e1cbc47)
## See Also