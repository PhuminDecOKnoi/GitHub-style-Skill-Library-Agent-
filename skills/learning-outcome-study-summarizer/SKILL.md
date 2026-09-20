---
name: learning-outcome-study-summarizer
description: Summarize lessons, chapters, units, modules, textbooks, lecture notes, or course documents by using learning outcomes, source headings, questions, activities, exercises, and answer keys as the controlling framework. Use for lesson summaries, exam-review notes, outcome-aligned study notes, unit synthesis, case-law review, mind maps, professional 16:9 infographics, and integrated STOU-to-Thai-Bar alignment. Treat Thai Bar / เนติฯ alignment as a mode inside this existing study, mind-mapping, and infographic workflow, not as a separate skill by default.
version: 1.1.0
---

# Learning Outcome Study Summarizer

## Core rule

Build the summary from the source, not from general memory. Treat learning outcomes as the inclusion test, the original heading hierarchy as the organization map, and activities or assessment items as evidence of what the learner must understand or perform.

Paraphrase and compress. Do not reproduce an entire textbook. Quote only short wording when exact language is essential, such as a statutory element, definition, formula, or technical term.

For legal-study work, separate source content, current law, case-law anchors, exam-key rules, and study strategy. Do not invent statutes, case numbers, issue weights, official dates, fees, or examination conditions.

## Interaction contract

- Infer subject, scope, depth, language, and intended use when reasonably clear.
- Ask one concise blocking question only when the unit, source, or deliverable cannot be identified safely.
- Lead with the completed study result, not extraction or tool narration.
- Use the user's language by default and retain useful original technical terms.
- Adapt depth to the source; omit empty sections, repeated caveats, internal matrices, and implementation details.
- State uncertainty at the exact claim or source location.
- If the current request explicitly says `Mind Mapping`, `Infographic`, `Infographic 16:9`, `mockup png`, or an equivalent visual command, treat it as approval and create that visual immediately without asking again.
- If the current request asks only for a summary, do not begin visual planning or generation. Offer the visual follow-up after delivering the summary.
- Never claim a file, visual, citation check, or external update was completed unless actually produced or verified.
- Do not create or invoke a separate `/SKILL neti/bar *` workflow unless the user explicitly asks for a separate skill artifact.

## Request routing

- `summary`: apply the default output and selected depth.
- `exam review`: prioritize issue spotting, recall cues, distinctions, exceptions, activity-derived questions, and common traps.
- `case law`: emphasize source-contained case-law rules while preserving links to outcomes and source sections.
- `mind map`: create a concise hierarchy or decision flow after applying the interaction contract.
- `infographic` or `mockup png`: route the visual detail mode, prepare a verified content plan, split images when needed, and render professional `16:9` visuals after applying the interaction contract.
- `Thai Bar`, `เนติฯ`, `bar exam`, or `STOU-to-Bar`: add the Thai Bar Alignment layer inside the same output.
- `document`, `spreadsheet`, or `presentation`: use the relevant artifact workflow while preserving source and quality controls.
- `external update`: keep supplied-material content separate from current external law, research, or commentary and cite the external layer.

When routes are combined, produce the core summary once and add only requested secondary deliverables. Do not duplicate the same content in several formats.

## Thai Bar Alignment Protocol

Use this protocol only when the user requests Thai Bar / เนติฯ alignment, legal exam preparation, bar-exam visual mode, or a STOU course map to Thai Bar. It is an integrated layer, not a standalone skill.

### Alignment sequence

```text
STOU course/unit
→ Thai Bar subject mapping
→ legal structure
→ current statutes
→ exam issues
→ verified case/deka anchor where available
→ exam-writing framework
→ checklist / next action
```

### Required distinctions

Separate clearly between:

- STOU course content and unit structure;
- current statutory text and amendments;
- Thai Bar official materials and administrative requirements;
- exam-writing technique;
- memory cue, trap, or study approximation.

### Registration-status guardrail

When the task involves Thai Bar registration or examination logistics, identify the user's status before giving operational conclusions:

1. still studying STOU LL.B.;
2. graduated but waiting for official completion evidence such as มสธ.14 or degree certificate;
3. registered as a Thai Bar student;
4. registered for a written examination group;
5. passed written groups and preparing for oral examination.

For the user's current planning baseline, while still studying น.บ. มสธ., they may attend/listen to lectures in advance, including normal lectures and evening/online/replay options as a general learner, but cannot yet register as a Thai Bar student with examination rights until completion evidence is available.

### Priority STOU course map for Thai Bar preparation

Use the user's current baseline unless a newer source or user instruction supersedes it:

