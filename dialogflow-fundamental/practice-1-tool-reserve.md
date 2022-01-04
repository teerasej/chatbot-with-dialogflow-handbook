
# 

ในที่นี้ให้ลองสร้าง Entity และ Intent เพื่อยืมอุปกรณ์สำหรับใช้ในการประชุม

## สร้าง Entity

1. กำหนดชื่อเป็น MeetingRoomTool
2. กำหนดรายชื่ออุปกรณ์เป็น 
   - projector
   - whiteboard
   - HDMI Cable 

จากนั้นกำหนด synnonym ตามสมควร


## สร้าง Intent 

1. กำหนดชื่อ ToolReserve
2. กำหนด training phase ที่มีการระบุ Entity **MeetingRoomTool**
3. กำหนดให้ parameter **MeetingRoomTool** เป็นแบบ required
4. กำหนดคำถามซ้ำเพื่อให้ผู้ใช้ระบุชื่ออุปกรณ์
5. แสดง Response ที่แจ้งชื่ออุปกรณ์

<img width="685" alt="2022-01-04_21-49-10" src="https://user-images.githubusercontent.com/85179/148076964-5dd2f1c9-5ab0-42fc-9ea2-191f970babb5.png">
