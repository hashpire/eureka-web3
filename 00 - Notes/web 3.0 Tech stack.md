---
version: "0.0.0"
published: true
---
uplinks:: [[Web 3.0]]
tags:: #type/article #lang/th #people/sutida 
# Web 3.0 Technology Stack
![[web3 tech stack.jpg]]
- **Layer 0** เป็นส่วนพื้นฐานของ Stack ของ Web 3.0 ที่ประกอบไปด้วยวิธีการสื่อสารของหน่วยสื่อสาร (Node) ต่าง ๆ และวิธีการติดตั้งโปรแกรมในระดับล่างที่สุด (Lowest Level)
	- *(1 ) Peer-to-Peer (P2P) internet overlay protocols*  หมายถึง Protocols ที่อธิบายวิธีการสื่อสารของ Node ในระบบ P2P เช่น Devp2p, Libp2p
	- *(2) Platform-neutral computation description language* หมายถึงภาษาที่ใช้อธิบายการทำงานของ Node ในระดับต่ำที่สุด เช่น EVM, WASM, UTXO

- **Layer 1** เป็นส่วนที่ทำหน้าที่ในส่วนของการจัดเก็บ, แจกจ่ายและการโต้ตอบข้อมูลระหว่าง Node ด้วยกัน ที่อาจจะยังไม่มีความปลอดภัยมากพอ
    -   _(3)Data distribution protocols_ เป็น Protocols ที่อธิบายวิธีการเเจกจ่าย จัดเก็บและสื่อสารข้อมูลระหว่าง Node ต่าง ๆ ในระบบ เช่น IPFS, Bluzelle, Fluence
    -   _(4) Zero/low-trust interaction platforms (shared security)_ เป็น Platforms ที่ใช้ Zero/low-trust interaction protocols เพื่อให้ผู้มีส่วนร่วมซึ่งอาจจะไม่รู้จักกันสามารถแชร์ความปลอดภัยซึ่งกันเเละกันได้ เช่น Polkadot
    -   _(5) Zero/low-trust interaction protocols_ เป็น Protocols ที่อธิบายวิธีการที่ทำให้ Node ที่ไม่รู้จักกันสามารถมีปฏิสัมพันธ์ซึ่งกันและเชื่อถือผลการคำนวณและข้อมูลของกันเเละกัน เช่น  Ethereum, Bitcoin, Zcash
    -   _(6) Transient data pub/sub messaging_ เป็น Protocols ที่อธิบายถึงวิธีการสื่อสารข้อมูลที่ไม่ต้องการจะจัดเก็บเเบบถาวร เช่น การอัปเดตสถานะและวิธีการที่ทำให้ Node รับรู้การมีอยู่ของข้อมูลที่ต้องสื่อสาร เช่น Whisper, Matrix
    
-  **Layer 2** เป็นส่วนที่ทำหน้าที่ในการสนับสนุนขั้นที่ 1 ด้วยการเพิ่มความสามารถฟังก์ชันต่าง ๆ อย่างเช่น การจัดเก็บข้อมูลแบบเข้ารหัส (Encrypted Messaging) และการเชื่อมโยงคอมพิวเตอร์หลายเครื่องเข้าด้วยกันบนเครือข่ายเข้าเป็นกลุ่ม เพื่อแบ่งปันข้อมูลและร่วมกันประมวลผล (Distributed Computing)
    -   _(7.1) State channel_ เป็นวิธีการจัด Blockchain มีการเปิด-ปิด Channel โดยให้ Node สื่อสารกันเเบบ Off-Chain จะไม่บันทึกทุกการเปลี่ยนแปลงสถานะบน Main Chain
    -   _(7.2) Plasma protocols_ การย้ายธุรกรรมจาก On-Chain ไป Off-Chain มีการสร้าง Tree of Blockchain
    -   _(7.3) Encrypted Storage_ การจัดเก็บข้อมูลเเบบเข้ารหัส
    -   _(7.4) Storage incentivisation_
    -   _(7.5) Heavy computation_ วิธีการที่ช่วยทำให้ การคำนวณกันบนคอมพิวเตอร์หลายเครื่องเเละการพิสูนจ์ว่าการคำนวณดำเนินไปอย่างถูกต้อง
    -   _(7.6) Distributed secret management_ การจัดเก็บความลับต่าง ๆ พวก Private Key เพื่อให้ข้อมูลสามารถเข้าถึงได้เฉพาะคนที่ได้รับอนุญาตเท่านั้น
    -   _(7.7) Oracles_ เป็นตัวทำหน้าที่นำเข้าข้อมูลจาก Off-Chain เข้าสู่ Blockchain
    
-  **Layer 3** เป็นส่วนที่เกี่ยวกับภาษาที่ใช้ในการเขียนโปรแกรม และ Libraries ซึ่งเป็นที่รวบรวมชุดฟังก์ชันต่าง ๆ เพื่อให้นักพัฒนาเข้ามาใช้พัฒนาแอปพลิเคชันต่าง ๆ ได้อย่างเหมาะสม เช่น Solidity, Rust
    
-  **Layer 4** เป็นส่วนบนสุดของ Stack ที่ได้รวบรวมโปรแกรมที่ผู้ใช้งานทั่วไป ที่ไม่ใช่นักพัฒนาเข้ามาใช้งานโดยตรงกับ Blockchain ได้ เช่น Status, Metamask, MyCrypto, Parity

## References
-   [พาไปรู้จักกับ ‘Web 3.0’](https://www.beartai.com/article/tech-article/914953)
-   [WEB 3.0 คืออะไร?](https://www.finnomena.com/zipmex/what-is-web-3-0/)
-   [https://web3-technology-stack.readthedocs.io/en/latest/](https://web3-technology-stack.readthedocs.io/en/latest/)

## See Also
- [[Blockchain คืออะไร]]
- [[On-Chain Scaling]]
- [[Off-Chain Scaling]]