- 41214: persons, juristic acts, obligations;
- 41215: tort, property, real rights;
- 41216: criminal law;
- 41217: public and constitutional law;
- 41218: commercial and business law 1;
- 41311: family and succession;
- 41312: civil procedure;
- 41313: criminal procedure and evidence;
- 41314: commercial and business law 2;
- 41404: labour law;
- 41455: intellectual property;
- 41317: execution and bankruptcy;
- 41401: English for lawyers;
- 41454 / 41463: human rights, justice process, and court-system support where applicable;
- 41421: tax law where available.

### Exam-writing framework

For Thai Bar-aligned legal answers, use:

```text
ประเด็น
→ หลักกฎหมาย
→ องค์ประกอบ/เงื่อนไข
→ วินิจฉัยข้อเท็จจริง
→ ข้อยกเว้น/ข้อโต้แย้ง
→ สรุป
```

Do not over-expand exam-writing sections when the user only needs a compact mind map or visual.

## Source workflow

1. Identify the requested subject, unit or chapter, depth, and purpose. Wait if the user explicitly asks to select a unit later.
2. Identify every available source file in scope. Never silently summarize a different unit.
3. Extract a source map containing:
   - unit, chapter, section, and subsection headings;
   - unit-level and section-level outcomes or objectives;
   - introductory concepts and stated key ideas;
   - questions, activities, exercises, cases, and answer keys;
   - judicial decisions, including court, number, necessary facts, holding or legal principle, and source location;
   - definitions, rules, formulas, processes, exceptions, limitations, and identifiers.
4. If outcomes are absent, infer a provisional framework from headings, introduction, key ideas, activities, and assessment; label it as inferred.
5. Create an internal alignment matrix with one row per outcome: outcome, supporting sections, relevant activity, essential content, and learner performance. Show it only if requested or materially useful.
6. Summarize each outcome independently, then connect related outcomes into a coherent progression. Preserve useful source numbering.
7. Read `references/subject-adapters.md` and apply only the relevant subject adapter when available.
8. Check activities and answer keys. Integrate the tested principle without copying long model answers. Report conflicts instead of choosing silently.
9. For law sources, inspect the requested scope for judicial decisions and apply the case-law rules below. Do not add outside judgments unless requested.
10. For Thai Bar alignment, add official Thai Bar materials only when supplied, found in the user's project baseline, or explicitly requested through web/connector search; keep them separate from STOU source content.
11. Run content quality checks.
12. Apply the visual gate. For an approved infographic, complete the visual workflow and visual QA before delivery.

## Case-law rules for legal sources

For each relevant judgment in the supplied material, provide:

1. Court and decision number exactly as shown.
2. Short keyword identifying the controlling issue.
3. Only the facts necessary to understand the ruling.
4. Holding or legal principle, paraphrased unless a short exact phrase is essential.
5. Connection to the current section, outcome, provision, or disputed issue.
6. Source file and page, section, activity, or answer-key identifier when available.

Group judgments beneath the topic they illuminate. Synthesize shared rules and note materially different facts, conditions, or outcomes.

Distinguish explicitly between source content, concise summary, and reasoned connection to the topic. Never infer a missing number, year, party, fact, holding, provision, or quotation. Mark unclear text and its location. Do not present commentary, headnotes, or the textbook author's explanation as the court's exact words.

For Thai Bar alignment, label unverified judgment anchors as `ต้องตรวจสอบต้นฉบับ/แหล่งทางการก่อนใช้อ้างอิงจริง`.

## Inclusion test

Include content when it directly explains an outcome; defines a required concept; supplies an element, condition, sequence, mechanism, exception, limitation, consequence, or application; supports an activity or assessment; distinguishes likely confusions; or preserves a necessary verification reference.

Exclude repeated exposition, decorative history, tangential commentary, and examples adding no distinct principle. Retain the smallest example needed to clarify application, calculation, interpretation, or a common error.

## Source discipline

- Distinguish explicit source content from inference and outside knowledge.
- Do not invent missing sections, answers, citations, statutes, formulas, data, or conclusions.
- Preserve technical meaning and exact section, activity, statute, clause, theorem, formula, figure, and judgment identifiers.
- Digit-check every displayed judgment and legal identifier against the source.
- Mark uncertain scan text with its page or section instead of guessing.
- For long files, process the requested unit in logical page ranges and reconcile heading continuity.
- Use supplied materials only unless external research is requested. Separate and cite supplemental findings.
- For current law or Thai Bar administrative information that may change, verify from an official current source when the user asks for operative planning.

## Default study output

Use plain text with minimal formatting unless the user requests another format.

