# L'ÉTOILE Registration Demo

Prototype แบบ static ที่ใช้ข้อมูลจำลองใน browser (`localStorage`) โดยไม่เชื่อมฐานข้อมูลหรือบริการภายนอก

## วิธีเปิด

เปิดไฟล์ [index.html](./index.html) โดยตรงใน browser หรือรัน local server จาก root ของ repository:

```bash
python3 -m http.server 4173 --directory Prototype
```

จากนั้นเปิด `http://localhost:4173`

## Routes

- `/` — Guest registration
- `/check-in/` — Staff check-in
- `/admin/` — Admin portal

## Demo accounts

| ส่วนงาน | Username | Password |
| --- | --- | --- |
| Staff check-in | `staff` | `demo123` |
| Admin portal | `admin` | `demo123` |

## ขอบเขตที่จำลองแล้ว

- ลงทะเบียน, ป้องกันอีเมล/เบอร์โทรซ้ำ, และ Digital Pass พร้อม QR code แบบ visual
- ค้นหา QR code ด้วยอีเมลหรือเบอร์โทร
- Staff login, ค้นหา QR code เพื่อ check-in, และ recent check-ins
- Dashboard, reports, search, CSV export, logs, users, event configuration และ import demo records

ข้อมูลที่เพิ่มหรือเปลี่ยนสถานะจะอยู่ใน browser เดียวกันจนกว่าจะล้าง site data/localStorage
