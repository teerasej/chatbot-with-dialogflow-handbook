
# สร้าง Intent สำหรับเก็บข้อมูล ชื่อ นามสกุล และ Email 

1. คลิกสร้าง** Follow-up Intent - custom **ใหม่ ต่อจาก **Start Registration**
2. ตั้งชื่อ **Start Registration - Full name**
3. กำหนด training phase
 - ชื่อ Peter นามสกุล Parker Email training@nextflow.in.th

โดยในที่นี้ให้เลือก และกำหนด Entity ตามลำดับ
 - **Peter** เลือกเป็น Entity เป็น **@sys.any** และกำหนดชื่อ parameter เป็น **firstName**
 - **Parker** เลือกเป็น Entity เป็น **@sys.any** และกำหนดชื่อ parameter เป็น **lastName**
 - **training@nextflow.in.th** เลือกเป็น Entity เป็น **@sys.email** และกำหนดชื่อ parameter เป็น **email**

และกำหนด ให้ทุก parameter เป็น required และใส่ข้อความสำหรับขอข้อมูลใน prompt ด้วย

4. กำหนด Response

ขอบคุณค่ะ ตรวจสอบข้อมูลว่าถูกต้องไหมนะคะ
ชื่อ: $firstName
นามสกุล: $lastName
Email: $email