1. ชื่อวิชา/หน่วยหรือบท
2. ผลลัพธ์การเรียนรู้
3. สาระสำคัญตามผลลัพธ์การเรียนรู้และหัวข้อย่อย
4. หลักการ องค์ประกอบ เงื่อนไข ขั้นตอน ข้อยกเว้น หรือข้อจำกัด
5. ประเด็นจากกิจกรรม/แบบฝึกหัดและแนวตอบ
6. คำพิพากษา/แนวคำวินิจฉัยในเอกสาร: เลขคดี คำสำคัญ ข้อเท็จจริงและหลักโดยย่อ ความเชื่อมโยง และจุดอ้างอิง
7. Thai Bar Alignment เฉพาะเมื่อเกี่ยวข้อง
8. จุดที่มักสับสนหรือควรระวัง
9. ข้อสรุปสำหรับทบทวน
10. ขอบเขตหรือข้อจำกัดของเอกสาร หากมี

Omit empty sections. Use a table or diagram only when it materially improves comparison, sequence, hierarchy, or relationships.

## Depth modes

- `brief`: one compact synthesis per outcome plus points to remember.
- `standard` (default): cover every outcome, relevant subsection, activity principle, and major exception.
- `detailed`: add distinctions, reasoning chains, necessary examples, cross-links, and traceability.
- `exam review`: prioritize definitions, elements, comparison points, application steps, traps, and activity-derived questions.
- `Thai Bar / เนติฯ`: add STOU-to-Bar mapping, issue spotting, legal elements, statutory structure, case/deka anchors when verified, and exam-writing framework.

Do not add quizzes, flashcards, or new practice questions unless requested.

## Visual follow-up gate

Visuals are optional, not part of the default summary.

- When the current request explicitly includes a visual, proceed without reconfirmation.
- When the current request does not include a visual, deliver the summary first and ask whether the user wants: Mind Mapping; Infographic `16:9`; both; or no visual yet.
- Prior approvals and standing preferences do not authorize a new unit or visual batch unless the current request includes it.

For Mind Mapping, organize from outcomes and controlling issues; show governing rules, elements, conditions, exceptions, effects, procedures, judgments, memory keys, traps, and Thai Bar Alignment when requested or materially useful.

## Legal mind-mapping structure

When the request is legal mind mapping and Thai Bar alignment is relevant, use this compact layer:

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

Keep the map readable. Split overcrowded maps or move details to supporting notes.

## Infographic detail modes

Route explicit Thai or English equivalents to these modes:

- `compact` / `กระชับ`: one image showing overview, essential rules, and memory cues.
- `standard` / `มาตรฐาน` (default): one or two images covering major rules, distinctions, exceptions, and key authorities.
- `detailed` / `ละเอียด`: two to four images covering elements, conditions, exceptions, legal effects, applications, and source-contained judgments.
- `bar exam` / `เนติฯ`: two to four exam-focused images emphasizing answer structure, issue spotting, application sequence, common traps, controlling source authorities, and a small Thai Bar Focus block.

If the user specifies both depth and audience, combine them; for example, `ละเอียด | เนติฯ` uses detailed coverage organized for bar-exam recall and application.

## Automatic multi-image split

Split an infographic rather than shrinking text when one or more apply:

- more than five major content groups;
- several provisions, formulas, cases, or comparisons;
- the content contains general rules, elements, exceptions, legal effects, and applications together;
- readable Thai text cannot be maintained at `1920 x 1080 px`;
- planned text exceeds approximately 350-450 Thai words for one image.

For detailed or bar-exam mode, prefer this sequence when supported by the source:

1. Overview and unit structure.
2. Governing rules, elements, and conditions.
3. Exceptions, legal effects, and application sequence.
4. Judgments, exam traps, memory cues, and Thai Bar Focus.

Use fewer images when the source does not justify all four. Label multi-image sets consistently, such as `1/3`, `2/3`, `3/3`.

## Visual Content Contract

Before image generation, prepare and verify an internal plan containing:

- exact visual title and unit scope;
- intended learner and study purpose;
- selected detail mode and reasoned image count;
- learning outcomes covered by each image;
- headings, subheadings, and reading order;
- exact provisions, formulas, figures, or judgment numbers;
- emphasis points, comparisons, traps, and memory cues;
- short copy for each content box, normally one heading plus two to five concise lines;
- Thai Bar Focus block only when relevant;
- links between images in a multi-image set;
- source location for every high-risk identifier or claim.

Do not expose the internal plan unless requested. Do not send unchecked source text directly to image generation.

## Infographic rendering standard

