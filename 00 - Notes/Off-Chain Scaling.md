---
version: "0.0.0"
published: true
---
uplinks:: [[Ethereum Layer 2]] 
tags:: #type/note #lang/th #people/Sutida

# Off-Chain Scaling
Off-Chain Scaling คือ การสร้างโปรโตคอลทางเลือกแบ่งเเยกจาก Layer 1  Mainet  โดยไม่ต้องเปลี่ยนเเปลง โปรโตคอลของ Ethereum เเต่จะใช้เป็น Layer 2 Solution ในการเเก้ปัญหาแทนซึ่งจะได้รับความปลอดภัยจากเชนหลักอย่าง ETH, BTC 

การปรับขนาดเป็นเลเยอร์ได้รับการสนับสนุนโดย Gall's Law ซึ่งระบุว่า
*“ระบบซับซ้อนที่ใช้งานได้นั้นมักจะพบว่ามีวิวัฒนาการมาจากระบบธรรมดาที่ใช้งานได้จริง ระบบซับซ้อนที่ออกแบบมาตั้งแต่เริ่มต้นจะไม่ทำงานและไม่สามารถแก้ไขเพื่อให้ใช้งานได้”*

**ตัวอย่างของ Off-Chain Scaling เช่น**
- **Lightning Network ของ Bitcoin** เป็นโซลูชันการปรับขนาดนอกเครือข่ายที่โดดเด่นที่สุดในตลาด Lightning Network มีหลักการทำงานคือต้องใช้การรวบรวมธุรกรรมจากเชนหลักเพื่อจัดการกับ Off-Chain แล้วถ่ายโอนข้อมูลกลับไปที่  Lightning Network และยังมีการนำ Smart Contract มาสู่ Bitcoin ซึ่งเป็นการปรับปรุงครั้งใหญ่ของเครือข่ายโดยรวม
   *ข้อเสีย* ของ Lightning Network คือผู้ใช้งานจำเป็นต้องมีสภาพคล่องค่อนข้างสูงในการดำเนินการ หรืออาจจะกล่าวได้ว่าจะต้องมีการเก็บ Bitcoin ไว้ใน Lightning Network เพื่อสะดวกในการชำระเงิน อีกข้อที่ถือได้ว่าเป็นข้อเสียเเต่จะเป็นข้อเสียสำหรับรัฐบาลหรือหน่วยงานกลาง เพราะ  Lightning Network ให้ความเป็นส่วนตัวแก่ผู้ใช้มากขึ้นเมื่อพวกเขาทำธุรกรรมด้วย bitcoin นี่เป็นสิ่งที่ดีสำหรับบุคคลทั่วไป
   
- **State Channels** คือการทำหลายธุรกรรมแบบ Off-Chain เเต่จะส่งเพียง 2 ธุรกรรมที่เกี่ยวกับการชำระเงินค่าการดำเนินธุรกรรมไปยัง Ethereum ทำให้รองรับธุรกรรมได้มากและค่าดำเนินการน้อยลง 
   *ข้อเสีย* การใช้งานยังจำกัดอยู่ในวงเเคบ และผู้ใช้งานต้องรู้ล่วงหน้ารวมทั้งต้องฝากเงินเข้าใน Multisig Contract ซึ่งเครือข่ายต้องได้รับการตรวจสอบอย่างสม่ำเสมอเพื่อให้แน่ใจได้ว่าเงินที่ฝากเข้ามานั้นยังมีความปลอดภัยอยู่เสมอ

- **Off-Chain Scaling – Other-Chain Scaling (ยืนยันธุรกรรมบน Blockchain ใหม่ )**
	- **Sidechain** : เป็น Blockchain อิสระที่สามารถทำงานได้กับ EVM เป็นการทำงานแบบคู่ขนานกับ Mainnet ซึ่งเข้ากันได้ดีกับ Ethereum ผ่านการ Brigdges ข้ามระหว่าง 2 Chain โดยแต่ละ Sidechain นั้นก็จะมีข้อแตกต่างกันในแต่ละ sidechain 

## References
- [Blockchain scaling: on-chain vs off-chain](https://bdtechtalks.com/2019/09/16/blockchain-scaling-on-chain-vs-off-chain/)
- [BLOCKCHAIN SCALING SOLUTION](https://academy.bitcoinaddict.org/blockchain-scaling-solution/)

## See Also

