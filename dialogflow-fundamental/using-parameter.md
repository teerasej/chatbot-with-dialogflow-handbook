
# วิธีการใช้งาน parameter

- parameter เป็นค่าที่ Agent จะใช้ในการจดจำข้อมูล รวมถึงส่งต่อให้ intent ตัวอื่น 
- แต่ถ้าต้องการก็สามารถนำมาใช้ภายใน intent ได้เช่นกัน

## 1. การกำหนดความต้องการ parameter และคำถามซ้ำ

เราสามารถกำหนดให้ parameter เป็นข้อมูลที่ Agent จำเป็นต้องถามผู้ใช้ซ้ำได้จนกว่าจะได้ข้อมูลที่ต้องการ

1. สามารถเปิดตัวเลือก required ด้านหน้า parameter ที่ต้องการได้ 
2. สามารถกำหนดคำถามเพื่อให้ Agent ใช้ในการขอข้อมูล

<img width="625" alt="2022-01-04_21-18-04" src="https://user-images.githubusercontent.com/85179/148073030-4d104fa0-1c1e-449f-a68a-da3c3e7c755e.png">

## 2. ทดสอบ RoomReserve 

1. เปิดตัวเลือก required ให้กับ parameter RoomType
2. กำหนดคำถามสำหรับ parameter RoomType 
3. บันทึกการเปลี่ยนแปลงโดยการกดปุ่ม Save 
4. ทดสอบ testing intent

## 3. การแสดงผล Parameter ใน Response

เราสามารถดึงข้อมูลจาก paramter มาใช้ใน response ได้ด้วยการพิมพ์เครื่องหมาย $ นำหน้า และตามด้วยชื่อ parameter

<img width="652" alt="2022-01-04_21-28-47" src="https://user-images.githubusercontent.com/85179/148074002-476e259f-f4e0-4090-b152-c37519e7021d.png">
