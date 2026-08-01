---
name: learning-outcome-study-summarizer
description: Summarize lessons, chapters, units, modules, textbooks, lecture notes, or course documents for any subject by using learning outcomes or objectives, source headings, and questions, activities, exercises, and answer keys as the controlling framework. Use when the user asks for a lesson summary, exam-review notes, outcome-aligned study notes, a unit or chapter synthesis, key concepts, points to remember, or a summary grounded in an attached PDF, document, image, slide deck, or course material. Adapt the analysis to law, business and HR, social science, science, mathematics, language, technology, or practical subjects while preserving source accuracy and traceability. After a summary, support optional mind maps and professional 16:9 exam-review infographics, but always obtain the user's confirmation immediately before creating either visual.
---

# Learning Outcome Study Summarizer

## Core rule

Build the summary from the source, not from general memory. Treat learning outcomes as the inclusion test, the original heading hierarchy as the organization map, and activities or assessment items as evidence of what the learner must understand or perform.

Do not embed or reproduce an entire textbook. Paraphrase and compress. Quote only short wording when exact language is essential, such as a statutory element, definition, formula, or technical term.

## Built-in-style interaction contract

Behave like a native study workflow rather than a prompt template:

- infer the subject, requested scope, depth, language, and intended use from the current request and available files;
- begin work without asking follow-up questions when those choices are reasonably clear;
- ask one concise blocking question only when the unit, source, or requested deliverable cannot be identified safely;
- lead with the completed study result, not a narration of extraction or tool steps;
- use the user's language by default and retain original technical terms when they improve precision;
- adapt section depth to the source instead of forcing every heading into every response;
- omit empty sections, repeated caveats, internal matrices, and implementation details;
- state uncertainty at the exact claim or source location instead of weakening the whole answer with generic disclaimers;
- treat an explicit visual request in the current message as confirmation and do not ask again for that same deliverable;
- never claim a file, visual, citation check, or external update was completed unless it was actually produced or verified.

## Request routing

Route the request before drafting:

- `summary`: apply the default output and selected depth mode;
- `exam review`: prioritize issue spotting, recall cues, distinctions, exceptions, activity-derived questions, and common traps;
- `case law`: emphasize the case-law rules while preserving connection to outcomes and source sections;
- `mind map`: create a concise hierarchy or decision flow only after current-turn confirmation;
- `infographic`: prepare and render a professional `16:9` visual only after current-turn confirmation;
- `document`, `spreadsheet`, or `presentation`: use the relevant artifact workflow and preserve the same source and quality controls;
- `external update`: keep the supplied-material summary separate from current external law, research, or commentary and cite the external layer.

When a request combines routes, produce the core summary once and add only the requested secondary deliverable. Do not duplicate the same content in multiple forms.

## Workflow

1. Confirm the requested subject, unit or chapter, desired depth, and output purpose from the user's message. Ask only when the missing choice blocks accurate work. If the user says to wait for a unit number, wait.
2. Identify every available source file that belongs to the requested scope. Never silently summarize a different unit.
3. Extract the following source map before drafting:
   - unit, chapter, section, and subsection headings;
   - unit-level and section-level learning outcomes or objectives;
   - introductory concepts or stated key ideas;
   - questions, activities, exercises, cases, and answer keys;
   - judicial decisions or case authorities, including court, decision number, key wording, facts, holding or legal principle, and the section or topic in which each decision appears;
   - definitions, rules, formulas, processes, exceptions, limitations, and source references.
4. If outcomes are absent, infer a provisional framework from the title, headings, introduction, stated key ideas, activities, and end-of-unit assessment. Label this as an inferred framework.
5. Create an internal alignment matrix with one row per learning outcome: outcome, supporting sections, relevant activity, essential content, and learner performance. Use it to decide inclusion; show it only if requested or materially useful.
6. Summarize each outcome independently, then connect related outcomes into a coherent progression. Preserve the source's hierarchy and numbering where useful for traceability.
7. Read the applicable adapter in [references/subject-adapters.md](references/subject-adapters.md) and apply only the relevant subject pattern.
8. Check every activity and answer key. Integrate the principle being assessed; do not copy a long model answer. If an answer conflicts with surrounding text, report the discrepancy instead of choosing silently.
9. For a law source, inspect the requested scope for cited Supreme Court judgments or other judicial decisions. When present, connect each decision to the nearest relevant legal issue or topic and summarize it under the case-law rules below. Do not add outside judgments unless the user requests external research.
10. Run the quality checks below before responding.
11. After delivering the summary, apply the visual follow-up gate below. Never create a mind map or infographic automatically.

## Case-law rules for legal sources

For each judgment that appears in the supplied material and is relevant to the requested scope, provide:

1. Court and decision number exactly as shown in the source, such as `คำพิพากษาศาลฎีกาที่ .../...`.
2. Short keyword or key phrase that identifies the controlling issue.
3. Concise facts necessary to understand the ruling.
4. Holding or legal principle, paraphrased unless a short exact phrase is essential.
5. Connection to the current section, learning outcome, statutory provision, or disputed issue.
6. Traceability reference: source file and page, section, activity, or answer-key identifier when available.

