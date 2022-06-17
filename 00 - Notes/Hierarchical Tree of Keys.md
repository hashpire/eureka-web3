---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC HD Wallet]]
tags:: #lang/th #type/thing

# Hierarchical Tree of Keys
*Hierarchical Tree of Keys* การสร้าง Key ออกมาในลักษณะของต้นไม้ 
- ลำดับบนสุดสามารถสร้างค่า Root Seed ออกมาหนึ่งค่า จากนั้นสร้าง Parent Private  Key (Master Private Key) และ Parent Chain Code (Master Chain Code) ออกมา แล้วคำนวณ Child Private Key และ Child Chain Code ออกมา ให้กับลำดับขั้นที่ต่ำลงมา ซึ่งในลำดับขั้นที่ต่ำลงมาสามารถนำเอา Child Private Key และ Child Chain Code มาใช้เป็น  Parent Private  Key และ Parent Chain Code ในลำดับขั้นของตนเอง เพื่อสร้าง Child Private Key และ Child Chain Code ให้กับลำดับขั้นที่ต่ำลงไปอีกได้ โดยสามารถสร้างตามหลักการนี้ได้เรื่อย ๆ  
- มาตราฐานที่ใช้คือ BIP44 / SLIP44
---
## See also
- [[Use Case of a Hierarchical Tree of Keys]]
## References

