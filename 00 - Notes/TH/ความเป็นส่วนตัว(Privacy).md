---
version: "0.0.1"
cover_image:
published: true
contributors: ["Sutida"]
---
uplinks:: [[MOC The need for multiple  keys]]
tags:: #lang/th #type/thing

# ความเป็นส่วนตัว(Privacy)
ความเป็นส่วนตัว(Privacy) เป็นเหตุผลแรกของการที่เราจำเป็นต้องมี Key และ Addresses จำนวนมากใน [[Blockchain]] ประกอบด้วย
- *Pseudonymous (นามแฝง) และ Anonymous (ไม่ระบุตัวตน)*
   Public Blockchain ส่วนใหญ่ไม่ว่าจะเป็น [[Ethereum]] หรือ [[Bitcoin]] จะเป็นแบบ Pseudonymous คือ จะมีการใช้นามแฝงในการทำธุรกรรม เช่น เราจะรู้ว่า A โอนเงินไป B แต่เราแค่จะไม่รู้ว่า A กับ B คือใคร แตกต่างกับ Anonymous ที่เราจะไม่รู้เลยว่าใครทำอะไร หรือใครมีเงินอยู่เท่าไร
- *Address reuse (การใช้บัญชีซ้ำ ๆ)*
   เนื่องจาก Blockchain ใช้นามแฝงแทนตัวบุคคลในการทำธุรกรรม หากเราใช้ บัญชีเดียวในการทำธุรกรรมทั้งหมด อาจจะทำให้บุคคลอื่นสามารถหาปฏิสัมพันธ์ระหว่างที่เกิดขึ้นเรากับบุคคลอื่น และเชื่อมโยงมาถึงตัวเราได้ เช่น เราเปิดร้านขายสินค้า แล้วใช้บัญชีเดียวทั้งหมด บุคคลอื่นสามารถที่จะหาปฏิสัมพันธ์ที่เกิดขึ้นระหว่างเราที่เป็นผู้ขาย และลูกค้าของเรา จนสามารถรู้ได้ว่าเราขายสินค้าใด 

---
## See also
- [[ความปลอดภัย(Security)]]
## References
- Anakorn Kyavatanakij,"[[A deeper look into Hierarchical Deterministic Wallets]],"2022.