Group judgments beneath the topic they illuminate rather than listing them without context. If several judgments establish the same principle, synthesize the shared rule and then note any materially different facts, conditions, or outcomes.

Distinguish the following explicitly:

- `ถ้อยคำ/สาระที่ปรากฏในเอกสาร`: source-grounded wording or principle;
- `สรุปโดยย่อ`: compressed account of facts and holding;
- `ความเชื่อมโยงกับหัวข้อ`: reasoned explanation of relevance.

Never infer a missing decision number, year, party, fact, holding, statutory section, or quotation. Mark unclear text and its location. Do not present commentary, a headnote, or the textbook author's explanation as the court's exact words. If no judgment appears in the requested scope, state this briefly only when case law was requested or expected.

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
- Preserve judicial decision numbers exactly as printed and verify every digit against the source before delivery.
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
6. คำพิพากษาศาลฎีกา/แนวคำวินิจฉัยที่ปรากฏในเอกสาร: เลขฎีกา คำสำคัญ ข้อเท็จจริงและหลักวินิจฉัยโดยย่อ ความเชื่อมโยงกับหัวข้อ และจุดอ้างอิงกลับไปยังแหล่งที่มา
7. จุดที่มักสับสนหรือควรระวัง
8. ข้อสรุปสำหรับทบทวน
9. ขอบเขตหรือข้อจำกัดของเอกสาร หากมี

Omit empty sections. Use a table or diagram only when it materially improves comparison, sequence, hierarchy, or relationships.

## Response contract

Return a polished, ready-to-study answer with this priority order:

1. identify the exact unit or chapter and source scope;
2. present the outcome-aligned synthesis;
3. surface controlling rules, distinctions, exceptions, applications, and source authorities;
4. close with concise review cues, traps, or limitations that materially affect understanding;
5. ask the visual follow-up question only when the current request did not already approve or reject a visual.

For long units, preserve completeness by grouping content under the source hierarchy or by delivering clearly labeled parts. Do not compress prose into unreadable blocks or omit controlling content merely to fit one response or one image.

For a user-requested quality report, append a compact validation block showing scope coverage, source grounding, identifier checks, visual authorization status, and external-research status. Do not append this block by default.

## Visual follow-up gate

Treat mind maps and infographics as optional follow-up deliverables, not part of the default summary.

After completing a summary, ask whether the user wants one of the following:

1. Mind Mapping for structured exam review;
2. Infographic image in PowerPoint widescreen ratio `16:9`;
3. both Mind Mapping and Infographic; or
4. no visual yet.

Do not begin visual planning, rendering, image generation, or file creation until the user confirms the desired option in that turn. A standing preference, prior approval, attached source, or request to summarize does not count as confirmation to create a visual. Ask again for each new unit, chapter, or visual batch unless the user's current message explicitly requests the visual.

If the user confirms a Mind Mapping output:

- organize from the unit's learning outcomes and controlling legal issues;
- show hierarchy among governing law, provisions, elements, conditions, exceptions, legal effects, procedure, and judgments;
- emphasize recall cues, comparisons, issue-spotting sequences, and common exam traps;
- keep each branch concise and traceable to the supplied source;
- split an overcrowded map into multiple maps rather than shrinking text excessively.

If the user confirms an Infographic output:

- create a professional exam-review image at `16:9`, preferably `1920 x 1080 px`, suitable for a PowerPoint slide;
- use a clear Thai typographic hierarchy, strong contrast, restrained professional colors, consistent icons, and generous spacing;
- design for Thai Bar Examination review when that is the user's stated purpose: prioritize statutory structure, elements, exceptions, legal consequences, issue-spotting steps, Supreme Court principles found in the source, memory cues, and common traps;
- preserve exact provision and judgment numbers and avoid decorative details that compete with legal content;
- use multiple images when one slide would become dense or unreadable;
- verify Thai text, legal identifiers, visual hierarchy, legibility, and source fidelity before delivery.

For both formats, do not add external statutes, judgments, or legal updates unless separately requested. If external research is requested, distinguish it visibly from source-derived content.

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
- every displayed judicial decision appears in the source, its decision number has been digit-checked, and its relevance to the topic is explained;
- heading and identifier references match the requested unit;
- no important condition, exception, limitation, or consequence was removed by compression;
- examples are necessary and minimal;
- language is readable without weakening technical accuracy;
- the summary does not replace the source through excessive reproduction.
- no mind map or infographic was created without the user's current confirmation;
- any confirmed visual preserves the source hierarchy, exact legal identifiers, legibility, and the requested `16:9` format.

## Invocation examples

- `$learning-outcome-study-summarizer สรุปหน่วยที่ 8 แบบมาตรฐาน`
- `$learning-outcome-study-summarizer สรุปบทที่ 3 เพื่อเตรียมสอบ โดยยึดผลลัพธ์การเรียนรู้`
- `$learning-outcome-study-summarizer สรุปตามหัวข้อย่อยและกิจกรรมท้ายบท พร้อมจุดที่มักสับสน`
- `$learning-outcome-study-summarizer สรุปหน่วยที่ 1 เพื่อเตรียมสอบเนติฯ แล้วถามฉันก่อนสร้าง Mind Mapping หรือ Infographic 16:9`
- `$learning-outcome-study-summarizer summarize this science module in detailed mode`
