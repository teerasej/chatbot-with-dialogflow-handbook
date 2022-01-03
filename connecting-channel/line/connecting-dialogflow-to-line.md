
# เรียนรู้วิธีเชื่อมต่อระหว่าง DialogFlow กับ LINE Official Account

## สร้างการเชื่อมต่อจากฝั่ง Dialogflow

1. จาก Dialogflow ให้เลือกเมนูชื่อ integration 
2. เลื่อนลงมาในส่วน text-based แล้วเลือก LINE 

<img width="1060" alt="2022-01-03_20-46-41" src="https://user-images.githubusercontent.com/85179/147937976-d0d29254-64f6-4439-bc97-b942591a5805.png">


## หน้าต่างกรอกข้อมูล 

ส่วนนี้จะต้องมีการนำข้อมูลจาก LINE Messaging API มากรอก และนำข้อมูลจากส่วนนี้ไปกรอกใน LINE Messagign API เช่นกัน

1. Channel ID
2. Channel Secret
3. Channel Access Token 
4. Web Hook URL (ส่วนนี้ต้องนำไปกรอกในฝั่ง LINE Messaging API ให้ทำการคัดลอกเอาไว้)
5. ส่วนของสถานะตัว Channel
6. หลังจากกรอกข้อมูลครบแล้ว ให้กดปุ่ม Start

<img width="794" alt="2022-01-03_21-56-17" src="https://user-images.githubusercontent.com/85179/147945727-3735eb4f-ea37-4a23-9613-af216a1b5c90.png">



