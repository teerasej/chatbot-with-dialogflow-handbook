
# การเพิ่ม Webhook


## 1. กำหนดข้อมูลในฝั่ง DialogFlow

เลือก Agent ที่ต้องการ > เลือก Integration จากเมนูด้านซ้าย และเลือก Facebook Messenger จากรายการ

1. คัดลอกข้อความนี้ เราจะต้องเอาไปใส่ใน Facebook App
2. Verify Token คือข้อความที่เราสามารถกำหนดขึ้นมาได้ และต้องตรงกับที่จะเอาไปใส่ใน Facebook App 
3. Page Access Token ที่ได้จาก Facebook App ให้เอามาใส่ไว้ที่นี้
4. เสร็จแล้วกดปุ่มยืนยัน

<img width="802" alt="2022-01-06_21-39-49" src="https://user-images.githubusercontent.com/85179/148406222-9e3c6327-0a15-4f64-9ec3-a76e623136d9.png">


## 2. กำหนดข้อมูลฝั่ง Facebook App 

กลับมาที่หน้า Messenger Platform จะมีส่วนที่ชื่อ Webhook ให้กดปุ่ม **Add Callback URL**

<img width="991" alt="2022-01-06_21-38-19" src="https://user-images.githubusercontent.com/85179/148405687-3e17e747-53d7-4d69-995d-611d34d2f7af.png">

จากนั้นให้เอาข้อมูลที่ได้จาก Dialogflow มากรอกในส่วนนี้

1. Callback URL 
2. verify token 
3. กดปุ่มยืนยัน ถ้าข้อมูลถูกต้อง จะสามารถใช้งานต่อได้

<img width="701" alt="2022-01-06_21-39-12" src="https://user-images.githubusercontent.com/85179/148406912-4b91ace7-a463-4fe6-8c0a-70e4a6a09719.png">
      
## 3. การจัดการ Webhook และกำหนด Permission

พอเพิ่ม Webhook แล้วจะมีหน้าตาประมาณด้านล่าง

1. หากต้องการแก้ไข Webhook คลิกตรงนี้
2. หากต้องการตรวจสอบว่า Webhook สามารถใช้งานได้ไหม คลิกตรงนี้
3. กดปุ่ม Add Subscription เพื่อกำหนดการใช้งานเพจของ Facebook App 

<img width="963" alt="2022-01-06_21-39-41" src="https://user-images.githubusercontent.com/85179/148407115-7cf4be8d-c6dd-43f5-9512-96a9c2d88f17.png">

จากนั้นเลือกตัวเลือก **message** กับ **messaging_postback**

<img width="695" alt="2022-01-06_21-48-11" src="https://user-images.githubusercontent.com/85179/148407482-6603a1c0-aef0-4146-8959-c95a7f3a4b06.png">
