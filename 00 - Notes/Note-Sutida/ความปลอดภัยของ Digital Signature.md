---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[Digital Signature-MOC]]
tags:: #lang/th #type/concept

# ความปลอดภัยของ Digital Signature
ประกอบด้วย
1. *การเข้ารหัสลายมือชื่อ (Signature Encryption)* ทำให้ลายมือชื่อมีความปลอดภัยสูง และทุกลายมือชื่อบนเอกสารสามารถตรวจสอบว่าตรงกับลายมือชื่อที่เก็บไว้หรือไม่
2. *การรับรองลายมือชื่อ (Certify Signature)* จากองค์กรที่รับรองลายมือชื่อ ทั้งภาครัฐและเอกชน ซึ่งลายมือชื่อที่ถูกเข้ารหัสเเละได้รับการรับรองจะถูกเก็บไว้ 2 ที่ คือ
    1. [ระบบลงลายมือชื่ออิเล็กทรอนิกส์ (e-Memo)](https://www.codium.co/e-signature) โดยเมื่อผู้ใช้งานสร้างเอกสารเเละลงลายมือชื่ออิเล็กทรอนิกส์บนระบบนี้ลายมือชื่อที่ลงไปจะมาจากลายมือชื่อที่ถูกเก็บ    
    2. ฮาร์ดเเวร์ที่เก็บลายมือชื่อโดยเฉพาะ (Hardware security module : HSM)  ระบบ e-Memo จะส่งลายมือชื่อที่ถูกรับรองแล้วไปที่ HSM หากลายมือชื่อตรงกันจะถือว่าลายมือชื่อนี้มีความน่าเชื่อถือตามกฎหมาย
3. *การปิดเอกสาร (Document Integrity)* เมื่อการลงลายมือชื่อเสร็จสิ้นระบบจะดำเนินการปิดเอกสารหรือสัญญา ไม่ให้สามารถลงลายมือชื่อต่อเเละเปลี่ยนแปลงเอกสารที่ได้ทำการบันทึกไว้		

---
## See also
- [[Digital Signature]]
- [[คุณสมบัติเด่นของ Digital Signature]]
## References
- [Siwanad,"Advanced e-signature/Digital Signature"](https://codium.co/blogs/30-What-the-difference-between-e-signature-and-digital-signature?utm_source=google&utm_medium=cpc&utm_campaign=eMemo-article&utm_content=Article-230821-esigvsdigital&utm_term=digital%20signature%20%E0%B8%84%E0%B8%B7%E0%B8%AD&gclid=CjwKCAjw9e6SBhB2EiwA5myr9tUT98mFOEcTg_LE8kmYmzY0Q7_5XniIeg5Nb4mwD8ziNTuTi6qENBoCRO8QAvD_BwE)
- ["บทนำเกี่ยวกับเทคโนโลยีความปลอดภัยของข้อมูล,"2560](https://www.nrca.go.th/content/02-1.html)
