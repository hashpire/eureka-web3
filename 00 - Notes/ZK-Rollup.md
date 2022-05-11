---
version: "0.0.0"
published: true
---
uplinks:: [[Ethereum Layer 2]] 
tags::#type/note #lang/th #people/Sutida

# ZK-Rollup
- ZK-Rollup หรือ Zero Knowledge Rollup คือ  Blockchain ที่เป็น Layer 2 
- ทำงานร่วมกันกับ Ethereum Chain หลัก *(On-chain)*
- ภายใน ZK-Rollup จะไม่สามารถนำแพลตฟอร์มหรือ DApps ที่รันอยู่บน Ethereum Chain มาใช้งานภายใน Blockchain นี้ได้ *(ใช้ EVM ไม่ได้)*
- *การบันทึกธุรกรรมของ ZK-Rollup เหมือนกับ Optimistic Rollup* เป็นการรวมธุรกรรมไว้เยอะ ๆ มัดรวมกันไว้เเล้วส่งไปบันทึกลงในเครือข่าย Etherem Chain หลัก ทำให้สามารถลดจำนวนธุรกรรมในระบบ ลดค่าธรรมเนียมได้ 
- ZK-Rollup ขึ้นชื่อว่า *Zero Knowledge* ที่แปลความรู้ศูนย์รวม มีความหมายตรงตัวเลยว่า Validator Node ที่มีหน้าที่คอยตรวจสอบธุรกรรมของ Ethereum ไม่จำเป็นต้องบันทึกข้อมูลหรือตรวจสอบข้อมูลทุกอย่างที่มาจาก - ZK-Rollup ทำให้เครือข่ายสามารถลดการประมวลผลข้อมูลภายใน Blockchain ได้ ลดระยะเวลาการตรวจสอบข้อมูล ทำให้เพิ่มประสิทธิภาพ และเพิ่มความเร็วในการรทำธุรกรรมได้นั่นเอง
- Vitalik Buterin กล่าวไว้ว่า ZK-Rollup ถือว่าเป็น Layer 2 ที่มีประสิทธิภาพมากที่สุดในอนาคต ถ้าการอัพเกรด Ethereum 2.0  เสร็จสิ้น จะมีแค่ Ethereum Layer 2 บางตัวที่ได้ไปต่อและมีประสิทธิภาพที่ดีเยี่ยม นั่นก็คือ ZK-Rollup
- *ตัวอย่าง* ZK-Rollup ที่ถูกใช้งานในปัจจุบัน (ข้อมูลจากเว็บไซต์ L2beat) เช่น dYdX (DEXs), Loopring (Payments & DEXs) เป็นต้น

## References
- [ETHEREUM LAYER 2](https://academy.bitcoinaddict.org/what-is-ethereum-layer-2/)
-  [Ethereum LAYER 2 SCALING Explained](https://www.youtube.com/watch?v=BgCgauWVTs0&t=455s)
## See Also
- [[Off-Chain Scaling]]
- [[DApps]]
- [[Ethereum Layer 2]]
