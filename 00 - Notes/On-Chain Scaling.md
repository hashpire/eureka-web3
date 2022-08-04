---
version: "0.0.0"
published: true
---
uplinks:: [[Ethereum Layer 2]] 
tags:: #type/note #lang/th #people/Sutida
> **Scaling Solution คือ?**
> คือวิธีการเเก้ปัญหาที่เกิดจากจำนวนผู้ใช้งานที่เพิ่มมากขึ้นของ Bitcoin & Ethereum ที่ทำให้ความสามารถในการรองรับการทำธุรกรรมไม่เพียงพอกับผู้ใช้งานจึงเกิดความล่าช้าและค่าธรรมเนียม (Gas) แพงขึ้น
> โดยประเภทของ Scaling Solution นั้นสามารถแบ่งออกได้เป็น 2 ประเภทคือ **On-Chain scaling** และ  **Off-chain Scaling**

# On-Chain Scaling
On-Chain Scaling ใช้วิธีในการปรับขนาดเพื่อรองรับการทำธุรกรรมโดยเป็นการเปลี่ยนเเปลงบน Layer 1 ใน Peer-to-Peer (P2P) Layer โดยการลดขนาดธุรกรรมและข้อความ เป็นต้น 

**ตัวอย่างของ On-Chain Scaling เช่น** 
**Segregated Witness (SegWit)** คือ การเปลี่ยนแปลงการทำธุรกรรม Bitcoin ที่แยกธุรกรรมและสคริปต์ (witness data) ออกจากข้อมูลรับเข้าและการส่งออก วัตถุประสงค์ของมันคือการแก้ปัญหาในการทำธุรกรรมโดยไม่ได้ตั้งใจ และเป็นแนวทางสำหรับการปรับขนาด Layer 2 Bitcoin scaling 

การปรับปรุงความสามารถในการปรับขนาดให้กับเลเยอร์พื้นฐานของบล็อคเชนที่มีอยู่นั้นยังไม่สามารถบรรลุระดับความสามารถในการรองรับผู้ใช้งานจำนวนมากได้แม้ว่า Bitcoin จะปรับปรุงความสามารถในการปรับขนาดในขั้นฐานได้ถึง 10 เท่าแต่ก็ยังไม่สามารถตอบสนองความต้องการ การชำระเงินของเศรษฐกิจโลกได้ นี่คือเหตุผลที่ Bitcoin มุ่งเน้นไปที่ "การปรับขนาดนอกเครือข่าย [[Off-Chain Scaling]]" 

อีกวิธีหนึ่งในการปรับปรุงการปรับขนาดแบบ On-Chain ไปอย่างสิ้นเชิงคือการสร้างเครือข่ายใหม่ที่มีกลไกฉันทามติใหม่ที่จัดลำดับความสำคัญของการปรับขนาดแทนคุณลักษณะที่อาจต้องการอื่นๆ ตามหลักการแล้ว วิธีนี้จะทำให้การทำธุรกรรมแบบ On-Chain สามารถใช้ได้กับคนทั่วไป ซึ่งหมายถึงการค้นหาทางเลือกอื่นแทนกลไกฉันทามติที่มีอยู่ เช่น [[Proof of Work (PoW)]], [[Proof of Stake (PoS)]] หรือ Delegated Proof of Stake (EOS)

## References
- [Blockchain scaling: on-chain vs off-chain](https://bdtechtalks.com/2019/09/16/blockchain-scaling-on-chain-vs-off-chain/)
- [BLOCKCHAIN SCALING SOLUTION](https://academy.bitcoinaddict.org/blockchain-scaling-solution/)

## See Also