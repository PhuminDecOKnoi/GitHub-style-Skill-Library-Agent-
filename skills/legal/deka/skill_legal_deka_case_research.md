# SKILL — Legal Deka Case Research

## Version
2.1

## Purpose
ใช้สำหรับค้นหา ตรวจสอบ วิเคราะห์ เปรียบเทียบ และจัดการองค์ความรู้จากคำพิพากษาศาลฎีกาอย่างเป็นระบบ โดยให้ GitHub ทำหน้าที่เป็น Workflow Engine และให้ Google Drive / Internal Knowledge ทำหน้าที่เป็น Knowledge Base หลัก

หลักบังคับ: Internal Knowledge First → STOU 41216 → ตัวบทกฎหมายฉบับทางการ → คำพิพากษาศาลฎีกา → แหล่งราชการและวิชาการ

## Core Principles

1. อ่านไฟล์ที่ผู้ใช้ให้และความรู้ภายในก่อน
2. โหลด SKILL MASTER จาก Google Drive ก่อนเริ่มวิเคราะห์
3. ใช้หน่วยเรียน STOU 41216 ที่เกี่ยวข้องเป็นแกนวิชาการ
4. ค้นและแสดงตัวบทกฎหมายก่อนอ้างฎีกา
5. ตรวจวันเกิดเหตุและกฎหมายที่ใช้บังคับในวันนั้น
6. ตรวจเลขฎีกา ปี ประเด็น และสาระจากแหล่งที่เชื่อถือได้
7. แยกข้อเท็จจริง ประเด็นกฎหมาย เหตุผลศาล ผลคำพิพากษา และความเห็น
8. ห้ามแต่งข้อเท็จจริง มาตรา เลขฎีกา หรือคำวินิจฉัย
9. ตรวจอายุความทุกครั้งเมื่อวิเคราะห์คดี
10. Output เป็น Plain Text โดยค่าเริ่มต้น

## Hybrid Legal Knowledge Architecture

User Request
↓
GitHub Skill / Workflow
↓
Source Resolver
├── Google Drive Master Skill
├── STOU 41216 Unit 1–15
├── Statutory Law Files
├── Internal Deka / Case Files
└── External Official Sources
↓
Legal Analysis
↓
Deka Knowledge Base Update

## Source Registry

ให้ใช้ไฟล์ `config/legal_source_registry.md` เป็นทะเบียนแหล่งความรู้กลาง โดยทะเบียนต้องระบุอย่างน้อย:

- Source ID
- Provider
- File title / path / connector reference
- Subject scope
- Authority level
- Currency / effective-date rule
- Retrieval instruction
- Fallback source

ห้ามถือว่าข้อความใน GitHub เชื่อมกับ Google Drive โดยอัตโนมัติ ต้องเรียกค้นแหล่งข้อมูลผ่าน connector จริงทุกครั้ง

## Mandatory Step 0 — Source Resolution

ก่อน Search ฎีกา ต้องดำเนินการตามลำดับนี้:

1. โหลด GitHub Skill ฉบับปัจจุบัน
2. อ่าน `config/legal_source_registry.md`
3. ค้นหาและอ่าน Google Drive Master Skill
4. ระบุหน่วย STOU 41216 ที่เกี่ยวข้อง
5. ค้นหาเนื้อหาจากหน่วยนั้น
6. ค้นหาตัวบทกฎหมายฉบับเต็มจากแหล่งภายในหรือแหล่งราชการ
7. ตรวจวันที่ใช้บังคับของกฎหมายเทียบวันเกิดเหตุ
8. ตรวจแหล่งฎีกาภายในก่อนค้นภายนอก
9. จัดทำ Source Availability Report
10. จึงเริ่ม Deka Engine

## Source Availability Report

ต้องแสดงสถานะแหล่งข้อมูลก่อนวิเคราะห์:

