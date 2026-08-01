---
name: learning-outcome-study-summarizer
description: Summarize lessons, chapters, units, modules, textbooks, lecture notes, or course documents for any subject by using learning outcomes or objectives, source headings, and questions, activities, exercises, and answer keys as the controlling framework. Use when the user asks for a lesson summary, exam-review notes, outcome-aligned study notes, a unit or chapter synthesis, key concepts, points to remember, or a summary grounded in an attached PDF, document, image, slide deck, or course material. Adapt the analysis to law, business and HR, social science, science, mathematics, language, technology, or practical subjects while preserving source accuracy and traceability.
---

# Learning Outcome Study Summarizer

## Core rule

Build the summary from the source, not from general memory. Treat learning outcomes as the inclusion test, the original heading hierarchy as the organization map, and activities or assessment items as evidence of what the learner must understand or perform.

Do not embed or reproduce an entire textbook. Paraphrase and compress. Quote only short wording when exact language is essential, such as a statutory element, definition, formula, or technical term.

## Workflow

1. Confirm the requested subject, unit or chapter, desired depth, and output purpose from the user's message. Ask only when the missing choice blocks accurate work. If the user says to wait for a unit number, wait.
2. Identify every available source file that belongs to the requested scope. Never silently summarize a different unit.
3. Extract the following source map before drafting:
   - unit, chapter, section, and subsection headings;
   - unit-level and section-level learning outcomes or objectives;
   - introductory concepts or stated key ideas;
   - questions, activities, exercises, cases, and answer keys;
   - definitions, rules, formulas, processes, exceptions, limitations, and source references.
4. If outcomes are absent, infer a provisional framework from the title, headings, introduction, stated key ideas, activities, and end-of-unit assessment. Label this as an inferred framework.
5. Create an internal alignment matrix with one row per learning outcome: outcome, supporting sections, relevant activity, essential content, and learner performance. Use it to decide inclusion; show it only if requested or materially useful.
6. Summarize each outcome independently, then connect related outcomes into a coherent progression. Preserve the source's hierarchy and numbering where useful for traceability.
7. Read the applicable adapter in [references/subject-adapters.md](references/subject-adapters.md) and apply only the relevant subject pattern.
8. Check every activity and answer key. Integrate the principle being assessed; do not copy a long model answer. If an answer conflicts with surrounding text, report the discrepancy instead of choosing silently.
9. Run the quality checks below before responding.

## Inclusion test

Include content when it does at least one of the following:

- directly explains a learning outcome;
- defines a concept required by an outcome;
- supplies an element, condition, sequence, mechanism, exception, limitation, consequence, or application required to achieve an outcome;
- resolves or supports an activity, exercise, or assessment item;
- distinguishes concepts likely to be confused;
- preserves a source reference necessary for verification.

Exclude repeated exposition, decorative history, tangential commentary, and examples that add no distinct principle. Retain the smallest example needed when it clarifies application, calculation, interpretation, or a common error.

## Source discipline

- Distinguish explicit source content from inference or outside knowledge.
- Do not invent missing sections, answers, citations, statutes, formulas, data, or conclusions.
- Preserve technical meaning while rewriting into clear, compact sentences or phrases.
- Preserve exact section, activity, statute, clause, theorem, formula, or figure identifiers when present.
- When a scan or extraction is unclear, mark the uncertain term and page or section rather than guessing.
- When files are long, process the requested unit in logical page ranges and reconcile heading continuity before finalizing.
- Use only the supplied materials unless the user requests external research. If research is requested, separate source-derived summary from supplemental findings and cite the latter.

## Default output

Use plain text with minimal formatting unless the user asks for a table, mind map, infographic, document, spreadsheet, or presentation.

1. ชื่อวิชา/หน่วยหรือบท
2. ผลลัพธ์การเรียนรู้
3. สาระสำคัญตามผลลัพธ์การเรียนรู้และหัวข้อย่อย
4. หลักการ องค์ประกอบ เงื่อนไข ขั้นตอน ข้อยกเว้น หรือข้อจำกัด
5. ประเด็นจากกิจกรรม/แบบฝึกหัดและแนวตอบ
6. จุดที่มักสับสนหรือควรระวัง
7. ข้อสรุปสำหรับทบทวน
8. ขอบเขตหรือข้อจำกัดของเอกสาร หากมี

Omit empty sections. Use a table or diagram only when it materially improves comparison, sequence, hierarchy, or relationships.

## Depth modes

- `brief`: one compact synthesis per outcome plus points to remember.
- `standard` (default): cover every outcome, relevant subsection, activity principle, and major exception.
- `detailed`: add distinctions, reasoning chains, necessary examples, cross-links, and traceability references.
- `exam review`: prioritize definitions, elements, comparison points, application steps, common traps, and activity-derived questions.

If the user does not specify a mode, choose `standard`. Do not add quizzes, flashcards, or new practice questions unless requested.

## Quality checks

Before delivering, verify that:

- every stated learning outcome is addressed;
- every included claim is supported by the source or clearly labeled as inference;
- all relevant activities have contributed their tested principle;
- heading and identifier references match the requested unit;
- no important condition, exception, limitation, or consequence was removed by compression;
- examples are necessary and minimal;
- language is readable without weakening technical accuracy;
- the summary does not replace the source through excessive reproduction.

## Invocation examples

- `$learning-outcome-study-summarizer สรุปหน่วยที่ 8 แบบมาตรฐาน`
- `$learning-outcome-study-summarizer สรุปบทที่ 3 เพื่อเตรียมสอบ โดยยึดผลลัพธ์การเรียนรู้`
- `$learning-outcome-study-summarizer สรุปตามหัวข้อย่อยและกิจกรรมท้ายบท พร้อมจุดที่มักสับสน`
- `$learning-outcome-study-summarizer summarize this science module in detailed mode`
