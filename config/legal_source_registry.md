# Legal Source Registry

## Version
1.0

## Purpose
ทะเบียนแหล่งความรู้กลางสำหรับเชื่อม GitHub Workflow กับ Google Drive, STOU 41216, ตัวบทกฎหมาย และฐานคำพิพากษา

> Registry นี้เป็น Logical and Retrieval Map ไม่ใช่การเชื่อมข้อมูลอัตโนมัติ ผู้ปฏิบัติต้องเรียกค้นผ่าน connector จริงและบันทึกสถานะทุกครั้ง

## Source Records

### SOURCE-CRIMINAL-MASTER
- Provider: Google Drive
- Title: `stou_41216_criminal_law_ai_master_v4_1.md`
- Scope: SKILL MASTER – Criminal Law AI; Units 1–15 operating framework
- Authority Level: Internal Master
- Retrieval: Search exact title in Google Drive, then fetch content before legal analysis
- Currency Rule: Confirm latest version and modified date; do not assume v4.1 remains latest
- Fallback: Current verified Criminal Law Master skill in Google Drive

### SOURCE-STOU-41216
- Provider: Google Drive / Internal Files
- Title Pattern: `41216-[unit].indd`, `41216`, `all.docx`, or verified unit files
- Scope: STOU Course 41216 Units 1–15
- Authority Level: Academic Core
- Retrieval: Search by unit number, topic, section, and offence name
- Citation Rule: Identify unit, topic, and exact supporting passage
- Currency Rule: Preserve the edition used; distinguish academic explanation from current statutory text
- Fallback: User-uploaded STOU files in the current conversation or File Library

### SOURCE-PENAL-CODE
- Provider: Google Drive / Official Government Source
- Title: ประมวลกฎหมายอาญา
- Scope: Penal Code sections, paragraphs, subsections, amendments, effective dates
- Authority Level: Primary Statutory Law
- Retrieval: Internal verified statute first; otherwise Royal Gazette or Office of the Council of State
- Currency Rule: Verify version effective on the offence date and separately state current text
- Stop Rule: Do not quote from memory when no verified text is available

### SOURCE-CRIMINAL-PROCEDURE
- Provider: Google Drive / Official Government Source
- Title: ประมวลกฎหมายวิธีพิจารณาความอาญา
- Scope: Complaint, investigation, prosecution, evidence, appeal, limitation-related procedure
- Authority Level: Primary Statutory Law
- Retrieval: Internal verified statute first; then official source
- Currency Rule: Verify effective version

### SOURCE-SPECIAL-LAWS
- Provider: Google Drive / Official Government Source
- Scope: Special criminal, labour, safety, technology, data, human-rights, and regulatory laws
- Authority Level: Primary Statutory Law
- Retrieval: Search exact law title and relevant section
- Currency Rule: Verify amendments and subordinate legislation

### SOURCE-DEKA-INTERNAL
- Provider: Google Drive / GitHub Deka Knowledge Base
- Scope: Verified Supreme Court judgments, digests, case maps, research queue
- Authority Level: Case Law Support
- Retrieval: Search internal sources before external search
- Verification Rule: Mark Full Text, Digest, Secondary Citation, or Not Found
- Stop Rule: Unverified case numbers remain in Research Queue

### SOURCE-DEKA-ENGINE
- Provider: GitHub
- Repository: `PhuminDecOKnoi/GitHub-style-Skill-Library-Agent-`
- Path: `skills/legal/deka/skill_legal_deka_case_research.md`
- Scope: Workflow, verification, comparison, trend analysis, case mapping
- Authority Level: Operating Procedure
- Retrieval: Load from `main` unless the user explicitly requests a development branch

## Unit Mapping — STOU 41216

- Unit 1: Scope and foundational criminal-law concepts
- Unit 2: Criminal liability, elements, causation
- Unit 3: Attempt and related general principles
- Unit 4: Justification, excuse, mitigation
- Unit 5: Principal, instigator, supporter
- Unit 6: Punishment, multiple offences, recidivism, limitation
- Unit 7: Security offences
- Unit 8: Administration and justice offences
- Unit 9: Religion, public peace, trade, forgery
- Unit 10: Offences against life and body
- Unit 11: Sexual offences, abortion, abandonment
- Unit 12: Liberty and reputation
- Unit 13: Property offences (1)
- Unit 14: Property offences (2), including trespass
- Unit 15: Corpse offences and petty offences

## Source Resolution Checklist

- [ ] GitHub skill loaded
- [ ] Registry loaded
- [ ] Master skill located
- [ ] Relevant STOU unit located
- [ ] Relevant statutory text located
- [ ] Effective date checked
- [ ] Internal Deka searched
- [ ] External verification completed if needed
- [ ] Source Availability Report produced

## Maintenance Rules

1. Update titles or paths when a source is renamed or replaced.
2. Do not store invented file IDs or temporary response URIs as permanent identifiers.
3. Prefer stable titles, repository paths, and official law names.
4. Record deprecated sources and their replacements.
5. Review this registry whenever the Master Skill, STOU corpus, or statutory-law repository changes.