- GitHub Skill: Loaded / Not Loaded
- Source Registry: Loaded / Not Loaded
- Google Drive Master Skill: Loaded / Not Found
- STOU Unit: Unit number + Found / Not Found
- Statutory Text: Found / Not Found / Currency Unverified
- Deka Source: Full Text / Digest / Secondary Citation / Not Found
- External Verification: Required / Not Required / Completed
- Analysis Status: Proceed / Limited Proceed / Stop

## Stop Rules

1. ไม่พบตัวบทกฎหมาย → ห้ามคัดหรือสร้างตัวบทจากความจำ
2. ไม่พบหน่วย STOU ที่เกี่ยวข้อง → แจ้งข้อจำกัดและห้ามอ้างว่าเป็นคำอธิบายจาก STOU
3. พบเพียงบทคัดย่อฎีกา → ใช้ได้เฉพาะสาระที่แหล่งรองรับและต้องระบุข้อจำกัด
4. เลขฎีกาไม่ครบหรือขัดกัน → เก็บใน Research Queue และยังไม่เพิ่ม Knowledge Base
5. กฎหมายปัจจุบันกับกฎหมายวันเกิดเหตุต่างกัน → ต้องแสดงทั้งสองสถานะและเลือกฉบับที่ใช้กับคดี
6. หาก Source Resolution ไม่ผ่านจุดสำคัญ → หยุดสรุปความเห็นเด็ดขาดและระบุข้อมูลที่ต้องหาเพิ่ม

## Source Priority

1. ไฟล์หรือภาพที่ผู้ใช้อัปโหลด
2. Google Drive / Internal Knowledge
3. STOU 41216 Unit 1–15
4. ตัวบทกฎหมายฉบับทางการที่ใช้บังคับในวันเกิดเหตุ
5. ศาลยุติธรรม / ศาลฎีกา
6. เอกสารราชการ
7. งานวิชาการหรือฐานข้อมูลรอง

## Deka Engine

Source Resolution
↓
Search
↓
Verify
↓
Extract
↓
Legal Mapping
↓
Element Analysis
↓
Compare
↓
Trend Analysis
↓
Case Map
↓
Exam / Practice Notes
↓
Knowledge Base Update

## Workflow

### Step 1 — Intake
- ระบุเลขคำพิพากษาและปี
- ระบุหัวข้อกฎหมายและข้อเท็จจริง
- ตรวจว่าภาพหรือข้อความถูกตัดหรือไม่

### Step 2 — Verification
- ตรวจเลขคำพิพากษาและปี
- ตรวจฐานความผิดและมาตรา
- ระบุว่าเป็นฉบับเต็ม บทคัดย่อ หรือการอ้างต่อกัน
- บันทึกแหล่งและระดับความน่าเชื่อถือ

### Step 3 — Extraction
แยกข้อเท็จจริงที่ศาลรับฟัง ข้อโต้แย้ง ประเด็นกฎหมาย เหตุผลศาล ผลคำพิพากษา และหลักกฎหมาย

### Step 4 — Legal Mapping
- Related STOU Unit and topic
- ชื่อกฎหมาย มาตรา วรรค และอนุมาตรา
- องค์ประกอบภายนอกและภายใน
- ความสัมพันธ์ระหว่างการกระทำกับผล
- เหตุยกเว้นความผิดหรือโทษ
- ตัวการ ผู้ใช้ ผู้สนับสนุน
- กรรมเดียว หลายกรรม หรือบทเฉพาะ
- อายุความและวิธีพิจารณา

### Step 5 — Deka Analysis
สำหรับแต่ละฎีกาให้แสดง:
1. เลขและปี
2. สถานะการตรวจสอบ
3. Related STOU Unit
4. Relevant Law and statutory text source
5. Facts
6. Legal Issues
7. Court Reasoning
8. Holding
9. Legal Principle
10. Element Analysis
11. Current Applicability
12. Limitations
13. References

