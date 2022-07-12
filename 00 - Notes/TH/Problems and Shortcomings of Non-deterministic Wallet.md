---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [MOC Type of HD Wallet](MOC%20Type%20of%20HD%20Wallet.md)
tags:: #lang/th #type/thing

# Problems and Shortcomings of  Non-deterministic Wallet
1. ในกรณีที่มีการทำธุรกรรมจำนวนมาก จำเป็นที่จะต้องมีความสามารถในการจัดการกับจำนวนของ [Private Key](Private%20Key.md) มากขึ้นตามไปด้วย
	-  จำเป็นต้องสำรองข้อมูลของ Private Key ของ [Address](Address.md) ที่มีการสร้างขึ้นมา เนื่องจากว่า หากในกรณีที่ระบบมีปัญหา เราจะไม่สามารถใช้เงินที่มีอยู่ได้
	- การสำรองข้อมูลจำนวนมาก จะทำให้เกิดปัญหาด้าน [Scalability](Scalability%20of%20Blockchain.md)ได้
2. [Non-deterministic Wallet](Non-deterministic%20Wallet.md)  ไม่รองรับการแชร์ไปยังอุปกรณ์อื่น เนื่องจาก Private key จะถูกเก็บไว้ใน Software และ Application ในเครื่องนั้นๆ

## See also
- [Early workarounds of Non-deterministic Wallet](Early%20workarounds%20of%20Non-deterministic%20Wallet.md)
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.