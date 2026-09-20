---
name: legal-multi-domain-analysis
description: Analyze Thai legal issues across labour, civil, criminal, public and constitutional, intellectual property, procedure, evidence, limitation, remedies, and STOU-to-Thai-Bar study alignment using an internal-first, source-traceable, version-controlled, human-reviewed workflow.
version: 1.1.0
author: PhuminDecOKnoi
license: MIT
---

# Legal Multi-Domain Analysis Skill

## 1. Purpose

This skill is the legal master router for Thai legal study, case analysis, HR and compliance work, audit support, research, teaching, structured legal memoranda, and exam-oriented legal reasoning.

It now includes a **Thai Bar Alignment Protocol** for integrating เนติบัณฑิตไทย preparation into existing legal-study, mind-mapping, and visual-mockup workflows. Do **not** create or call a separate standalone `/SKILL neti/bar *` skill unless the user explicitly asks for a separate skill file. Treat Thai Bar preparation as a mode inside the existing legal master, legal mind-mapping, and legal mockup PNG workflows.

The skill does not replace qualified legal advice or a court's determination. High-risk outputs require human legal review.

## 2. Covered legal domains

The analysis router may invoke one or more of the following domains:

1. Labour law and labour relations
2. Civil and commercial law
3. Tort law
4. Property law
5. Criminal law
6. Criminal procedure and evidence
7. Public law
8. Constitutional law
9. Administrative-law issues where necessary
10. Intellectual property law
11. Civil procedure and remedies where necessary
12. Special statutes connected to the facts
13. Legal-study and exam-alignment workflows, including STOU LL.B. course/unit mapping to Thai Bar subjects

A single matter may require multiple domains. The system must identify the primary domain, supporting domains, procedural law, special law, and any study/exam alignment layer before reaching a conclusion.

## 3. Core philosophy

### 3.1 Internal knowledge first

Use sources in this order:

1. User instructions and files supplied for the current task
2. Relevant internal Skill Master files and project knowledge
3. Current official statutory text applicable on the material date
4. Subordinate legislation, notifications, regulations, and official registers
5. Constitutional or judicial decisions from the competent court
6. Supreme Court and specialist-court decisions
7. Official interpretations, guidance, and administrative materials
8. STOU course materials and user-provided study sources when the task is study/exam work
9. Thai Bar official materials when the task concerns เนติบัณฑิตไทย, including official announcements, Student guide, Q&A, lecture schedules, examination regulations, and official subject structure
10. Reliable academic commentary
11. General web sources, used cautiously and corroborated

Do not silently replace internal course doctrine or user-provided materials with external summaries.

### 3.2 Current law controls

Learning materials organize the analysis, but the law in force on the material date controls the legal conclusion. Judicial decisions interpret and apply the law. Academic sources explain, compare, and critique.

For exam-preparation work, distinguish:

- source-course doctrine;
- current statutory text;
- Thai Bar official requirement;
- exam-oriented issue spotting;
- memory aid or pedagogical simplification.

### 3.3 Evidence before conclusion

Distinguish clearly between:

- verified fact;
- allegation;
- inference;
- statutory text;
- judicial holding;
- academic explanation;
- legal analysis;
- recommendation;
- study strategy;
- exam-writing framework.

Do not present an inference as a fact or a source summary as a binding rule.

## 4. Master legal router

For every new matter, apply this sequence:

```text
Receive facts and user objective
→ Identify whether this is legal advice, study work, exam preparation, visual planning, or mixed work
→ Identify persons, acts, dates, documents, property, and institutions
→ Build timeline where facts matter
→ Identify primary legal relationship
→ Select primary domain
→ Select supporting domains
→ Identify procedural forum and remedy where relevant
→ Identify applicable law on the material date
→ Retrieve authoritative sources
→ Break each claim/offence/right into legal elements
→ Apply verified facts to each element
→ Test defences, exceptions, jurisdiction, standing, and limitation
→ Analyze evidence and burden of proof
→ Analyze remedies, penalties, and enforcement
→ If study/exam work, add Thai Bar Alignment where relevant
→ Check conflicts between legal domains and source layers
→ State conclusion, uncertainty, and further evidence required
→ Human legal review when required
```

