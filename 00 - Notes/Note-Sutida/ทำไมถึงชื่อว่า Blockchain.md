---
version: "0.0.1"
cover_image:
published: "ture"
contributors: ["Sutida"]
---
uplinks:: [[Blockchain]]
tags:: #lang/th #type/statement

# ทำไมถึงชื่อว่า Blockchain
- Blockchain เกิดจากการรวมกันของคำ 2 คำ คือ Block  + chain หมายถึง 
 *"ห่วงโซ่เเห่งบล็อกที่เก็บข้อมูล"*  
 - *ตัวอย่าง* จากการทำงานของ Bitcoin ก็คือข้อมูลการทำธุรกรรมของเราจะถูกบันทึกไว้เป็นชุด ๆ อยู่ใน Block  ซึ่ง 1 ชุดเท่ากับ 1 Block (ใน 1 Block จะเก็บข้อมูลธุรกรรมได้หลายรายการ) แล้วใน 1 Block จะประกอบด้วย 3 ส่วน คือ
	 1. ข้อมูลที่ต้องการบันทึก เช่น Satoshi Nakamoto โอนเงินให้เรา 1000 BTC เป็นต้น
	 2. [[Hash Function]] ชุดตัวอักษรที่อ่านไม่ออก (ข้อมูล Block เปลี่ยน = Hash เปลี่ยน)
	 3. Hash ของ Block ก่อนหน้า เมื่อมีข้อมูลชุดใหม่เข้ามาจะถูกบันทึกไว้ใน Block ใหม่ ซึ่งใน Block จะมีข้อมูล Hash ของ Block เก่าไว้ด้วย ในส่วนนี้ก็จะทำให้ Block เชื่อมต่อกันเป็นสายโซ่ (Chain)
-  ข้อมูลธุรกรรมของ Block ก่อนหน้าจะถูก Cryptographic Hash (การเข้ารหัสทางเดียวเพื่อเช็กว่าเป็นข้อมูลต้นฉบับไม่มีใครเปลี่ยนเเปลง)
- หากมีคนแอบไปเปลี่ยนแปลงข้อมูลธุรกรรม Block เก่าแม้แต่เพียงนิดเดียว Hash ก็จะเปลี่ยนทำให้เรารู้ว่ามีการแอบแก้ไข

---
## References
- [''เทคโนโลยีบล็อกเชน มีข้อดีและข้อจำกัดอย่างไร?,"2564.](https://www.bitkub.com/blog/blockchain-142baeb2db28)
- [Wikipedia,"Blockchain,"2565.](https://th.wikipedia.org/wiki/%E0%B8%9A%E0%B8%A5%E0%B9%87%E0%B8%AD%E0%B8%81%E0%B9%80%E0%B8%8A%E0%B8%99)
- [iT24Hrs,''Blockchain คืออะไร บล็อกเชนทำอะไรได้บ้าง นอกจากแค่ cryptocurrency /bitcoin,2561.](https://youtu.be/2oaLjzx6tZY)

## See also
- [[Blockchain Trilemma]]