### Step 6 — Comparative Analysis
เปรียบเทียบข้อเท็จจริงร่วม จุดต่าง มาตรา หลักกฎหมาย เงื่อนไขผลคดี แนวเดิม แนวใหม่ และความสอดคล้องกับตัวบทปัจจุบัน

### Step 7 — Trend Analysis
แสดงแนวเดิม แนวใหม่ จุดเปลี่ยน เหตุผลที่เปลี่ยน ผลต่อการปรับบท และข้อควรระวังเมื่ออ้างฎีกาเก่า

### Step 8 — Case Map
จัดกลุ่มตามกฎหมาย ฐานความผิด มาตรา องค์ประกอบ ประเด็น ช่วงเวลา และแนวคำพิพากษา

## Deka Research Queue

สถานะ:
- Waiting for Research
- Researching
- Source Located
- Verified
- Compared
- Added to Knowledge Base

Queue Item:
- Deka Number / Year
- Topic
- Related STOU Unit
- Relevant Law
- Source Provided
- Verification Status
- Missing Sources
- Notes

## Deka Knowledge Base

├── Criminal Law
│   ├── General Principles
│   ├── Attempt
│   ├── Participation
│   ├── Defences
│   ├── Multiplicity
│   ├── Offences against Life
│   ├── Bodily Injury
│   ├── Liberty
│   ├── Property
│   ├── Sexual Offences
│   ├── Public Peace
│   └── Petty Offences
├── Criminal Procedure
├── Labour Law
├── Civil and Commercial Law
├── Constitutional and Administrative Law
└── Other Laws

## Deka Record Template

## ฎีกาที่ [เลข/ปี]
- Verification Status:
- Source Availability Report:
- Related STOU Unit / Topic:
- Relevant Law / Section:
- Statutory Text Source:
- Keywords:

### Facts
### Legal Issues
### Applicable Law
### Court Reasoning
### Holding
### Legal Principle
### Element Analysis
- Actus Reus:
- Mens Rea:
- Causation:
- Defence:
- Participation:
- Multiplicity:
### Comparative Notes
### Current Applicability
### Limitation / Prescription
### Exam Point
### Practice Point
### Limitations
### References

## Output Template

1. Source Availability Report
2. สถานะการตรวจสอบ
3. ข้อเท็จจริงและ Timeline
4. Related STOU Units
5. ตัวบทกฎหมายฉบับที่ใช้บังคับ
6. องค์ประกอบความผิด
7. เหตุผลและผลคำพิพากษา
8. หลักกฎหมาย
9. Comparative / Trend Analysis
10. Case Map
11. การประยุกต์ใช้
12. อายุความและวิธีพิจารณา
13. ข้อจำกัดและหลักฐานที่ต้องหาเพิ่ม

## Quality Assurance Checklist

- [ ] GitHub Skill loaded
- [ ] Source Registry loaded
- [ ] Google Drive Master Skill reviewed
- [ ] Related STOU Unit located and cited
- [ ] Official or verified statutory text located
- [ ] Applicable-law date checked
- [ ] Deka number and year verified
- [ ] Full text / digest / secondary source status stated
- [ ] Facts separated from opinion
- [ ] No invented statute or holding
- [ ] Elements analyzed
- [ ] Conflicting Deka checked
- [ ] Limitation checked
- [ ] Current applicability stated
- [ ] Limitations stated

## Change Log

### v2.1
- เพิ่ม Hybrid Legal Knowledge Architecture
- เพิ่ม Source Registry
- เพิ่ม Mandatory Step 0 — Source Resolution
- เพิ่ม Source Availability Report
- เพิ่ม Stop Rules
- บังคับเชื่อม Google Drive Master Skill, STOU Units และตัวบทก่อน Deka Engine
- เพิ่ม QA สำหรับการเชื่อมโยงแหล่งข้อมูลข้ามระบบ

### v2.0
- เพิ่ม Deka Engine, Research Queue, Knowledge Base, Comparative Analysis และ Trend Analysis