## 5. Cross-domain issue matrix

### 5.1 Labour plus civil

Check whether the facts create contractual, tort, property, agency, unjust-enrichment, or damages issues in addition to employment rights.

### 5.2 Labour plus criminal

Check whether conduct may constitute fraud, embezzlement, theft, forgery, defamation, coercion, bodily harm, computer offences, or offences under special statutes. Do not treat internal disciplinary findings as proof of criminal guilt.

### 5.3 Labour plus public or constitutional law

Check state-employer status, public authority, statutory power, administrative procedure, equality, human dignity, due process, lawful limitation of rights, and available judicial review.

### 5.4 Labour plus intellectual property

Check ownership and permitted use of employee-created works, inventions, trade secrets, databases, software, trademarks, confidential know-how, and post-employment restrictions.

### 5.5 Civil plus criminal

A single act may create both civil liability and criminal exposure. Analyze each separately because legal elements, burden of proof, limitation periods, remedies, and procedural routes differ.

### 5.6 Public plus private law

Identify whether the disputed act is an exercise of public power, a private transaction, or a mixed act. Do not assume that every act by a state body is administrative, or that every contract with the state is purely private.

### 5.7 STOU study plus Thai Bar preparation

When the user studies a STOU law course or asks for mind mapping, mockup PNG, exam review, or Thai Bar preparation, connect the learning source to Thai Bar only as a support layer:

```text
STOU course/unit
→ Thai Bar subject mapping
→ Legal structure
→ Current statutes
→ Exam issues
→ Verified case/deka anchor where available
→ Exam-writing framework
→ Checklist / next action
```

Do not convert every answer into Thai Bar preparation. Apply this layer only when the user requests Thai Bar, เนติฯ, exam alignment, legal mockup for study, or when the course-to-Bar connection is materially useful.

## 6. Domain engines

### 6.1 Labour-law engine

Analyze employment status, employer-employee relationship, wages, working time, leave, welfare, dismissal, severance, disciplinary action, labour relations, discrimination, occupational safety, social security, provident funds, employee welfare funds, migrant labour, child labour, and related special laws.

### 6.2 Civil and commercial engine

Analyze legal act, contract, capacity, agency, obligation, breach, default, damages, set-off, guarantee, unjust enrichment, management of affairs without mandate, prescription, and available civil remedies.

### 6.3 Tort and property engine

Analyze unlawful act, intention or negligence, causation, damage, vicarious liability, defences, compensation, ownership, possession, registration, real rights, joint ownership, recovery of property, interference, and limitation.

### 6.4 Criminal-law engine

Analyze actus reus, causation, mens rea, attempt, principal, instigator, supporter, multiplicity of offences, justification, excuse, individual liability, penalty, complaint requirements, and limitation.

### 6.5 Public and constitutional engine

Analyze source of public power, legal authority, jurisdiction, procedure, public interest, equality, proportionality, rule of law, legal certainty, constitutional rights, checks and balances, constitutional review, and remedies.

### 6.6 Intellectual-property engine

Classify the subject matter before choosing the law. Analyze creation or registration of rights, ownership, transfer, licensing, scope, infringement, exceptions, civil and criminal liability, border or administrative measures, treaties, evidence, remedies, and limitation.

### 6.7 Procedure and evidence engine

Identify competent court or authority, standing, cause of action, complaint or filing requirements, burden and standard of proof, admissibility, documentary and electronic evidence, provisional measures, appeal, enforcement, and procedural limitation.

### 6.8 Thai Bar Alignment engine

Use this engine only as an integrated mode within existing legal-study outputs.

Required sequence:

1. Identify the STOU course code, unit, topic, or legal area.
2. Map to Thai Bar phase and subject group where supported by official Thai Bar material or the user's confirmed study baseline.
3. Identify whether the issue belongs to ภาคหนึ่ง or ภาคสอง, and whether it is primary or supporting.
4. Verify current statutory text before giving legal conclusions.
5. Build the legal structure as a rule tree or decision flow.
6. Identify Thai Bar-style issue spots, elements, exceptions, limitation, jurisdiction, evidence, and remedy concerns.
7. Add case/deka anchors only when verified from an official source, uploaded material, or a trusted legal database; otherwise mark as requiring verification.
8. Produce an exam-writing framework:

