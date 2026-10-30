# Thai Analyzer (Static Frontend)

Frontend สำหรับ Thai Analyzer ที่เรียก Backend จาก Google Apps Script

## วิธี Deploy บน Render.com

1. Push ไฟล์นี้ขึ้น GitHub (ดูขั้นตอนด้านล่าง)
2. ใน Render → New → Static Site
3. เชื่อม GitHub repo
4. Build Command: ว่างไว้
5. Publish Directory: `.` หรือ `public` (ถ้าแยกโฟลเดอร์)
6. Deploy

## ตั้งค่า Backend URL

เปิด `index.html` แล้วแก้บรรทัดนี้:

```js
const BACKEND_URL = "https://script.google.com/macros/s/YOUR_DEPLOYMENT_ID/exec";
```

ใส่ลิงก์ `/exec` จริงที่ได้จาก Google Apps Script

## หมายเหตุ

- Backend ยังต้อง Deploy บน Google Apps Script ตามปกติ
- หน้าเว็บนี้เป็นแค่ Frontend ที่เรียก API จาก Apps Script
