---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks::[MOC Type of HD Wallet](./MOC%20Type%20of%20HD%20Wallet.md)
tags:: #lang/th #type/thing

# Use Case of a Hierarchical Tree of Keys
- ใช้หลักการของ[Hierarchical Tree of Keys](./Hierarchical%20Tree%20of%20Keys.md)ในการวางโครงสร้างขององค์ได้ โดยที่ผู้บริหารระดับสูงจะสร้าง Root Seed ออกมา จากนั้นก็สร้าง Child Private Key และ Child Chain Code ให้แต่ละแผนกในองค์กร รวมทั้งสามารถกำหนดสิทธิ์การเข้าถึงต่างกันได้
- การสำรองข้อมูลทำได้ง่าย เนื่องจากผู้บริหารระดับสูง เก็บแค่ตัว Root Seed จะเท่ากับเก็บข้อมูลทั้งหมดขององค์กรไว้ รวมทั้งสามารถเข้าถึง Key ของแผนกอื่นๆ ที่อยู่ในลำดับขั้นที่อยู่ต่ำกว่าได้  ส่วนของแผนกอื่นๆ ที่อยู่ในองค์ก็จะสำรองข้อมูลเเค่เพียง Key ของตนเองไว้ และสามารถเข้าถึง Key ของพนักงานหรือ Key ของลูกค้า ที่อยู่ในลำดับที่ต่ำกว่าได้ 

---
## See also

## References
- Anakorn Kyavatanakij,[A deeper look into Hierarchical Deterministic Wallets](./A%20deeper%20look%20into%20Hierarchical%20Deterministic%20Wallets.md)"2022.