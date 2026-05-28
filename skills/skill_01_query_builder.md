# Skill 01: Labour Dika Query Builder

## Purpose
สร้างคำค้นภาษาไทยสำหรับค้นคำพิพากษาศาลฎีกาประเภทคดีแรงงาน

## Input
- ข้อเท็จจริงของผู้ใช้
- ประเด็นที่สงสัย
- กฎหมายที่เกี่ยวข้อง ถ้ามี
- คำศัพท์ HR ที่ผู้ใช้ใช้

## Process
1. Extract layperson terms.
2. Convert to legal terms.
3. Add statutory phrases.
4. Add consequence terms.
5. Add alternative synonyms.
6. Prioritize exact phrase search first.

## Query pattern

```text
[พฤติการณ์] + [ผลทางกฎหมาย] + [มาตรา/คำกฎหมาย]
```

## Example 1: ขาดงาน / ละทิ้งหน้าที่

User phrase:
> ลูกจ้างขาดงาน 3 วัน มีวันหยุดคั่น เลิกจ้างได้ไหม

Search terms:
- ละทิ้งหน้าที่ สามวันทำงานติดต่อกัน
- ขาดงานสามวัน วันหยุดคั่น
- ไม่มีเหตุอันสมควร ละทิ้งหน้าที่
- มาตรา 119 5 ละทิ้งหน้าที่
- เลิกจ้าง ไม่จ่ายค่าชดเชย ขาดงาน

## Example 2: OT / ค่าล่วงเวลา

User phrase:
> นายจ้างให้ทำงานก่อนเวลาแต่ไม่จ่ายโอที

Search terms:
- ค่าล่วงเวลา ก่อนเวลาทำงาน
- นายจ้างสั่งให้ทำงานล่วงเวลา
- ทำงานล่วงเวลาโดยปริยาย
- เวลาทำงาน ค่าล่วงเวลา พยานหลักฐาน
- ค่าล่วงเวลา ภาระการพิสูจน์

## Output
Return:
- Primary keywords
- Secondary keywords
- Legal terms
- Search strategy
