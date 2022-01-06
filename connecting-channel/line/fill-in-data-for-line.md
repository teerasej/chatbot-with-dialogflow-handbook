
# การตั้งค่าสำหรับการเชื่อมต่อกับ Dialog Flow

## 1. เก็บข้อมูลเพื่อนำไปเชื่อมต่อกับ Dialogflow 

จากรายละเอียดของ Channel ให้คัดลอกข้อมูลตามรายการด้านล่าง เก็บไว้ใน Note ดังนี้

1. Basic Setting > Channel ID
2. Basic Setting > Channel Secret
3. Messaging API > Channel Access Token > กดปุ่ม Issue จะได้เลข Token มา

## 2. กรอกข้อมูลใน Dialogflow Integration 

กลับมาที่ Dialogflow ในหน้าจอ LINE Integration ให้กรอกข้อมูลที่ได้มาลงไปในช่องให้ถูกต้อง

<img width="794" alt="2022-01-03_21-56-17" src="https://user-images.githubusercontent.com/85179/147948282-44c67520-8b0e-4e59-bbb1-8f490899e0db.png">


## 3. ตั้งค่า Webhook

จากนั้นให้เอาส่วนของ Web hook จากฝั่งของ Dialogflow มาใส่ในส่วน Web hook ใน LINE Messaging API

Provider > Channel > Messaging API > Web Hook

<img width="889" alt="2022-01-03_22-17-23" src="https://user-images.githubusercontent.com/85179/147947778-f6457cc8-29e6-4e79-b279-74411bd87f57.png">

เสร็จแล้วกดปุ่ม Verify เพื่อเช็คว่าตัว LINE Messaging API สามารถติดต่อกับ Web hook ของ Dialogflow ได้

และอย่าลืมกดเปิด webhook ด้านล่างด้วน 

<img width="773" alt="2022-01-06_20-30-48" src="https://user-images.githubusercontent.com/85179/148391767-55907de5-ea86-471f-a57c-0c2984457e02.png">


## 4. ตั้งค่า LINE Official Account Feature หากต้องการ

ส่วนนี้ไม่ได้จำเป็นมาก แต่เราสามารถเปิดปิดการทำงานของ LINE Official Account จากตรงนี้ได้เลย โดยการกดปุ่ม Edit ทางด้านขวา

1. เปิด/ปิด ให้บอทสามารถเข้าร่วม group line ได้
2. เปิด/ปิด ข้อความตอบกลับอัตโนมัติ (ปกติจะปิดถ้าใช้ bot)
3. เปิด/ปิด ข้อความทักทาย 

<img width="763" alt="2022-01-06_20-39-31" src="https://user-images.githubusercontent.com/85179/148391838-30553959-e12d-45c8-8c9b-68d81ec440ce.png">


