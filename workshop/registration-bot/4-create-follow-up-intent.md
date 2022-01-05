
# กำหนด Follow-up Intent สำหรับยืนยันข้อมูล

ในที่นี้ให้สร้าง follow-up intent ต่อจาก **Start Registration - Full name**

1. follow-up yes
2. follow-up later
3. follow-up no 

เพื่อเป็น intent ที่โต้ตอบภายหลังจากลูกค้าเลือกยืนยันความถูกต้อง

## 1. StartRegistration - Full name - yes

กำหนด response 

```
ขอบคุณค่ะ ลงทะเบียนให้เรียบร้อยนะคะ กรุณาตรวจสอบ Email ที่ส่งไปให้เพื่อยืนยันด้วยค่ะ
```

## 2. StartRegistration - Full name - later

กำหนด response 

```
ขอบคุณที่สนใจกิจกรรมของเรานะคะ ถ้าเปลี่ยนใจกลับมาลงทะเบียนกับเราต่อได้ค่ะ
```

## 3. StartRegistration - Full name - no

กำหนด response 1 และ 2 ตามลำดับ

```
1: รบกวนกรอกชื่อ นามสกุล และ Email อีกรอบตามรูปแบบด้านล่างนะคะ
2: ชื่อ Peter นามสกุล Parker Email peter@parker.com
```