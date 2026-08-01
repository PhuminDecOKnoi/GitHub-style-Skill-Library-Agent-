---
name: legal-multi-domain-analysis
description: Analyze Thai legal issues across labour, civil, criminal, public and constitutional, intellectual property, procedure, evidence, limitation, and remedies using an internal-first, source-traceable, version-controlled, human-reviewed workflow.
version: 1.0.0
author: PhuminDecOKnoi
license: MIT
---

# Legal Multi-Domain Analysis Skill

## 1. Purpose

This skill expands the repository from labour-law precedent research into a multi-domain Thai legal analysis system. It is designed for legal study, case analysis, HR and compliance work, audit support, research, teaching, and structured legal memoranda.

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

A single matter may require multiple domains. The system must identify the primary domain, supporting domains, procedural law, and any special law before reaching a conclusion.

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
8. Reliable academic commentary
9. General web sources, used cautiously and corroborated

Do not silently replace internal course doctrine or user-provided materials with external summaries.

### 3.2 Current law controls

Learning materials organize the analysis, but the law in force on the material date controls the legal conclusion. Judicial decisions interpret and apply the law. Academic sources explain, compare, and critique.

### 3.3 Evidence before conclusion

Distinguish clearly between:

- verified fact;
- allegation;
- inference;
- statutory text;
- judicial holding;
- academic explanation;
- legal analysis;
- recommendation.

Do not present an inference as a fact or a source summary as a binding rule.

## 4. Master legal router

For every new matter, apply this sequence:

```text
Receive facts and user objective
→ Identify persons, acts, dates, documents, property, and institutions
→ Build timeline
→ Identify primary legal relationship
→ Select primary domain
→ Select supporting domains
→ Identify procedural forum and remedy
→ Identify applicable law on the material date
→ Retrieve authoritative sources
→ Break each claim/offence/right into legal elements
→ Apply verified facts to each element
→ Test defences, exceptions, jurisdiction, and standing
→ Analyze evidence and burden of proof
→ Analyze limitation/prescription
→ Analyze remedies, penalties, and enforcement
→ Check conflicts between legal domains
→ State conclusion, uncertainty, and further evidence required
→ Human legal review
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

## 7. Temporal and version control

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

## 8. Authoritative citation protocol

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
5. Verified internal official-law files
6. Reliable academic sources for explanation only

## 9. Limitation and prescription engine

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

## 10. Conflict and hierarchy rules

When sources or legal domains conflict:

1. identify the conflict expressly;
2. compare legal hierarchy;
3. compare dates and transitional provisions;
4. compare jurisdiction and subject matter;
5. apply lex superior, lex specialis, and lex posterior only where legally appropriate;
6. distinguish substantive law from procedural law;
7. explain why one rule is preferred;
8. preserve unresolved uncertainty for human review.

## 11. Standard output

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
## Conclusion
## Recommended action and evidence required
## Human-review note

## 12. Human-review gate

Mandatory human legal review is required before using an output for:

- dismissal or serious disciplinary action;
- criminal complaint, prosecution, or defence strategy;
- litigation, settlement, or admission of liability;
- constitutional or administrative challenge;
- intellectual-property enforcement or licensing dispute;
- regulatory reporting;
- publication of allegations about identifiable persons;
- any high-impact decision involving rights, liberty, reputation, livelihood, or substantial financial exposure.

## 13. Quality assurance checklist

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
- [ ] No invented law, judgment, source, or fact
- [ ] Personal and confidential information minimized
- [ ] Human-review requirement stated

## 14. Google Drive source synthesis

This skill incorporates governance patterns observed in the user's internal legal Skill Masters, including:

- Criminal Law AI: element-by-element analysis, applicable-law date control, procedure, evidence, individual liability, and mandatory limitation analysis;
- Civil Tort and Property AI: separation of facts, law, application, conclusion, rights of all parties, remedies, evidence, and prescription;
- Public and Constitutional Law AI: power, authority, procedure, rights, proportionality, constitutionality, review, and remedy;
- Intellectual Property Law AI: subject-matter classification, creation or registration of rights, ownership, infringement, exceptions, multiple liability routes, procedure, and treaty status.

The source files remain the controlling internal references for their respective domains. This cross-domain skill is a router and synthesis layer, not a replacement for those detailed Skill Masters.

## 15. Change control

- Version changes must be made on a `version-X.Y-*` branch.
- Do not modify `main` directly.
- Verify all changed files by readback.
- Open a draft pull request.
- Do not merge into `main` without explicit user approval.
- Update the changelog for every material change.
