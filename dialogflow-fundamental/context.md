
# การประยุกต์ใช้ Context

ก่อนเริ่มส่วนนี้ให้แน่ใจว่ามีการสร้าง intent ไว้ 2 ตัวแล้ว นั่นคือ 
1. [intent](create-manage-intent-practice-1.md) และ [entity](create-manage-entity-practice-1.md) สำหรับจองห้อง
2. [intent และ entity สำหรับยืมของ](practice-1-tool-reserve.md)



## 1. การให้ข้อมูลที่ซ้ำซ้อน

1. ทดสอบเพิ่ม parameter วันที่สำหรับการจองอุปกรณ์ เข้าไปใน intent ToolReserve และบันทึกการแก้ไข
2. ทดสอบจองห้องประชุม
3. ทดสอบจองอุปกรณ์

สังเกตว่าถ้าเกิดเป็นการจองอุปกรณ์ต่อจากการจองห้องประชุม ผู้ใช้ต้องระบุวันที่ซ้ำซ้อน 2 ครั้ง

ส่วนนี้เราใช้ context ช่วยได้ 

## 2. การกำหนดให้ส่งข้อมูล intent ไปใช้งานใน intent ตัวอื่น ในรูปแบบ Context

เปิด intent **RoomReserve** และกำหนดชื่อลงไปใน output context

<img width="684" alt="2022-01-04_21-58-52" src="https://user-images.githubusercontent.com/85179/148079629-d1b63598-36ee-4a11-b36c-24f95637079a.png">

## 3. นำ context มาใช้งานใน intent ToolReserve

1. กำหนดชื่อของ context ที่ต้องการเรียกใช้ใน intent นี้ในส่วน **input context**
2. สังเกตว่าใน training phase มีส่วนที่ดึงวันที่มาแล้ว
3. ซึ่งวันที่จะถูกนำมากำหนดในชื่อ parameter ว่า **date-time**
4. คลิกเปิดเมนูของ parameter และเลือก Default value วิธีการเรียกใช้ดูจากส่วน **การกำหนดเรียกใช้ค่าจาก context** ที่อยู่ถัดลงไปด้านล่าง
5. เรียกใช้ค่า parameter ใน response

<img width="691" alt="2022-01-04_22-05-31" src="https://user-images.githubusercontent.com/85179/148079634-88ae20bd-d830-412b-940a-f2f1154a28a5.png">

### การกำหนดเรียกใช้ค่าจาก context 

สังเกตว่าขึ้นต้นด้วยเครื่องหมาย **#ชื่อcontext.ชื่อ parameter จาก intent นั้นๆ**

<img width="802" alt="2022-01-04_22-04-36" src="https://user-images.githubusercontent.com/85179/148079637-ef3e714c-ecc2-424f-bdf6-da77eebd1018.png">

## 6. ทดสอบ

1. จองห้องประชุม
2. จากนั้นตามด้วยการจองอุปกรณ์การประชุม