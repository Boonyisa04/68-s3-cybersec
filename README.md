# Cyber Security

## Owner
- 6702041511021
- Boonyisa Aiamsamarng
- s6702041511021@email.kmutnb.ac.th

### มาตรการด้านความปลอดภัย (Security Implementations)
- **Network Isolation**: มีการสร้างเครือข่ายส่วนตัวชื่อ `my-network` เพื่อให้ระบบทั้งสองคุยกันได้ภายในเท่านั้น เพื่อความปลอดภัย
- **Environment Variables**: ใช้ตัวแปร `${PGADMIN_EMAIL}` และ `${PGADMIN_PASSWORD}` เพื่อหลีกเลี่ยงการฝังรหัสผ่านลงในโค้ดโดยตรง
- **Branch Protection**: ตั้งค่าป้องกัน Branch `main` บน GitHub เพื่อป้องกันการแก้ไขไฟล์สำคัญโดยไม่ผ่านการตรวจสอบ (Pull Request)

### ขั้นตอนการติดตั้งและรันระบบ
1. **รันส่วนจัดการฐานข้อมูล (Admin)**:
   ```bash
   docker compose -f admin.yaml up -d