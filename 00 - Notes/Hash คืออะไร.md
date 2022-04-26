---
version: "0.0.0"
---
uplinks:: [[Genesis]] [[Hash Function คืออะไร|Hash Function]] [[Blockchain คืออะไร|Blockchain]]
tags:: #type/note #lang/th #people/parinyar
# Hash คืออะไร
**Hash** คือผลลัพธ์ของ [[Hash Function คืออะไร|Hash Function]] 
- เมื่อได้ Hash (Output) มาแล้วจะไม่สามารถคำนวณเพื่อหา Input ได้
- หากอยากทราบ Input ทำได้เพียงแค่สุ่มไปเรื่อยๆ จนกว่าจะเจอ Output ที่ตรงกัน
- ในระบบ [[Blockchain คืออะไร|Blockchain]]
	- Input คือข้อมูลของ Block ก่อนหน้าเมื่อทำการนำไปใส่ยัง [[Hash Function คืออะไร|Hash Function]] แล้วค่า Hash ที่ได้มานั้นเปรียบเสมือนได้ ID ของ Block
	- ถ้าข้อมูลภายใน Block เปลี่ยน ID ที่ได้จาก [[Hash Function คืออะไร|Hash Function]] ก็จะเปลี่ยนไปด้วย ทำให้เมื่อมีการเปลี่ยนแปลงข้อมูลภายใน Block ทุก Block หลังจากนั้นจะต้องทำการอัพเดท ID ให้ตรงกันด้วย

## References

## See Also