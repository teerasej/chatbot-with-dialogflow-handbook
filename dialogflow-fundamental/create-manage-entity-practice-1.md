
# การทำบอทจองห้องประชุม 2

## เพิ่ม Entity ให้กับ RoomReserveBot 

ให้ทำการสร้าง Entity ดังนี้

1. กำหนดชื่อ Entity เป็น RoomType
2. กำหนด refernce value เป็น small, medium, และ Large
3. กำหนด symnonym เป็นคำที่เกี่ยวข้อง
4. กดปุ่ม Save

<img width="683" alt="2022-01-04_20-52-51" src="https://user-images.githubusercontent.com/85179/148069273-c0fc75c2-4d9e-45a9-a72a-be3b87d38ebe.png">

## ใช้งาน Entity กับ Intent

เปิดกลับมาที่ Intent ชื่อ RoomReserve

1. ทดลองเพิ่ม training phase ใหม่ โดยเจาะจงให้มีคำที่ตรงกับ symnonym ใน entity ที่สร้างไว้
2. สังเกตว่า Agent จะนำคำที่ตรงกับ entity มาแสดงไว้ในส่วน Action and Parameters และกำหนดชื่อ entity

<img width="660" alt="2022-01-04_21-01-22" src="https://user-images.githubusercontent.com/85179/148070370-842addac-c816-439f-86e2-88282364a994.png">

## ทดสอบ 1

1. ทดลองเพิ่ม training phase ที่มีคำใกล้เคียงกับ entity แต่ไม่ตรงซะทีเดียว เช่น **ห้องเล็ก** แทนที่จะเป็น **ห้องประชุมเล็ก**
2. สังเกตผล
3. ลองกลับไปเพิ่ม synnonym **ห้องเล็ก** ใน entity และกดปุ่ม Save
4. กลับมาทดสอบกับ intent อีกครั้งด้วยคำเดิม
5. สังเกตผลอีกครั้ง
6. ทดสอบใช้ส่วน testing เพื่อทดสอบ intent

## ทดสอบ 2

1. ทดลองเพิ่ม training phase ที่มีวันที่จองลงไปด้วยเช่น **จองห้องประชุมเล็กวันที่ 9 มกราคม 2565**
2. สังเกตผล
3. ทดสอบใช้ส่วน testing เพื่อทดสอบ intent

<img width="653" alt="2022-01-04_21-09-47" src="https://user-images.githubusercontent.com/85179/148071412-55968aee-d64f-4b53-bd98-6bd3c476ff41.png">