- Render at PowerPoint widescreen `16:9`, preferably `1920 x 1080 px`.
- Use a clear Thai typographic hierarchy, high contrast, restrained professional colors, consistent icons, and generous spacing.
- Preserve exact provisions, formulas, figures, and judgment numbers.
- Prefer short paraphrases over dense paragraphs.
- Keep source-grounded content visually distinct from supplemental external research.
- Avoid decorative details that compete with legal or technical content.
- For Thai Bar review, prioritize statutory structure, elements, exceptions, consequences, issue-spotting steps, source-contained Supreme Court principles, memory cues, traps, and exam-writing flow.
- Avoid long Thai Bar registration logistics, fee tables, document lists, or administrative details unless the visual topic is specifically Thai Bar registration/planning.

## Two-pass visual QA

Complete both passes before delivery.

### Pass 1 - content accuracy

- Verify the title, unit, and scope.
- Verify every provision, formula, figure, and judgment number character by character.
- Confirm elements, conditions, exceptions, consequences, and sequence against the source.
- Confirm every visual claim appears in the approved content plan.
- Confirm Thai Bar Focus content is source-supported or explicitly marked as planning guidance.
- Confirm no outside statute, judgment, update, or commentary was added without request and visible separation.

### Pass 2 - visual quality

- Inspect the rendered image, not only the prompt or plan.
- Check Thai glyphs, spelling, missing characters, duplicated or truncated text, and punctuation.
- Check reading order, hierarchy, contrast, alignment, spacing, and consistent set numbering.
- Confirm `16:9` dimensions and practical readability on a normal screen.
- Regenerate or repair before delivery if a material content error, identifier error, malformed Thai text, overlap, truncation, or unreadable text remains.

## Benchmark protocol: course 41455

Use supplied files `41455-1.pdf` through `41455-15.pdf` as a benchmark set when available; they are test inputs, not bundled skill content.

Test at least five representative units:

1. a shorter or concept-led unit;
2. a unit with multi-layer legal rules;
3. a unit with several judgments;
4. a comparison-heavy unit;
5. a dense unit comparable to Unit 3.

For each test, record only when a quality report is requested: source scope, requested visual mode, planned versus produced image count, outcome and heading coverage, identifier checks, split-rule decision, and both QA pass results. Do not claim the benchmark passed unless the relevant source files were actually inspected and the requested outputs were produced or verified.

## Quality checks

Before delivery, verify:

- every stated outcome is addressed;
- every claim is source-supported or labeled as inference;
- relevant activities contributed their tested principle;
- every displayed judgment appears in the source, has been digit-checked, and is connected to the topic;
- headings and identifiers match the requested unit;
- current-law or Thai Bar information is verified when used for operative planning;
- Thai Bar Alignment is added only when relevant;
- no standalone neti/bar skill lines are added unless explicitly requested;
- no controlling condition, exception, limitation, or consequence was lost;
- examples are necessary and minimal;
- language remains readable and technically accurate;
- copyrighted source material was not excessively reproduced;
- visual authorization follows the current request;
- any approved visual follows its detail mode, split rules, Visual Content Contract, `16:9` standard, and two-pass QA.

## Response contract

Return a polished, ready-to-study result in this order: exact unit and source scope; outcome-aligned synthesis; controlling rules, distinctions, exceptions, applications, and authorities; Thai Bar Alignment if relevant; concise review cues and limitations; then the visual follow-up only when the current request did not already approve or reject a visual.

For long units, group under source hierarchy or deliver clearly labeled parts. Do not omit controlling content merely to fit one response or image.

Append a compact validation block only when the user requests a quality report. Show scope coverage, source grounding, identifier checks, visual authorization, selected visual mode, image split decision, both QA passes, Thai Bar alignment status, and external-research status.

## Invocation examples

- `$learning-outcome-study-summarizer สรุปหน่วยที่ 8 แบบมาตรฐาน`
- `$learning-outcome-study-summarizer สรุปหน่วยที่ 3 เพื่อเตรียมสอบเนติฯ แล้วถามฉันก่อนสร้างภาพ`
- `$learning-outcome-study-summarizer * Mind Mapping`
- `$learning-outcome-study-summarizer * Infographic 16:9`
- `$learning-outcome-study-summarizer * Infographic | กระชับ`
- `$learning-outcome-study-summarizer * Infographic 16:9 | ละเอียด`
- `$learning-outcome-study-summarizer * Infographic | เนติฯ`
- `$learning-outcome-study-summarizer 41214 หน่วยที่ 3 | Thai Bar Alignment`
- `$learning-outcome-study-summarizer summarize this science module in detailed mode`
