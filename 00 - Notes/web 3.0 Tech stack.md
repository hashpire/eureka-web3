---
version: "0.0.0"
---
uplinks:: [[Internet คืออะไร]]
tags:: #type/article #lang/th #people/sutida 
# web 3.0 Technology stack
![[web3 tech stack.jpg]]
   ***Layer 0*** เป็นส่วนพื้นฐานของ Stack ของ Web 3.0 ที่ประกอบไปด้วยวิธีการสื่อสารของหน่วยสื่อสาร (Node) ต่าง ๆ และวิธีการติดตั้งโปรแกรมในระดับล่างที่สุด (Lowest Level)
	- (1) Peer-to-peer (p2p) internet overlay protocols หมายถึง protocols  ที่อธิบายวิธีการสื่อสารของ  node ในระบบ P2P 
	- (2) Platform-neutral computation description language หมายถึงภาษาที่ใช้อธิบายการทำงานของ  node ในระดับต่ำที่สุด

-   ***Layer 1*** เป็นส่วนที่ทำหน้าทั้งในส่วนของการจัดเก็บ, แจกจ่าย และการโต้ตอบข้อมูลระหว่าง Node ด้วยกัน ที่อาจจะยังไม่มีความปลอดภัยมากพอ
	- (3)Data distribution protocols เป็น protocols  ที่ฮธิบายวิธีการเเจกจ่าย จัดเก็บและสื่อสารข้อมูล ระหว่ง  node ต่าง ๆในระบบ
	- (4) Zero/low-trust interaction platforms (shared security)  เป็น platforms ที่ใช้  Zero/low-trust interaction protocols  เพื่อให้ผู้มีส่วนร่วมซึ่งอาจจะไม่รู้จักกันสามารถแชร์ความปลอดภัยซึ่งกันเเละกันได้
	- (5) Zero/low-trust interaction protocols เป็น protocols ที่อธิบายวิธีการที่ทำให้ node ที่ไม่รู้จักกันสามารถมีปฏิสัมพันธ์ซึ่งกันและเชื่อถือผลการคำนวณและข้อมูลของกันเเละกัน
	- (6) Transient data pub/sub messaging เป็น protocols ที่อธิบายถึงวิธีการสื่อสารข้อมูลที่ไม่ต้องการจะจัดเก้บเเบบถาวร เช่น การอัปเดตสถานะและวิธีการที่ทำให่้ node รับรู้การมีอยู่ของข้อมูลที่ต้องสื่อสาร
	
-  ***Layer 2*** เป็นส่วนที่ทำหน้าที่ในการสนับสนุนขั้นที่ 1 ด้วยการเพิ่มความสามารถฟังก์ชันต่าง ๆ อย่างเช่น การจัดเก็บข้อมูลแบบเข้ารหัส (Encrypted Messaging) และ การเชื่อมโยงคอมพิวเตอร์หลายเครื่องเข้าด้วยกันบนเครือข่ายเข้าเป็นกลุ่ม เพื่อแบ่งปันข้อมูลและร่วมกันประมวลผล (Distributed Computing)
	- 7.1 State channels เป็นวิธีการจัด Blockchain มีการเปิด-ปิด channel โดยให้ node สื่อสารกันเเบบ off-chain จะไม่บันทึกทุกการเปลี่ยนแปลงสถานะบน main chain 
	- 7.2 Plasma protocols การย้ายธุรกรรมจาก on-chain ไป off-chain มีการสร้าง tree of Blockchain
	- 7.3 Encrypted Storage การจัดเก็บข้อมูลเเบบเข้ารหัส
	- 7.4 Storage incentivisation 
	- 7.5 Heavy computation วิธีการที่ช่วยทำให้ การคำนวณกันบนคอมพิวเตอร์หลายเครื่องเเละการพิสูนจ์ว่าการคำนวณดำเนินไปอย่างถูกต้อง
	- 7.6 Distributed secret management การจัดเก็บความลับต่าง ๆพวก private key เพื่อให้ข้อมูลสามารถเข้าถึงได้เฉพาะคนที่ได้รับอนุญาตเท่านั้น
	- 7.7 Oracles เป็นตัวทำหน้าที่นำเข้าข้อมูลจาก off-chain เข้าสู่ Blockchain
-   ***Layer 3*** เป็นส่วนเกี่ยวกับภาษาโปรแกรมมิง และ Libraries ซึ่งเป็นที่รวบรวมชุดฟังก์ชันต่าง ๆ เพื่อสำหรับให้นักพัฒนาเข้ามาใช้พัฒนาแอปพลิเคชันต่าง ๆ ได้อย่างเหมาะสม

-   ***Layer 4*** เป็นส่วนบนสุดของ Stack ที่ได้รวบรวมโปรแกรมที่ผู้ใช้งานทั่วไป ที่ไม่ใช่นักพัฒนาเข้ามาใช้งานโดยตรงกับ Blockchain ได้ หรือเรียกง่าย ๆ ก็คือโปรแกรมที่ใช้เข้าอินเทอร์เน็ตที่ทุกคนกำลังอ่านบทความนี้นั่นเอง

## References
- [พาไปรู้จักกับ ‘Web 3.0’](https://www.beartai.com/article/tech-article/914953)
- [WEB 3.0 คืออะไร?](https://www.finnomena.com/zipmex/what-is-web-3-0/)

## See Also