```text
ประเด็น
→ หลักกฎหมาย
→ องค์ประกอบ/เงื่อนไข
→ ปรับข้อเท็จจริง
→ ข้อยกเว้น/ข้อโต้แย้ง
→ สรุป
```

9. End with checklist and next action.

Do not include long admissions, fee tables, or administrative-registration details in legal issue analysis unless the user is planning Thai Bar registration or study logistics.

## 7. Thai Bar integration rules for existing workflows

### 7.1 Legal master output

When Thai Bar alignment is requested, add only the relevant block:

```text
## Thai Bar Alignment
- STOU course/unit:
- Thai Bar subject group:
- Priority:
- Legal structure:
- Current statutes to verify:
- Bar issues:
- Case/deka anchor:
- Exam-writing framework:
- Checklist / next action:
```

### 7.2 Legal mind-mapping output

Use this compact layer:

```text
STOU Unit
→ Thai Bar Subject
→ Legal Structure
→ Key Statutes
→ Bar Issues
→ Case/Deka Anchor
→ Exam Writing
→ Memory Key
→ Next Action
```

Keep maps readable. Split dense maps rather than forcing all details into one block.

### 7.3 Legal mockup PNG output

For visual work, add a small `Thai Bar Focus` block only when useful:

- Thai Bar subject;
- key statutory structure;
- issue-spotting trigger;
- exam-writing sequence;
- one memory cue or trap.

Avoid overcrowding images with registration logistics, fee tables, document lists, or long procedural instructions unless the image topic is specifically Thai Bar registration or planning.

### 7.4 Standalone skill avoidance

Remove or avoid unused lines that create a separate neti/bar skill. Preferred wording:

```text
Use Thai Bar Alignment Protocol inside the existing legal master, legal mind-mapping, and legal mockup PNG workflows.
```

Avoid wording such as:

```text
/SKILL neti/bar *
NETI_BAR_STOU_MASTER_SKILL.md
Create a separate Thai Bar skill
```

unless the user explicitly requests a standalone skill artifact.

## 8. Temporal and version control

Before applying a legal provision, identify:

- date or period of the event;
- date the legal relationship arose;
- date of damage or completion of the offence;
- date of discovery where relevant;
- date of complaint, claim, filing, prosecution, or administrative action;
- statute, constitutional text, regulation, or notification in force on that date;
- transitional provisions;
- amendments, repeal, and replacement provisions;
- later judgments that may alter interpretation.

If the material date is unknown and could change the result, ask for it or state an explicit assumption.

For Thai Bar and STOU planning, also identify the academic year, student guide version, official announcement date, and whether the user is still studying, graduated but waiting for proof, registered as a Thai Bar student, registered for examination, or preparing for oral examination.

## 9. Authoritative citation protocol

For each material legal rule:

1. State the full title of the law or decision.
2. State the section, paragraph, subsection, clause, or article.
3. Quote only the operative text needed, from an official or verified source.
4. State the effective version and relevant date.
5. Separate source text from analysis.
6. Identify the elements of the rule.
7. Apply each element to verified facts.
8. State missing evidence and uncertainty.
9. Never invent a provision, amendment, judgment number, penalty, or quotation.

Preferred source order:

1. Royal Gazette
2. Office of the Council of State
3. Constitutional Court, Supreme Court, Administrative Court, or competent specialist court
4. Competent ministry, regulator, registrar, or enforcement authority
5. Official Thai Bar materials for Thai Bar logistics and subject structure
6. Verified internal official-law files
7. STOU course materials for study structure and course doctrine
8. Reliable academic sources for explanation only

## 10. Limitation and prescription engine

Every case analysis must test limitation or prescription where it may affect rights, claims, complaints, prosecution, enforcement, or remedies.

Required questions:

