# รวม Statement ธนาคารรายวัน

เว็บสำหรับนำไฟล์ Statement ที่ดาวน์โหลดจาก BBL, KBank, KTB และ SCB มาต่อท้ายในไฟล์ Summary BankStatement ตามฟอร์ม

## ไฟล์ใน repository

| ไฟล์ | หน้าที่ |
|---|---|
| `index.html` | หน้าเว็บหลัก มีตัวอ่านไฟล์ Excel และฟอร์ม Summary BankStatement เปล่าอยู่ในไฟล์แล้ว |
| `js/jszip.min.js` | สำรอง: JSZip 3.10.2 (MIT) |
| `js/xlsx.full.min.js` | สำรอง: SheetJS 0.18.5 (Apache-2.0) |
| `.nojekyll` | บอก GitHub Pages ให้แสดงไฟล์ตามที่อัปโหลด |

## วิธีเปิดใช้ GitHub Pages

1. สร้าง repository ใหม่ (เลือก Public ถ้าบัญชี GitHub เป็นแบบฟรี)
2. อัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้ไว้ที่ระดับบนสุดของ repository
3. ไปที่ Settings → Pages → Build and deployment
   - Source: Deploy from a branch
   - Branch: main / (root) → Save
4. รอ 1–2 นาที แล้วเปิด `https://<ชื่อผู้ใช้>.github.io/<ชื่อ repository>/`

## หมายเหตุ

- ไฟล์ Statement และไฟล์ Summary ประมวลผลในเบราว์เซอร์ของผู้ใช้เท่านั้น ไม่ถูกส่งขึ้น GitHub หรือเซิร์ฟเวอร์ใด
- ใน Chrome / Edge ปุ่มบันทึกจะเปิดหน้าต่าง Save As ให้เลือกโฟลเดอร์ได้
- ห้ามอัปโหลดไฟล์ Statement หรือไฟล์ Summary ที่มีข้อมูลจริงไว้ใน repository เพราะ repository แบบ Public ทุกคนเปิดดูได้
