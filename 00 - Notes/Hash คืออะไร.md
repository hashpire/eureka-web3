---
version: "0.0.0"
---
uplinks:: [[Genesis]]
tags:: #type/note #lang/th #people/parinyar
# Hash คืออะไร
**Hash** คือ Output ของ Hash Function หลังจากที่เราใส่ Input เข้าไป Hash Function เป็นฟังก์ชั่นอะไรก็ได้ที่เป็นแบบ One way หมายความว่าจะทราบว่า Output คืออะไร แต่ไม่สามารถทราบได้ว่า Input ที่ทำให้ได้ Output ออกมาแบบนี้คืออะไร การเปลี่ยน Input แค่ตัวอักษรเดียวทำให้ Hash เปลี่ยนและไม่ใกล้เคียงก่อนหน้าเลยแม้จะเปลี่ยนแค่ 1 ตัวอักษร วิธีเดียวที่จะรู้ Input ได้ คือต้องสุ่มจนกว่าจะได้ Output ที่ตรงกัน ถึงจะรู้ว่า Input คืออะไร 

**ในระบบ Blockchain**, Input คือ ข้อมูลของ Block ก่อนหน้านี้เมื่อทำการใส่ไปยัง Hash Function แล้วค่า Hash ที่ได้มานั้นเปรียบเสมือน ID ของ Block ถ้าข้อมูลภายใน Block เปลี่ยน ID ก็จะเปลี่ยนไปด้วย 
ตัวอย่างเช่น มี Block ที่เชื่อมต่อกันในระบบทั้งหมด 3 Block หากข้อมูลของ Block 1st เปลี่ยนแปลง จะกระทบกับ Block 2nd และ 3rd ด้วย เนื่องจาก Block 2nd มีค่า Hash ID ของ Block 1st อยู่และ Block 3rd ก็มี Hash ID ของ Block 2nd อยู่ด้วย ทำให้เมื่อ Block 1st อัพเดทข้อมูล จำเป็นต้องอัพเดททุก Block หลังจาก Block 1st ด้วย


## References

## See Also