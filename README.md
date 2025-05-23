
<h1 align="center">🎤 คาราโอเกะซิตี้ - ระบบจองห้องคาราโอเกะด้วย Django</h1>
<p align="center">
  <img src="Screenshorts_Project/log_index.png" alt="Karaoke" style="max-width: 100%;" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Django-4.2%2B-green?logo=django" alt="Django Version">
  <img src="https://img.shields.io/badge/Bootstrap-5.3-purple?logo=bootstrap" alt="Bootstrap Version">
</p>

<p align="center">
  ระบบจองเว็บคาราโอเกะ
</p>

---

## 🧠 Stack ที่ใช้

- 💻 Django (Back-end)
- 🎨 Bootstrap 5 (Front-end)
- 🗄 SQLite (Database dev mode)
- 🔐 ระบบ Auth แยก User และ Admin

---

## 🚀 ฟีเจอร์หลัก

* 👤 **ระบบสมาชิก:**
    * ลงทะเบียน (Register)
    * เข้าสู่ระบบ (Login)
    * (ตัวเลือก) ลืมรหัสผ่านผ่านอีเมล
* 🔒 **การยืนยันตัวตน:**
    * บังคับให้ผู้ใช้ล็อกอินก่อนทำการจองห้อง
* 📅 **ระบบการจอง:**
    * แสดงรายการห้องว่างให้เลือก
    * ฟอร์มสำหรับกรอกข้อมูลการจอง (ชื่อ, วันเวลาเริ่มต้น-สิ้นสุด)
    * แสดงหน้ายืนยันเมื่อการจองสำเร็จ
    * แสดงรายการจองทั้งหมดของผู้ใช้ (หรือทั้งหมดในระบบ)
    * แก้ไขและลบการจองได้
* 💰 **การคำนวณ:**
    * คำนวณระยะเวลาการจอง (ชั่วโมง)
    * คำนวณค่าบริการตามราคาห้องและระยะเวลา
* 📞 **การติดต่อ:**
    * หน้าฟอร์มสำหรับติดต่อ/แจ้งปัญหา (ผ่าน Modal ใน Base Template)

---

## 🖼 ตัวอย่างหน้าจอระบบ

### 🗟 หน้าแรกเว็บไซต์ก่อนล็อกอิน

<img src="Screenshorts_Project/unlog_index.png" width="100%" />

### 🔐 หน้าล็อกอิน

<img src="Screenshorts_Project/login.png" width="100%" />

### 📝 สมัครสมาชิก

<img src="Screenshorts_Project/register.png" width="100%" />

### 🎶 หน้าเลือกจองห้อง

<img src="Screenshorts_Project/log_index.png" width="100%" />

### 📝 ฟอร์มจองห้องคาราโอเกะ

<img src="Screenshorts_Project/booking_form.png" width="100%" />

### 💯 หน้าเมื่อจองห้องเสร็จ

<img src="Screenshorts_Project/booking_success.png" width="100%" />

### 📜 ประวัติการจองทั้งหมด

<img src="Screenshorts_Project/booking_all.png" width="100%" />

### 📞 ติดต่อ/แจ้งปัญหา

<img src="Screenshorts_Project/contact.png" width="100%" />

---

## 🧱 โครงสร้างโปรเจกต์ (บางส่วน)
```
kraoke_project/
├── accounts/                                     # แอปพลิเคชันจัดการระบบผู้ใช้
│   ├── templates/
│   │   └── accounts/
│   │       ├── login.html                        # เทมเพลตหน้าเข้าสู่ระบบ
│   │       └── register.html                     # เทมเพลตหน้าลงทะเบียน
│   └── ... (models.py, views.py, urls.py, etc.)
├── booking/                                      # แอปพลิเคชันจัดการระบบการจอง
│   ├── templates/
│   │   └── booking/
│   │       ├── base.html                         # เทมเพลตหลัก (Navbar & Footer)
│   │       ├── all_bookings.html                 # เทมเพลตแสดงรายการจองทั้งหมด
│   │       ├── booking_form.html                 # เทมเพลตฟอร์มการจอง
│   │       ├── booking_success.html              # เทมเพลตแสดงผลเมื่อจองสำเร็จ
│   │       └── room_list.html                    # เทมเพลตแสดงรายการห้อง
│   └── ... (models.py, views.py, urls.py, etc.)
├── kraoke_project/                               # โฟลเดอร์โปรเจกต์หลัก (settings.py, urls.py)
├── manage.py                                     # สคริปต์จัดการ Django
└── README.md                                     # เอกสารแนะนำโครงการ
```

---

## 🚀 วิธีรันโปรเจกต์ (Dev Mode)

### 1. ติดตั้ง Django
```bash
pip install django
```

### 2. รัน migration และสร้าง superuser
```bash
python manage.py migrate
python manage.py createsuperuser
```

### 3. รันเซิร์ฟเวอร์
```bash
python manage.py runserver
```

---

## 💌 ติดต่อผู้พัฒนา

<div align="center">

<table>
  <tr>
    <td align="center"><strong>📧 Email</strong></td>
    <td><a href="mailto:minkridsada233@gmail.com">minkridsada233@gmail.com</a></td>
    <td><a href="mailto:wuttipatphuakmaneeo@gmail.com">wuttipatphuakmaneeo@gmail.com</a></td>
    <td><a href="mailto:Teeraphat15.km@gmail.com">Teeraphat15.km@gmail.com</a></td>
  </tr>
  <tr>
    <td align="center"><strong>🔗GitHub</strong></td>
    <td><a href="https://github.com/minkpn">minkpn</a></td>
    <td><a href="https://github.com/wuttipatphuakmanee">Wuttipat</a></td>
    <td><a href="https://github.com/Teerapatkm">Patlom</a></td>
  </tr>
  <tr>
    <td align="center"><strong>💬 Line</strong></td>
    <td>@minkpn</td>
    <td>@Wuttipat</td>
    <td>@Patlom</td>
  </tr>
</table>

</div>

---

<h1 align="center">✨ Made with ❤️ by minkpn x Wuttipat x Patlom</h1>
