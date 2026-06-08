# 🎨 DVE Self-Learning Program — Infographic Script

> เอกสารสรุปครบวงจรของระบบทั้งหมด พร้อมคำแนะนำภาพประกอบ
> ใช้สำหรับสร้าง Infographic ใน Canva / Figma / PowerPoint / Adobe Illustrator

---

## 📋 สารบัญ

1. [ภาพรวมระบบ](#1-ภาพรวมระบบ)
2. [โครงสร้างผู้ใช้งาน 5 บทบาท](#2-โครงสร้างผู้ใช้งาน-5-บทบาท)
3. [โครงสร้างเนื้อหา (Hierarchy)](#3-โครงสร้างเนื้อหา-hierarchy)
4. [Workflow ครู](#4-workflow-ครู)
5. [Workflow นักเรียน](#5-workflow-นักเรียน)
6. [Workflow ผู้ดูแลระบบ](#6-workflow-ผู้ดูแลระบบ)
7. [Features เด่นทั้งระบบ](#7-features-เด่นทั้งระบบ)
8. [Multi-Content Support](#8-multi-content-support)
9. [Security & Reliability](#9-security--reliability)
10. [Technology Stack](#10-technology-stack)
11. [Image Resources & Design](#11-image-resources--design)
12. [Layout Templates](#12-layout-templates)

---

## 1. ภาพรวมระบบ

### 🎯 Main Title

```
🎓 DVE Self-Learning Program
ระบบการเรียนรู้ด้วยตนเอง สำหรับอาชีวศึกษา
```

### 💬 Tagline

```
"เรียนได้ทุกที่ ทุกเวลา ติดตามได้ทุกการเรียนรู้"
Vocational E-Learning Platform Built for Thailand
```

### 📝 What is DVE?

ระบบ E-Learning ครบวงจรที่ออกแบบเฉพาะสำหรับสถานศึกษาอาชีวะของไทย รองรับการเรียนการสอนแบบ Self-paced ที่นักเรียนเรียนรู้ได้ตามจังหวะของตัวเอง ครูสามารถสร้างเนื้อหาได้หลากหลายรูปแบบ และผู้บริหารดูผลการเรียนรู้ได้แบบ Real-time

### 📊 Key Statistics

| Metric | Value | Description |
|--------|-------|-------------|
| 🏫 | Multi-tenant | รองรับหลายสถานศึกษาในระบบเดียว |
| 👥 | 5 บทบาท | Super Admin / Admin / Executive / Teacher / Student |
| 📚 | Unlimited | ชั้นเรียน บทเรียน และเนื้อหาไม่จำกัด |
| 🎬 | 2 GB | ขนาดไฟล์วิดีโอสูงสุดต่อไฟล์ |
| 📄 | Sequential | PDF เปิดทีละหน้า ป้องกันการข้าม |
| ⚡ | 500+ concurrent | รองรับผู้ใช้งานพร้อมกันได้ |
| 🔒 | 2FA + OTP | ความปลอดภัยระดับสูง |
| 📍 | GPS Tracking | ติดตามตำแหน่งตอนสอบ |

### 🖼️ ภาพแนะนำ

- **Hero Image:** นักเรียนอาชีวะ (ชาย+หญิง) ในชุดนักศึกษา ยิ้มแย้ม ใช้ Laptop/Tablet
- **Background:** Gradient สีแบรนด์ (Crimson → Pink → Indigo)
- **Decorative:** Pattern จุดเล็กๆ, เส้นโค้งโปร่งใส, รูปทรงเรขาคณิต
- **Hero Logo:** Logo DVE ขนาดใหญ่ตรงกลาง

---

## 2. โครงสร้างผู้ใช้งาน 5 บทบาท

### 🎯 Title

```
👥 5 บทบาทผู้ใช้งาน
แต่ละบทบาทมีหน้าที่และสิทธิ์ต่างกัน
```

### 🔐 Role Hierarchy

```
┌─────────────────────────────────────┐
│  🌟 Super Admin                      │ ← ดูแลทั้งระบบ
│  ดู/แก้/ลบทุกอย่างในระบบทุกสถานศึกษา │
└──────────────┬──────────────────────┘
               ↓
┌─────────────────────────────────────┐
│  🏢 Admin                            │ ← ผู้ดูแลสถานศึกษา
│  จัดการครู นักเรียน สาขาวิชา ระดับ  │
└──────────────┬──────────────────────┘
               ↓
┌──────────────┴──────────────┐
↓                              ↓
┌─────────────┐         ┌─────────────┐
│ 👔 Executive│         │ 👨‍🏫 Teacher │ ← ผู้สอน
│ ดูรายงาน    │         │ สร้างเนื้อหา│
│ ไม่แก้ไข    │         │ สอน + รายงาน│
└─────────────┘         └──────┬──────┘
                               ↓
                        ┌─────────────┐
                        │ 👨‍🎓 Student │ ← ผู้เรียน
                        │ เข้าเรียน    │
                        │ ทำแบบทดสอบ  │
                        └─────────────┘
```

### 📋 Permissions Matrix

| สิทธิ์ | Super Admin | Admin | Executive | Teacher | Student |
|------|:-----------:|:-----:|:---------:|:-------:|:-------:|
| จัดการสถานศึกษา | ✅ | ❌ | ❌ | ❌ | ❌ |
| จัดการครูในสถานศึกษา | ✅ | ✅ | ❌ | ❌ | ❌ |
| สร้างชั้นเรียน | ✅ | ✅ | ❌ | ✅ | ❌ |
| สร้าง/แก้ไขเนื้อหา | ✅ | ✅ | ❌ | ✅ | ❌ |
| ดูรายงาน | ✅ | ✅ | ✅ | ✅ (เฉพาะตัว) | ❌ |
| เข้าเรียน + ทำแบบทดสอบ | ✅ | ✅ | ❌ | ✅ | ✅ |
| Duplicate ชั้นเรียน | ✅ | ✅ | ❌ | ✅ | ❌ |
| Maintenance Mode | ✅ | ❌ | ❌ | ❌ | ❌ |

### 🖼️ ภาพแนะนำ

- Avatar แต่ละบทบาทแบบ flat illustration (5 ตัว)
- ใช้สีต่างกันแยกแต่ละ role
- Icon ครอบรูปแบบ shield/badge สำหรับ permission level

---

## 3. โครงสร้างเนื้อหา (Hierarchy)

### 🎯 Title

```
🏗️ โครงสร้างเนื้อหาเป็นชั้น
จัดเก็บข้อมูลอย่างเป็นระบบ
```

### 📊 Hierarchy Diagram

```
🏫 สถานศึกษา (School)
└── 🎓 สาขาวิชา (Department)
    └── 📊 ระดับชั้น (Level/Grade)
        └── 📚 ชั้นเรียน (Classroom)
            ├── 👨‍🏫 ครูผู้สอน (Teacher)
            ├── 👨‍🎓 นักเรียน (Students)
            └── 📖 บทเรียน (Lessons)
                └── 📄 เนื้อหา (Contents)
                    ├── 🎬 วิดีโอ (Video)
                    ├── 📑 เอกสาร PDF (Document)
                    └── ❓ แบบทดสอบ (Quiz)
                        └── 📝 คำถาม (Questions)
                            └── ✓ ตัวเลือก (Options)
```

### 💡 ตัวอย่าง Real-world

```
🏫 วิทยาลัยอาชีวศึกษานครสวรรค์
└── 🎓 สาขาวิชาคอมพิวเตอร์ธุรกิจ
    └── 📊 ปวช.1
        └── 📚 การโปรแกรมเบื้องต้น (ห้อง 1/1)
            └── 📖 บทที่ 1: เกริ่นนำ
                ├── 🎬 วิดีโอแนะนำ Python (15 นาที)
                ├── 📑 เอกสารประกอบ (50 หน้า)
                └── ❓ แบบทดสอบบทที่ 1 (10 ข้อ)
```

### 🖼️ ภาพแนะนำ

- Tree diagram แบบ organic / mind map
- Icons แต่ละ level ใช้สีไล่ tone
- เพิ่ม folder/file icons สไตล์ modern

---

## 4. Workflow ครู

### 🎯 Title

```
👨‍🏫 สำหรับครูผู้สอน
สร้างชั้นเรียนได้ใน 5 ขั้นตอน
```

### 📋 5 Steps Journey

#### **Step 1️⃣ สร้างชั้นเรียน**
```
🏫 Create Classroom
─────────────────────
• ตั้งชื่อ + คำอธิบาย
• เลือก: สาขาวิชา / ระดับชั้น
• ตั้งการมองเห็น:
   🔒 ส่วนตัว (เฉพาะนักเรียนที่เชิญ)
   🏢 ภายในสถานศึกษา
   🌐 สาธารณะ (ครูคนอื่น Duplicate ได้)
• สร้าง Invite Link / รหัสชั้นเรียน
```

#### **Step 2️⃣ เพิ่มบทเรียน**
```
📚 Add Lessons
─────────────────────
• สร้างบทเรียน 1, 2, 3, ...
• ลำดับการเรียนรู้แบบ Sequential
• Drag & Drop จัดลำดับใหม่ได้
• จัดกลุ่มเป็น Indent/Sub-lesson
• Draft mode → Publish เมื่อพร้อม
```

#### **Step 3️⃣ อัปโหลดเนื้อหา**
```
📤 Upload Contents
─────────────────────
🎬 วิดีโอ (สูงสุด 2 GB)
   • Chunked upload — รองรับไฟล์ใหญ่
   • Background upload widget
   • Auto-transcode → 720p H.264
   • นำทางไปหน้าอื่นได้ระหว่างอัป

📑 PDF Documents
   • Drag & drop upload
   • Sequential viewer attached

❓ แบบทดสอบ
   • Multiple choice
   • กำหนดเกณฑ์ผ่าน (เช่น 60%)
   • จำกัดจำนวนครั้งทำได้
```

#### **Step 4️⃣ เผยแพร่**
```
🚀 Publish
─────────────────────
• เปลี่ยน "ฉบับร่าง" → "เผยแพร่"
• ดูตัวอย่างก่อนเผยแพร่
• แชร์ Invite Link ให้นักเรียน
• หรือเปิด Public ให้ครูคนอื่น Duplicate
```

#### **Step 5️⃣ ติดตามผล**
```
📊 Monitor Progress
─────────────────────
• ดูใครเรียนถึงไหน (% per content)
• คะแนนแบบทดสอบรายบุคคล
• Quiz attempts history
• ตำแหน่ง GPS ตอนสอบ (ป้องกันโกง)
• Export Excel report
```

### 🖼️ ภาพแนะนำ

- ครูยืน + chalkboard ดิจิทัล
- Step icons แต่ละขั้น
- Arrow connectors ระหว่าง steps
- Screenshot mockup ของแต่ละหน้า (Frame ใน laptop)

---

## 5. Workflow นักเรียน

### 🎯 Title

```
👨‍🎓 สำหรับผู้เรียน
เรียนรู้แบบ Self-paced อย่างเป็นระบบ
```

### 📋 6 Steps Journey

#### **Step 1️⃣ ลงชื่อเข้าใช้**
```
🔐 Sign In
─────────────────────
• ลงทะเบียนด้วย Email + รหัสนักศึกษา
• 2-Factor OTP ผ่าน Email
• Trusted Device 30 วัน
• Password Reset via Email
```

#### **Step 2️⃣ เข้าร่วมชั้นเรียน**
```
🎟️ Join Classroom
─────────────────────
• คลิก Invite Link จากครู
• หรือใส่รหัสชั้นเรียน
• Auto-enroll พร้อมเข้าเรียน
```

#### **Step 3️⃣ เริ่มเรียนตามลำดับ**
```
📖 Start Learning
─────────────────────
ดูเนื้อหาที่ปลดล็อกแล้ว:
   🎬 วิดีโอ — เล่นได้, seek ได้
   📑 PDF  — Sequential page unlock
   ❓ Quiz — ทำแบบทดสอบ
   
🔒 เนื้อหาถัดไป Lock อยู่
   จนกว่าจะผ่านเงื่อนไข
```

#### **Step 4️⃣ ระบบจดจำให้**
```
💾 Auto Resume
─────────────────────
• วิดีโอ — กลับมาเล่นต่อจุดเดิม
• PDF — เปิดหน้าที่อ่านล่าสุด
• Max page reached — บันทึก
• Quiz — เห็นประวัติคะแนน
```

#### **Step 5️⃣ ปลดล็อกบทต่อไป**
```
🔓 Unlock Next
─────────────────────
เงื่อนไขผ่าน:
✅ ดูวิดีโอจบ (90%+)
✅ อ่าน PDF จนถึงหน้าสุดท้าย
✅ ผ่านแบบทดสอบ (≥ เกณฑ์)
        ↓
ปลดล็อก: บท / เนื้อหาถัดไป
```

#### **Step 6️⃣ ดูผลการเรียน**
```
🏆 Track Progress
─────────────────────
• Progress % แต่ละบท
• Quiz scores history
• เวลาที่ใช้เรียน
• ใบประกาศ / Certificate
   (ถ้ามีการตั้งค่า)
```

### 🖼️ ภาพแนะนำ

- นักเรียนใช้ Laptop/Mobile หลายอุปกรณ์
- Progress bar visual (0% → 100%)
- Lock/unlock icons animation
- Trophy / Certificate ที่จุดจบ

---

## 6. Workflow ผู้ดูแลระบบ

### 🎯 Title

```
🛠️ สำหรับผู้ดูแลระบบ
จัดการระบบและสถานศึกษาได้ง่าย
```

### 📋 Admin Capabilities

```
👑 Super Admin
─────────────────────
• ดู/แก้/ลบ ทุกสถานศึกษา
• สร้าง Admin ของแต่ละโรงเรียน
• Maintenance Mode (ปิดระบบทั้งหมด)
• Database & Backup management
• System-wide analytics

🏢 Admin (ระดับโรงเรียน)
─────────────────────
• จัดการครู + นักเรียน
• สาขาวิชา / ระดับชั้น
• ดูรายงานของโรงเรียน
• Approve เนื้อหาก่อนเผยแพร่
• Quota / Storage management

👔 Executive (ผู้บริหาร)
─────────────────────
• ดูรายงานเชิงสถิติ
• KPI dashboard
• เปรียบเทียบสาขาวิชา
• ไม่แก้ไขข้อมูล (Read-only)
```

### 🛡️ Maintenance Mode

```
🔧 Maintenance Mode (3 Stages)
─────────────────────
Stage 1: 📢 Modal — แจ้งเตือนเด่นชัด
Stage 2: 📋 Drawer — เลื่อนเก็บข้าง
Stage 3: 🎯 Handle — มือจับเล็กๆ

User ยังเห็นได้ตลอดว่ามีการบำรุงรักษา
แต่ไม่กวนระหว่างใช้งานอื่น
```

### 🖼️ ภาพแนะนำ

- Dashboard mockup
- Settings/gear icons
- Maintenance illustration
- Multi-tenant diagram

---

## 7. Features เด่นทั้งระบบ

### 🎯 Title

```
✨ 12 Features เด่น
ที่ทำให้ DVE เหนือกว่าระบบทั่วไป
```

### 🌟 Feature Highlights

#### 1️⃣ 🎬 **Smart Video Pipeline**
```
อัปโหลดครั้งเดียว เล่นได้ทุกอุปกรณ์
─────────────────────
✓ Chunked upload (รองรับไฟล์ 2 GB)
✓ Background processing
✓ Auto-transcode → 720p H.264 1-pass CRF
✓ HTTP Range request (seek เร็ว)
✓ Adaptive bitrate (max 2.5 Mbps)
✓ Media Fragment URI resume
```

#### 2️⃣ 📑 **Sequential PDF Viewer**
```
ป้องกันการข้ามเนื้อหา
─────────────────────
✓ เปิดได้ทีละหน้า
✓ ปลดล็อกตามที่อ่านจริง
✓ Per-student progress tracking
✓ Max page reached lock
✓ Resume to last page
```

#### 3️⃣ ❓ **Quiz with GPS Tracking**
```
แบบทดสอบที่ป้องกันการโกง
─────────────────────
✓ Multiple choice + auto-grading
✓ จำกัดจำนวนครั้งทำได้
✓ GPS location ตอนเริ่ม + ส่ง
✓ Time tracking per question
✓ Attempt history per student
```

#### 4️⃣ 🔄 **Classroom Duplication**
```
คัดลอกชั้นเรียนของครูคนอื่นได้
─────────────────────
✓ เฉพาะชั้นเรียน Public หรือของตัวเอง
✓ Shared file (ประหยัด disk)
✓ Reset progress สำหรับชั้นใหม่
✓ Source tracking (ใครคัดมาจากใคร)
✓ Confirm modal อธิบายชัดเจน
```

#### 5️⃣ 📊 **Real-time Analytics**
```
ครูเห็นภาพรวมทั้งห้อง
─────────────────────
✓ Per-student progress
✓ Quiz scores breakdown
✓ Average completion time
✓ Identify struggling students
✓ Export to Excel
```

#### 6️⃣ 🔒 **Multi-Factor Authentication**
```
ปลอดภัยตามมาตรฐาน
─────────────────────
✓ Email + Password
✓ OTP 6-digit via Email
✓ Trusted Device (30 days)
✓ Password reset secure flow
✓ Session management
```

#### 7️⃣ 🎯 **Maintenance Mode**
```
ระบบที่ดูแลตัวเองได้
─────────────────────
✓ ปิดระบบเฉพาะ user ทั่วไป
✓ Admin ยังเข้าได้
✓ 3-stage notice (Modal/Drawer/Handle)
✓ Custom message
✓ Toggle one-click
```

#### 8️⃣ 📤 **Background Upload Manager**
```
อัปโหลดในเบื้องหลัง ใช้งานต่อได้
─────────────────────
✓ Multi-file concurrent upload
✓ Progress widget floating
✓ Cancel mid-upload
✓ Resume on resume
✓ beforeunload guard
```

#### 9️⃣ ♻️ **Soft Delete + Restore**
```
ลบแล้วยังกู้คืนได้
─────────────────────
✓ Soft delete classrooms
✓ Soft delete contents
✓ Restore by Admin
✓ Audit trail
✓ Auto cleanup orphan files
```

#### 🔟 🛡️ **Race-Condition Safe**
```
ระบบที่ทนทานต่อสถานการณ์เผลอ
─────────────────────
✓ Concurrent upload safe
✓ Transcode + delete safe
✓ Queue retry_after tuned
✓ Worker process group signaling
✓ Auto-recovery on crash
```

#### 1️⃣1️⃣ 🚀 **Auto-Recovery**
```
Server ดับ → กลับมาเองอัตโนมัติ
─────────────────────
✓ Proxmox auto-boot containers
✓ systemd services enabled
✓ Supervisor auto-restart workers
✓ Docker containers restart=always
✓ Cron schedules persist
```

#### 1️⃣2️⃣ 🎨 **Modern UX**
```
หน้าจอที่ใช้งานง่าย สวยงาม
─────────────────────
✓ Responsive (Mobile/Tablet/Desktop)
✓ Dark/Light mode (ถ้ามี)
✓ Smooth animations
✓ Toast notifications
✓ Skeleton loaders
✓ Confirm modals everywhere
```

### 🖼️ ภาพแนะนำ

- Feature grid 4x3 (12 features)
- Icon ใหญ่กลางการ์ดแต่ละใบ
- สี gradient หลังการ์ด
- Hover effect ถ้าทำ web version

---

## 8. Multi-Content Support

### 🎯 Title

```
📦 รองรับ Content หลากหลายรูปแบบ
ครอบคลุมทุกวิธีการสอน
```

### 📋 Content Types

#### 🎬 **Video Content**
```
รายละเอียดทางเทคนิค:
─────────────────────
• Format:     MP4 (H.264 + AAC)
• Max Size:   2 GB per file
• Resolution: Auto → 720p
• Bitrate:    1.5 Mbps (CRF 23)
• Audio:      128 kbps stereo
• Features:   
  - Seek (HTTP Range)
  - Resume (Media Fragment URI)
  - Speed control (0.5x - 2x)
  - Closed captions (ถ้ามี)
```

#### 📑 **PDF Document**
```
รายละเอียดทางเทคนิค:
─────────────────────
• Format:     PDF (any version)
• Max Size:   100 MB
• Viewer:     react-pdf 10.4
• Features:
  - Sequential page lock
  - Zoom in/out
  - Per-student progress
  - Mobile responsive
  - Lazy loading pages
```

#### ❓ **Quiz**
```
รายละเอียดทางเทคนิค:
─────────────────────
• Type:       Multiple choice
• Questions:  Unlimited
• Options:    2-6 per question
• Features:
  - Random order (optional)
  - Time limit (optional)
  - Pass threshold (%)
  - Max attempts
  - GPS tracking
  - Score history
```

### 🖼️ ภาพแนะนำ

- 3 ใบใหญ่ๆ ของแต่ละ content type
- Mockup ของ player/viewer แต่ละแบบ
- Highlight features ด้านข้าง

---

## 9. Security & Reliability

### 🎯 Title

```
🛡️ ความปลอดภัยและความเสถียร
ระดับ Production Grade
```

### 🔐 Security Features

```
👤 Authentication
─────────────────────
✓ Email + Password (Bcrypt hashed)
✓ Email OTP verification
✓ Trusted device (30-day)
✓ Session management
✓ Password reset via email

🔒 Authorization
─────────────────────
✓ Role-based access control (5 roles)
✓ Permission matrix
✓ School isolation
✓ Content visibility levels
✓ Audit logging

🌐 Network Security
─────────────────────
✓ HTTPS / TLS
✓ CORS configuration
✓ CSRF protection
✓ XSS prevention
✓ SQL injection guards (Eloquent)

📍 Anti-Cheating
─────────────────────
✓ GPS tracking during exams
✓ IP logging
✓ Sequential content lock
✓ Page-by-page PDF
✓ Time tracking
```

### 🛠️ Reliability Features

```
⚡ Performance
─────────────────────
✓ HTTP Range request streaming
✓ Chunked upload (5MB chunks)
✓ Background queue workers
✓ Database query optimization
✓ Lazy loading

🔄 Auto-Recovery
─────────────────────
✓ Container auto-boot
✓ Service auto-restart
✓ Worker auto-respawn
✓ Schedule auto-retry
✓ Health checks

🧹 Self-Maintenance
─────────────────────
✓ Daily orphan cleanup (03:00)
✓ Hourly temp clear (xx:25)
✓ Log rotation
✓ Cache auto-rebuild
✓ Race-condition guards
```

### 🖼️ ภาพแนะนำ

- Shield + checkmark icons
- Lock illustrations
- Server room / cloud
- Auto-recovery diagram

---

## 10. Technology Stack

### 🎯 Title

```
💻 Modern Tech Stack
สร้างจากเทคโนโลยีชั้นนำ
```

### 🛠️ Stack Breakdown

#### **Frontend**
```
⚛️ React 19          — UI Framework
⚡ Vite 7            — Build tool
🎨 Tailwind CSS      — Styling
📦 TanStack Query    — Data fetching
🐻 Zustand           — State management
🎭 Headless UI       — Components
📄 react-pdf 10      — PDF viewer
🎬 Native HTML5      — Video player
```

#### **Backend**
```
🚀 Laravel 12        — PHP Framework
🐘 PHP 8.3           — Runtime
🔐 Sanctum           — API auth
📧 Laravel Mail      — Email service
🎬 php-ffmpeg        — Video processing
📦 Pion ChunkUpload  — Chunked upload (concept)
🗄️ Eloquent ORM     — Database
🔄 Queue + Supervisor — Background jobs
```

#### **Database & Storage**
```
🐬 MySQL 8           — Primary DB
📁 Local Storage     — File system
🔗 Symlink           — Public access
💾 LVM-thin          — Volume management
📊 541 GB allocated  — Storage capacity
```

#### **Infrastructure**
```
🖥️ Proxmox 9.1      — Hypervisor
📦 LXC Containers    — Lightweight VMs
🌐 Nginx             — Web server
🐘 PHP-FPM           — Application server
🐳 Docker            — DB containers
🔄 Supervisor        — Process manager
⏰ Cron              — Scheduler
🔌 Tailscale         — VPN access
```

#### **Production Tools**
```
🎬 FFmpeg 6.1        — Transcoding
   • 1-pass CRF 23
   • preset=fast
   • tune=film
   • maxrate 2.5 Mbps
```

### 🖼️ ภาพแนะนำ

- Tech logos grid (official logos)
- Architecture diagram
- Server stack visualization
- Cloud + connectivity lines

---

## 11. Image Resources & Design

### 🌈 Color Palette

```
Primary (Crimson):    #DC2626  rgb(220, 38, 38)
Secondary (Pink):     #EC4899  rgb(236, 72, 153)
Accent (Indigo):      #6366F1  rgb(99, 102, 241)
Success (Green):      #10B981  rgb(16, 185, 129)
Warning (Amber):      #F59E0B  rgb(245, 158, 11)
Danger (Red):         #EF4444  rgb(239, 68, 68)
Info (Blue):          #3B82F6  rgb(59, 130, 246)

Background Light:     #FFFFFF
Background Subtle:    #F9FAFB
Background Card:      #F3F4F6

Text Primary:         #1F2937
Text Secondary:       #6B7280
Text Muted:           #9CA3AF
Border:               #E5E7EB
```

### 🔤 Typography

```
Heading (Thai):       Sarabun ExtraBold
Heading (English):    Inter Bold / Poppins
Body (Thai):          Sarabun Regular
Body (English):       Inter Regular
Numbers:              Poppins SemiBold
Code:                 JetBrains Mono / Fira Code
```

### 🆓 Free Image Resources

| Type | Source | URL |
|------|--------|-----|
| Icons | Heroicons | https://heroicons.com |
| Icons | Tabler Icons | https://tabler-icons.io |
| Icons | Lucide | https://lucide.dev |
| Illustrations | Storyset | https://storyset.com |
| Illustrations | unDraw | https://undraw.co |
| Illustrations | Open Doodles | https://www.opendoodles.com |
| Photos | Unsplash | https://unsplash.com |
| Photos | Pexels | https://www.pexels.com |
| 3D Avatars | Memoji Generator | https://www.memojigenerator.app |
| 3D Avatars | Persona by Draftbit | https://personas.draftbit.com |
| Mockups | Mockup World | https://www.mockupworld.co |
| Patterns | Hero Patterns | https://heropatterns.com |
| Gradients | UI Gradients | https://uigradients.com |

### 📸 Photos to Capture/Find

**Hero Images:**
- นักเรียนอาชีวะใช้ระบบ (Laptop/Mobile)
- ครูยืนหน้าจอแสดงเนื้อหา
- กลุ่มนักเรียนเรียนร่วมกัน
- Classroom setting แบบทันสมัย

**Lifestyle:**
- มือถือกับ Notebook คู่กัน (responsive)
- Headphone + Coffee + Laptop
- Student at home learning

**Tech:**
- Server room (ถ้าจะแสดง infrastructure)
- Code on screen
- Network diagram

### 🖼️ Screenshot Suggestions

ต้องเตรียม screenshot ของ:

1. **Dashboard** — หน้าแรกหลัง login
2. **Classroom List** — รายการชั้นเรียน
3. **Classroom Detail** — ภายในชั้นเรียน
4. **Lesson View** — หน้าเรียน (3 modes: video/PDF/quiz)
5. **Video Player** — กำลังเล่นวิดีโอ
6. **PDF Sequential Viewer** — เปิดทีละหน้า
7. **Quiz Interface** — ทำแบบทดสอบ
8. **Upload Widget** — กำลังอัปโหลด
9. **Reports** — Dashboard ของครู
10. **Mobile View** — Responsive

---

## 12. Layout Templates

### 📐 Page Sizes

```
A4 Vertical (Print):
   210 × 297 mm @ 300 DPI
   2480 × 3508 px

A4 Horizontal (Print):
   297 × 210 mm @ 300 DPI
   3508 × 2480 px

Instagram Square:
   1080 × 1080 px

Instagram Story:
   1080 × 1920 px

Facebook Post:
   1200 × 630 px

Twitter Post:
   1600 × 900 px

LinkedIn Post:
   1200 × 627 px

PowerPoint 16:9:
   1920 × 1080 px

YouTube Thumbnail:
   1280 × 720 px
```

### 🎨 Suggested Layouts

#### **Layout A: Single Long Vertical** (สำหรับ Web/Social)
```
┌────────────────────┐
│   [Hero + Title]   │
├────────────────────┤
│  📊 Key Stats      │
├────────────────────┤
│  Workflow ครู      │
├────────────────────┤
│  Workflow นักเรียน │
├────────────────────┤
│  Features          │
├────────────────────┤
│  Tech Stack        │
├────────────────────┤
│  [CTA + Footer]    │
└────────────────────┘
```

#### **Layout B: Multi-page A4** (สำหรับ Print/PDF)
```
Page 1: Hero + Overview + Stats
Page 2: Teacher Workflow
Page 3: Student Workflow
Page 4: Features Grid (12 items)
Page 5: Tech + Contact
```

#### **Layout C: Square Grid** (สำหรับ Social Carousel)
```
Slide 1: 🎓 Title
Slide 2: 📊 Stats
Slide 3: 👨‍🏫 Teacher Flow
Slide 4: 👨‍🎓 Student Flow
Slide 5: ✨ Top Features
Slide 6: 🛡️ Security
Slide 7: 📞 Contact + CTA
```

### 📏 Spacing Guide

```
✓ Use multiples of 8px (8, 16, 24, 32, 48, 64)
✓ Border radius: 12-16px (modern look)
✓ Card padding: 24-32px
✓ Section gap: 48-64px
✓ Element gap: 16-24px
✓ Icon size: 24-48px (depending on hierarchy)
✓ Shadow: soft, low opacity (1-2 layers)
```

---

## 🎬 Bonus: Slogans & CTAs

### 💬 Slogans (ภาษาไทย)

```
🎯 "เรียนได้ทุกที่ ทุกเวลา"
🎯 "ระบบเรียนรู้ที่อาชีวศึกษาไทยรอคอย"
🎯 "ครูสร้างได้ง่าย นักเรียนเรียนได้สนุก"
🎯 "ติดตามผลการเรียนรู้แบบ Real-time"
🎯 "เปลี่ยนการเรียนการสอน ด้วยเทคโนโลยี"
🎯 "Self-paced Learning ที่นักเรียนชอบ"
```

### 💬 Slogans (English)

```
🎯 "Learn Anywhere, Anytime, at Your Pace"
🎯 "Modern E-Learning for Vocational Education"
🎯 "Empowering Thai Vocational Schools"
🎯 "Built for Students, Loved by Teachers"
🎯 "Where Tradition Meets Technology"
```

### 📢 Call-to-Action

```
👉 ทดลองใช้งานฟรี
👉 สมัครเป็นโรงเรียนนำร่อง
👉 ติดต่อเพื่อ Demo
👉 Scan QR Code เพื่อเริ่มต้น
👉 เข้าร่วมการอบรมครู
```

---

## 📦 Deliverables Checklist

ก่อนเริ่มทำ Infographic ตรวจสอบให้แน่ใจว่ามี:

- [ ] **Logo DVE** — PNG transparent + SVG
- [ ] **Color codes** — Hex values (ตามที่ระบุ)
- [ ] **Fonts** — Sarabun + Inter (download ใน Google Fonts)
- [ ] **Screenshots** — 10 รูปจากระบบจริง
- [ ] **Icons** — ดาวน์โหลด Heroicons set
- [ ] **Hero photo** — นักเรียน/ครู (จากสถานศึกษา)
- [ ] **Stats verified** — ตัวเลขที่ใช้ check จริง
- [ ] **Tech logos** — Official logos ของ frameworks
- [ ] **QR Code** — link ไปยัง website ระบบ
- [ ] **Contact info** — Email, Phone, Website

---

## 🚀 Production Steps

1. **เลือก Tool**
   - 🎨 Canva (ง่ายสุด มี template เยอะ)
   - 🖌️ Figma (ละเอียดสุด ใช้ระบบ design)
   - 📊 Adobe Illustrator (Pro grade)
   - 📑 PowerPoint (รวดเร็ว ใช้ในที่ทำงาน)

2. **เริ่มจาก Wireframe** (กระดาษหรือ digital)
3. **สร้าง Color System + Type System** ก่อน
4. **วาง Layout** ตาม Section ที่กำหนด
5. **เพิ่ม Content** ทีละ Section
6. **เพิ่ม Icons + Illustrations**
7. **เพิ่ม Screenshots** ใน mockup frames
8. **Review** — อ่านได้ไหม / รก/ไม่รก
9. **Export** — High res PNG + PDF + Source file

---

## 📞 Contact Template (สำหรับ Footer)

```
🌐 Website:    https://nvc.tailb765d4.ts.net
📧 Email:      contact@dve-school.ac.th
📱 Tel:        02-XXX-XXXX
📍 Address:    [Your School Address]

Powered by:
🎓 DVE Self-Learning Program v1.0.0
Built with ❤️ for Thai Vocational Education

© 2026 Your Institution Name
```

---

## ✅ Document Status

```
Version:        1.0.0
Last Updated:   2026-06-04
For Use With:   DVE Self-Learning Program
License:        Internal Use
Maintained By:  [Your Name]
```

---

**End of Document** 📋

ใช้ document นี้เป็น single source of truth ในการทำ Infographic ทุกเวอร์ชั่นและทุก format ครับ ถ้ามีอะไรเพิ่ม/แก้ — กลับมา edit ที่นี่ที่เดียวจบ 🎨✨