- What event starts the period?
- Is the period substantive or procedural?
- Is there a discovery rule?
- Is a complaint required within a special period?
- Is the conduct continuing, repeated, or composed of multiple acts?
- Does a special statute override the general code?
- Has filing, prosecution, acknowledgment, interruption, suspension, or another event affected the period?
- Does each claim or offence have a different period?
- Does final judgment create a separate enforcement period?

State the limitation conclusion separately for each claim, offence, remedy, and party.

## 11. Conflict and hierarchy rules

When sources or legal domains conflict:

1. identify the conflict expressly;
2. compare legal hierarchy;
3. compare dates and transitional provisions;
4. compare jurisdiction and subject matter;
5. apply lex superior, lex specialis, and lex posterior only where legally appropriate;
6. distinguish substantive law from procedural law;
7. explain why one rule is preferred;
8. preserve unresolved uncertainty for human review.

For study work, also distinguish:

- current law from course text;
- course-unit explanation from exam-key answer;
- Thai Bar official rule from third-party study advice;
- verified case holding from memory cue.

## 12. Standard output

Default output is plain text unless the user orders another format.

Use this structure where relevant:

## Request and scope
## Source basis
## Verified facts
## Allegations and uncertainties
## Timeline
## Primary legal domain
## Supporting legal domains
## Legal issues
## Applicable law and effective date
## Authoritative statutory text
## Elements and application
## Rights and liabilities by person
## Defences and exceptions
## Jurisdiction and procedure
## Evidence and burden of proof
## Limitation / prescription
## Remedies, penalties, and enforcement
## Cross-domain interaction
## Thai Bar Alignment
## Conclusion
## Recommended action and evidence required
## Human-review note

Omit empty sections. Include `Thai Bar Alignment` only when the user requests it or when it is materially useful for a legal-study deliverable.

## 13. Human-review gate

Mandatory human legal review is required before using an output for:

- dismissal or serious disciplinary action;
- criminal complaint, prosecution, or defence strategy;
- litigation, settlement, or admission of liability;
- constitutional or administrative challenge;
- intellectual-property enforcement or licensing dispute;
- regulatory reporting;
- publication of allegations about identifiable persons;
- any high-impact decision involving rights, liberty, reputation, livelihood, or substantial financial exposure.

## 14. Quality assurance checklist

- [ ] User-provided and internal sources reviewed first
- [ ] Primary and supporting domains identified
- [ ] Material dates and applicable legal version identified
- [ ] Full law title and precise provision stated
- [ ] Source text separated from analysis
- [ ] Each element applied to verified facts
- [ ] Counterarguments and defences considered
- [ ] Procedure, evidence, and jurisdiction considered
- [ ] Limitation analyzed separately
- [ ] Remedies and enforcement identified
- [ ] Thai Bar Alignment added only when relevant
- [ ] STOU course material separated from Thai Bar official material
- [ ] Case/deka anchors verified or marked for verification
- [ ] No invented law, judgment, source, exam rule, fee, date, or fact
- [ ] Personal and confidential information minimized
- [ ] Human-review requirement stated

## 15. Google Drive source synthesis

This skill incorporates governance patterns observed in the user's internal legal Skill Masters, including:

- Criminal Law AI: element-by-element analysis, applicable-law date control, procedure, evidence, individual liability, and mandatory limitation analysis;
- Civil Tort and Property AI: separation of facts, law, application, conclusion, rights of all parties, remedies, evidence, and prescription;
- Public and Constitutional Law AI: power, authority, procedure, rights, proportionality, constitutionality, review, and remedy;
- Intellectual Property Law AI: subject-matter classification, creation or registration of rights, ownership, infringement, exceptions, multiple liability routes, procedure, and treaty status;
- Thai Bar/STOU preparation baseline: treat เนติบัณฑิตไทย preparation as an integrated alignment protocol inside existing legal-study skills, not a separate standalone skill by default.

The source files remain the controlling internal references for their respective domains. This cross-domain skill is a router and synthesis layer, not a replacement for those detailed Skill Masters.

## 16. Change control

- Version changes must be made on a `version-X.Y-*` branch.
- Do not modify `main` directly.
- Verify all changed files by readback.
- Open a draft pull request.
- Do not merge into `main` without explicit user approval.
- Update the changelog for every material change.
