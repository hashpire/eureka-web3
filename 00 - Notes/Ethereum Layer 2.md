## version: "0.0.0"
uplinks:: [[Ethereum]]
tags:: [](app://obsidian.md/index.html#type/note)[#type/note](app://obsidian.md/index.html#type/note) [](app://obsidian.md/index.html#lang/th)[#lang/th](app://obsidian.md/index.html#lang/th) [](app://obsidian.md/index.html#people/Sutida)[#people/Sutida](app://obsidian.md/index.html#people/Sutida)

# Ethereum Layer 2
จุดเริ่มต้นของ Ethereum layer 2
 - Blockchian ที่เราใช้งานกันในปัจจุบัน ไม่ว่าจะเป็น Bitcoin Ethereum หรือเหรียญต่าง ๆ เราจะเรียกมันว่าเป็น *Blockchain Layer 1* คือ โครงสร้างพื้นฐานหลักๆที่แต่ละ Blockchain ใช้ในการบันทึกธุรกรรมลงบนบล็อคและตรวจสอบธุรกรรมต่างๆ มันเปรียบเสมือนเป็น*ถนนเส้นหลักที่ทุกคนใช้งานกัน*
 -  พอ Blockchain นั้นๆมีผู้ใช้งานมากยิ่งขึ้น จำนวนธุรกรรมภายในระบบก็มากขึ้น ก็เปรียบเสมือนจำนวนรถยนต์ที่วิ่งบนถนนที่มากขึ้น ผลที่ตามมาคือ รถติด ไปถึงจุดหมายช้ากว่าเดิม แถมยังเปลืองน้ำมันด้วย อย่าง Blockchain Layer 1 ตัวแรกๆในวงการอย่าง Bitcoin หรือ Ethereum  จำนวนธุรกรรมที่มาก แถมยังรองรับธุรกรรมได้น้อย ทำให้ธุรกรรมของเราล่าช้า แถมยังเสียค่า gas ที่แพงอีกด้วย
 -  Blockchain กำเนิดมารุ่นหลังๆอย่างเช่น Binance Smart Chain,Terra Chain, Solana Chain เห็นถึงปัญหาของ Blockchain รุ่นแรกๆ ว่า ที่มันทำธุรกรรมได้ช้า ก็เพราะมันรองรับธุรกรรมได้น้อย ถนนมันเล็กนิดเดียวเองเลนสองเลน รถติดเปลืองน้ำมันกันไปหมด
 -  Blockchain รุ่นใหม่จึงเพิ่มถนนจากเดิมสองเลนไปเป็นสี่ถึงห้าเลน รถจะได้ไม่ติด ถึงเร็ว ไม่เปลืองน้ำมัน นั่นทำให้  Blockchain รุ่นหลัง ๆให้ความสำคัญกับ **การรองรับธุรกรรมที่มากขึ้น ความสามารถในการทำธุรกรรมเร็วขึ้น และค่าธรรมเนียมถูกสุดๆ**
 -   เเต่ Blockchain รุ่นเเรก อย่าง Bitcoin หรือ Ethereum  ที่สร้างถนนมาแล้ว จะให้ทุบถนนทั้งหมดแล้วสร้างใหม่ก็ไม่ได้เดือดร้อนไปทั้งหมด เขาจึงมีการเกิดไอเดียที่ว่า “ ถ้าเราสร้างถนนใหม่ไม่ได้ เราก็สร้างทางด่วนเลยสิ จะได้ระบายรถจากถนนหลักไปบางส่วนด้วย “ นี่จึงเป็นต้นกำเนิดของ Ethereum Layer 2
 
 ## Ethereum Layer 2 คืออะไร
  - Blockchain ที่ถูกสร้างขึ้นมาเพื่อทำงานร่วมกันกับ Layer 1
  - ทำให้เครือข่ายมีประสิทธิภาพการใช้งานที่ดีขึ้น ลดค่าธรรมเนียมในการทำธุรกรรม รวมถึงการทำธุรกรรมที่เร็วยิ่งขึ้น
 **Ethereum Layer 2 แบ่งเป็นกี่ประเภท? อะไรบ้าง?**
 > EVM ย่อมาจากคำว่า Ethereum Vitual Machine ซึ่งมันเป็นเหมือนซอฟแวร์ที่ไว้สำหรับให้นักพัฒนาสร้างแพลตฟอร์ม หรือ DApps ต่างๆบน Ethereum Chain ถ้า Blockchain Layer 2 ประเภทไหนที่สามารถนำ EVM มาใช้งานได้ โปรแกรมเมอร์ก็แค่นำ code ของ DApps ที่รันอยู่บน Ethereum Chain มาใช้ต่อได้เลยใน Layer 2  ต่างจาก Layer 2 ที่ไม่สามารถนำ EVM มาใช้งานได้ โปรแกรมเมอร์อยากที่สร้าง DApps มารันในเครือข่าย พวกเขาจะต้องเขียน smart contract เองใหม่ทั้งหมดเลย ไม่สามารถ copy code มาใช้งานได้
 1. [[Plasma]] (ใช้ EVM และเป็น Off-chain)
 - มี Blockchain แยกออกมาจาก Ethereum Chain หลัก (Off-chain) 
 - ภายใน Plasma นี้จะสามารถนำแพลตฟอร์มหรือ DApps ที่รันอยู่บน Ethereum Chain มาใช้งานภายใน Blockchain นี้ได้เลย (ใช้ EVM ได้)
 3. [[Validium]] (ไม่ใช้ EVM และเป็น Off-chain)
 - มี Blockchain แยกออกมาจาก Ethereum Chain หลัก (Off-chain)
 - ภายใน Validium จะไม่สามารถนำแพลตฟอร์มหรือ DApps ที่รันอยู่บน Ethereum Chain มาใช้งานภายใน Blockchain นี้ได้ (ใช้ EVM ไม่ได้)
 4. [[Optimistic Rollup]] (ใช้ EVM และเป็น On-chain) 
 -  Blockchain ของมันทำงานร่วมกันกับ Ethereum Chain หลัก (On-chain)
 -  ภายในเครือข่าย Optimistic Rollup จะสามารถนำแพลตฟอร์มหรือ DApps ที่รันอยู่บน Ethereum Chain มาใช้งานภายใน Blockchain นี้ได้เลย (ใช้ EVM ได้)
 5. [[ZK-Rollup]] (ไม่ใช้ EVM และเป็น On-chain)
 - Blockchain ของมันทำงานร่วมกันกับ Ethereum Chain หลัก (On-chain)
 - ภายใน ZK-Rollup จะไม่สามารถนำแพลตฟอร์มหรือ DApps ที่รันอยู่บน Ethereum Chain มาใช้งานภายใน Blockchain นี้ได้ (ใช้ EVM ไม่ได้)

## References
- [ETHEREUM LAYER 2](https://academy.bitcoinaddict.org/what-is-ethereum-layer-2/)
-  [Ethereum LAYER 2 SCALING Explained](https://www.youtube.com/watch?v=BgCgauWVTs0&t=455s)
## See Also