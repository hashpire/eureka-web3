---
version: "0.0.0"
---
uplinks:: [[Genesis]]
tags:: #type/note #lang/th #wallet #people/parinyar
# Chainlink Bangkok Meetup - HD Wallet
- Blockchain Wallets
	- แท้จริงแล้ว Blockchain Wallet ไม่ได้ถูกใช้ในการเก็บเหรียญดิจิทัล แต่ใช้เก็บอย่างเดียวคือ Private key
	- หากต้องการทำธุรกรรมอย่างปลอดภัย ควรจะใช้หลาย Private key 
		- 1  ธุรกรรมต่อ 1 Private key
- Modular Arithmetic
	- คอมพิวเตอร์คำนวณตัวเลขขนาดใหญ่ได้ไม่ค่อยดี จึงได้นำฟังก์ชั่นการหารเอาเศษส่วนมาช่วยในการคำนวณ ตัวอย่างเช่น
		- 7 mod 3 = 1
		- 11 mod 7 = 4
		- -11 mod 7 = 3
	- Hash function คือฟังก์ชั่นการเข้ารหัสแบบทางเดียว (One way) และไม่สามารถคำนวณย้อนกลับหา Input ได้ ตัวอย่างเช่น
		- SHA256("hello") => 2cf24dba5fb0a30e26e83b2ac5b9e29e1b161e5c1fa7425e73043362938b9824
		- Hash function ที่ดีนั้นแม้ Input จะต่างกันเพียงแค่ตัวษรเดียว Output ที่ได้ไม่ควรจะคล้ายคลีงกัน
			- SHA256("hellO") => 04a6f55face2f46be8c23f627d539827615851e10751b63ec59db6d2c706b770
		- Hash function มีหลายอัลกอริทึม ตัวอย่างเช่น
			- SHA256
			- SHA512
			- Keccak-256
			- Keccak-512
- HD Wallets มี 2 ประเภทคือ
	- Non-deterministic Wallet
		- สร้าง Private key ใหม่ทุกครั้งที่ต้องการทำ Transaction
		- ปัญหาของกระเป๋าประเภทนี้คือ
			- มีการทำ Transaction จำนวนมาก
			- การสำรองข้อมูลต้องสำรองทุก Private key ที่สร้างขึ้นมา
			- ไม่รองรับการแชร์ไปยังอุปกรณ์อื่น เพราะว่า Private key ถูกเก็บไว้ใน Software & Application ในเครื่องนั้นๆ
	- Deterministic Wallet 
		- สร้าง Private key ทำโดยการสุ่มตัวเลขขึ้นมา 1 ชุด (Seed) และนำไปเข้าฟังก์ชั่น Key Derivation 
		- ทำการสำรองข้อมูล Seed ก็เท่ากับการเก็บ Private key
		- Type-1 Determinisic Wallet
			- สร้าง Private Key ประกอบไปด้วยการนำ Identifier, Seed, Type ไปเข้า Hash function
			- ไม่สามารถแชร์ Seed ให้กันได้ เนื่องจาก Seed สามารถเข้าถึง Private key ได้
			- หากนำ Seed ไปไว้ในเซิฟเวอร์ แล้วเซิฟเวอร์โดยแฮกก็จะเหมือนสูญเสีย Private key ไปแล้ว
		- Type-2 BIP32 Hierarchical Deterministic Wallet
			- สร้าง Private key โดยใช้มาตรฐานกระเป๋าเงินดิจิทัลยุคใหม่
			- นำ Chain Code มาใช้เพื่อแก้ปัญหาด้านความปลอดภัยจากกระเป๋ารุ่นที่ 1
			- สามารถสร้าง Parent key และ Child key จาก Master key อันเดียวได้
			- ไม่ปลอดภัย เพราะสามารถคำนวณหา Master key ได้
- Hierarchical Tree of Keys
	- สามารถสร้างและคำนวณ Key อื่นๆ ได้ในลักษณะของต้นไม้ โดย Key ที่อยู่ในระดับที่สูงกว่าสามารถคำนวณการ Key ที่อยู่ต่ำกว่าได้
	- สำรองเพียง Key เดียว ยิ่งสูงยิ่งสามารถเข้าถึง Key ด้านล่างได้ทั้งหมด
	- องค์กรสามารถสร้าง Child key ให้กับพนักงานแต่ละแผนก และสามารถกำหนดสิทธิ์การเข้าถึงต่างกันได้
- BIP32 Normal Key Derivation
	- วิธีสร้าง Child Private Key ทำได้โดยการนำ Parent Public Key, Parent Chain Code, Index ไปเข้า Hash function SHA512
	- ทำการแบ่ง Output ที่ได้จาก Hash function SHA512 เป็น 2 ฝั่งซ้ายและขวา
		- ด้านซ้ายมีขนาด 256bit (IL) ทำการนำ Parent Private Key และ IL ไปเข้าฟังก์ชั่น Modular Addition จะได้เป็น Child Private Key
		- ด้านขวามีขนาด 256bit (IR) โดยจะเรียกส่วนนี้ว่าเป็น Child Chain Code
- BIP32 Hardened Key Derivation
	- วิธีสร้าง Child Private Key ทำได้โดยการนำ Parent Private Key, Parent Chain Code, Index ไปเข้า Hash function จะต่างจากแบบ Normal Key Derivation เนื่องจากใช้ Parent Private Key แทนการใช้ Parent Public Key
- BIP32 Public Key Generation
	- วิธีสร้าง Child Public Key ทำได้โดยใช้วิธีเดียวกับการสร้าง Child Private Key แต่จะแตกต่างกันตรงส่วนของ IL ที่จะต้องนำไปเข้าฟังก์ชั่น Point Addition แทนที่จะเอาไปเข้า Modular Addition
- CPK Algorithm
	- วิธีการสร้าง Private key
		1. นำ Identier เข้า Mapping function จะทำให้ได้ Selector Sequence
		2. นำ Selector Sequence และ Private Sequence ไปเข้าฟังก์ชั่น Modular Multiplication
		3. นำ Output จากข้อที่ 2 ไปเข้าฟังก์ชั่น Modular Sum ก็จะได้เป็น Private key
	- วิธีการสร้าง Public Key
		- ขั้นตอนคล้ายกับการสร้าง Private key แต่จะแตกต่างกันตรงที่ใช้ Public Sequence แทน Private Sequence และใช้ฟังก์ชั่น Point Sum แทน Modular Sum ก็จะได้เป็น Public key 
- CPK Security
	- เนื่องจาก Private Squence คือการนำ Private key มาเรียงต่อกันเรื่อยๆ ทำให้ยิ่งมี Private key จำนวนมาก ความปลอดภัยก็จะมากขึ้นไปด้วย

## References

## See Also
