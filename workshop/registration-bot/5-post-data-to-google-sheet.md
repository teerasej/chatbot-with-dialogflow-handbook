

# ส่งข้อมูลเข้า Google Sheet

> ส่วนนี้จะเป็นการ Setup และมีการทำงานกับการเขียนโปรแกรมเข้ามาร่วมด้วย ถ้าไม่ถนัดก็สามารถดูขอบเขตการทำงานแทนได้ครับ

## 1. สร้าง Google Sheet 

ตั้งชื่ออะไรก็ได้ แต่ต้องก้อปปี้ URL มาใช้งาน

<img width="666" alt="2022-01-05_21-24-45" src="https://user-images.githubusercontent.com/85179/148248749-078e49f3-0ad0-4ccd-86e0-2ea1e0b48b14.png">


## 2. สมัครใช้งาน SheetDB

1. เข้าไปที่ https://sheetdb.io/ และสมัครเข้าใช้ด้วย Google Account พร้อมกดอนุญาตให้สามารถเปลี่ยนแปลงแก้ไขข้อมูลใน Google sheet ได้
2. จากนั้นกดสร้าง Free API 
3. นำ URL ของ Google Sheet ที่เตรียมไว้มาวางไว้ในช่อง และกด Create

<img width="1023" alt="2022-01-05_21-24-38" src="https://user-images.githubusercontent.com/85179/148249415-720943d9-d753-469c-ac17-5cb0cc1e9c61.png">

4. กรอกชื่อ field ให้ตรงกับใน parameter ของ Dialogflow และกดปุ่มยืนยัน

<img width="1009" alt="2022-01-05_21-25-12" src="https://user-images.githubusercontent.com/85179/148249656-922d40cd-8610-4f4e-ae5d-0dc486e65381.png">

5. จะได้ URL ของ API ที่เชื่อมกับ Google Sheet มา ส่วนนี้เอาไปส่งต่อสำหรับให้ Developer ใช้งาน

<img width="946" alt="2022-01-05_21-25-26" src="https://user-images.githubusercontent.com/85179/148249855-3fc25efa-fb56-4546-bc76-9e81668c1467.png">


## 3. เปิดการทำงานของ fulfillment ใน intent ที่ต้องการ

กลับมาที่ Dialog flow และเข้าไปที่ intent **StartRegistration - Full name - yes**
ลงมาด้านล่างสุด และเปิดการทำงานของ Fulfillment ในส่วน Enable webhook call for this intent

<img width="657" alt="2022-01-05_21-28-57" src="https://user-images.githubusercontent.com/85179/148249933-a723d38c-35a0-4e37-96a8-3e93a60d82f8.png">


## 4. เปิดการเชื่อมต่อ fulfillment ให้กับ Agent 

จากเมนูทางด้านซ้ายให้เลือก fulfillment และ enable webhook integration

<img width="1264" alt="2022-01-05_21-29-23" src="https://user-images.githubusercontent.com/85179/148250396-86024240-2c26-435a-8b05-5b0d53d1c152.png">

ส่วนนี้ให้นำ URL ของระบบที่ developer จัดเตรียมไว้มาวางในช่อง URL และกด SAVE

## 5. ทดสอบใช้งาน agent มาจนถึง intent ที่กำหนด และตรวจสอบ Google Sheet

### Note

- สำคัญมากที่ชื่อของ intent, parameter และ context ในฝั่งของ dialogflow ต้องสอดคล้องกับฝั่งที่ Developer นำไปใช้ 
- หากมีการปรับเปลี่ยนชื่อต้องมีการแจ้ง developer ให้ทราบ เพราะจะทำให้ระบบไม่สามารถจับคู่ชื่อกับข้อมูลที่นำไปใช้ได้