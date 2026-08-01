---
name: github-repository-professional-standard
description: Create, audit, modernize, and govern GitHub repositories using a professional standard covering README, licensing, security, contribution workflows, issue/PR templates, changelog, support policy, academic learning design, SEO/AI search, and repository-type-specific governance.
version: 1.0.0
author: PhuminDecOKnoi
license: MIT
---

# GitHub Repository Professional Standard Skill

## 1. Purpose

This skill defines a repeatable professional workflow for creating, auditing, modernizing, and maintaining GitHub repositories.

It applies to:

- software projects;
- learning repositories and courseware;
- API and AI prototypes;
- data, dashboard, HR, legal, and compliance projects;
- documentation-only repositories;
- personal portfolio repositories;
- experimental and legacy repositories.

The objective is not to add every possible file to every repository. The objective is to apply the correct governance depth for the repository type, risk, maturity, audience, and maintenance model.

## 2. Core Principles

### 2.1 Preserve First

Before modifying a repository:

1. inspect the existing README and governance files;
2. preserve professional content that is already correct;
3. avoid rewriting solely for stylistic consistency;
4. do not invent files, features, APIs, versions, licenses, tests, or deployment workflows;
5. do not remove historical context unless it is inaccurate, unsafe, obsolete, or explicitly requested.

### 2.2 Evidence Before Claim

Every statement in repository documentation must be supported by actual repository evidence, verified official documentation, or explicit user-provided information.

Do not claim production readiness, security compliance, successful tests, CI status, a specific license, supported versions, or feature completeness unless verified.

### 2.3 Minimum Necessary Governance

Use repository-type-specific governance. Do not add a full open-source governance package to a small private experiment unless there is a clear benefit.

### 2.4 Security and Privacy by Default

Never commit or expose API keys, access tokens, passwords, private keys, real `.env` values, personal data, confidential company data, production database dumps, payment information, authentication cookies, or internal credentials.

Use `.env.example`, placeholders, synthetic data, and anonymized examples.

### 2.5 Professional but Practical

Documentation should be accurate, concise, navigable, copy-paste ready, technically precise, easy to maintain, and suitable for GitHub search, web search, and AI-assisted discovery.

## 3. Repository Classification

### Type A — Flagship Open-Source Project

Recommended:

- `README.md`
- `LICENSE`
- `SECURITY.md`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `SUPPORT.md`
- `CHANGELOG.md`
- `.github/PULL_REQUEST_TEMPLATE.md`
- bug and feature issue templates
- CI workflows where justified
- release and versioning policy

### Type B — Professional Learning Repository

Recommended:

- `README.md`
- `LICENSE`
- `SECURITY.md`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `SUPPORT.md`
- `CHANGELOG.md`
- PR template
- content-error or bug template
- learning outcomes
- course structure
- prerequisites
- version policy
- exercises, labs, or projects
- references and citation policy

### Type C — Application Prototype or MVP

Recommended:

- `README.md`
- verified `LICENSE` when appropriate
- `SECURITY.md`
- `CONTRIBUTING.md` if collaboration is expected
- PR template if maintained collaboratively
- environment-variable guidance
- architecture overview
- deployment warning
- limitations and assumptions
- data and privacy controls

### Type D — Documentation or Knowledge Repository

Recommended:

- `README.md`
- source and citation policy
- verified `LICENSE` when applicable
- `CONTRIBUTING.md`
- `CHANGELOG.md`
- `SUPPORT.md` if public questions are expected
- content-error issue template
- human-review notice for high-risk topics

### Type E — Legacy or Small Experimental Repository

Recommended:

- accurate `README.md`
- verified license or neutral license wording
- status label: learning, legacy, archived, experimental, or reference
- setup instructions when possible
- modernization recommendations
- security warning for outdated patterns

Do not automatically add all community files.

### Type F — Profile Repository

Recommended:

- professional profile `README.md`
- expertise areas
- featured projects
- learning and professional themes
- approved contact channels
- no private personal information
- navigation to major repositories

## 4. Mandatory Audit Workflow

### Step 1 — Identify Metadata

Capture repository name, owner, visibility, default branch, description, topics, homepage, archived status, fork status, primary language, and license metadata.

### Step 2 — Inspect Core Files

Check:

- `README.md`
- `LICENSE`
- `.gitignore`
- package/dependency manifest
- project entry point
- source folders
- environment examples
- test files
- CI workflows
- Docker files
- configuration files
- documentation folder

### Step 3 — Inspect Governance Files

Check:

- `SECURITY.md`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `SUPPORT.md`
- `CHANGELOG.md`
- PR template
- issue templates
- funding configuration
- dependabot configuration
- code owners

### Step 4 — Classify Gaps

Each action must be classified as:

- **Required**
- **Recommended**
- **Optional**
- **Not applicable**

### Step 5 — Apply Preserve-First Changes

- update only verified gaps;
- keep established structure when professional;
- prefer additive changes;
- use focused commits;
- do not mix unrelated changes.

### Step 6 — Verify

After writing:

- fetch the changed file;
- confirm path and content;
- record commit SHA;
- ensure no duplicate file exists;
- ensure links and headings are coherent;
- ensure no secrets or unsupported claims were introduced.

## 5. Professional README Standard

Use sections where relevant:

1. Title
2. Summary
3. Verified badges
4. Project information table
5. Features or scope
6. Learning outcomes
7. Prerequisites
8. Verified repository structure
9. Installation and quick start
10. Environment variables
11. Testing and quality checks
12. Security
13. Limitations and assumptions
14. Roadmap or modernization path
15. References
16. Verified license
17. Search topics

### README Rules

- one clear H1;
- describe only implemented or documented capabilities;
- commands must match actual configuration;
- never show real secrets;
- list test commands only when verified;
- include limitations for prototypes and MVPs;
- never claim open source when no license is present.

## 6. License Standard

Before stating a license:

- inspect `LICENSE`, `LICENSE.md`, or `COPYING`;
- verify repository metadata;
- check third-party code or copied upstream content.

Use MIT only when authorized and compatible.

For forks or vendored projects, preserve the upstream license. Never replace Apache, GPL, BSD, or another upstream license with MIT.

For educational repositories, clarify that third-party images, datasets, book excerpts, and external course content may have separate restrictions.

## 7. Security Standard

`SECURITY.md` should cover:

- supported versions or maintenance scope;
- private vulnerability reporting;
- report details;
- secret management;
- data privacy;
- dependency risk;
- input validation;
- output encoding;
- authentication and authorization;
- database least privilege;
- file upload and path traversal where applicable;
- third-party API risk;
- production-use disclaimer where appropriate.

### Domain-Specific Additions

**Legal, HR, Compliance**
- human review;
- no automatic legal conclusion;
- source traceability;
- personal-data controls;
- access control;
- retention and export risk.

**AI and LLM**
- prompt and response privacy;
- API-key protection;
- model-output verification;
- hallucination and citation risk;
- provider/model variability;
- rate-limit and cost control.

**Database**
- parameterized queries;
- least privilege;
- backup and restore;
- migration review;
- destructive-query warnings;
- transaction and locking implications.

**Frontend**
- XSS prevention;
- safe URL handling;
- no client-side secrets;
- dependency/CDN review;
- accessible forms and user feedback.

## 8. Contributing Standard

`CONTRIBUTING.md` should explain:

- repository purpose;
- accepted contribution types;
- setup;
- coding or writing standards;
- branch and commit guidance;
- testing or validation requirements;
- documentation rules;
- security and privacy;
- copyright and license expectations;
- PR checklist.

For learning repositories, add:

- lesson structure;
- measurable learning objectives;
- code-comment expectations;
- beginner readability;
- references;
- version-review process.

## 9. Pull Request Template Standard

Include:

- summary;
- type of change;
- related issue;
- validation performed;
- documentation impact;
- security/privacy impact;
- backward compatibility;
- screenshots for UI changes;
- secret and personal-data checklist;
- license confirmation.

Add project-specific checks, such as:

- SQL tested on teaching baseline;
- TypeScript type-check passed;
- React accessibility reviewed;
- Excel sample data anonymized;
- API responses validated;
- legal conclusions human-reviewed.

## 10. Issue Template Standard

### Bug Report

Capture description, reproduction steps, expected behavior, actual behavior, environment, redacted logs, screenshots, affected version, and security/privacy impact.

### Feature Request

Capture problem, proposed solution, alternatives, audience, learning/business value, compatibility impact, and security/privacy considerations.

### Content Error

Recommended for learning and documentation repositories:

- affected file and section;
- incorrect text;
- proposed correction;
- supporting source;
- version/date;
- impact on code examples.

## 11. Changelog Standard

Use sections:

- Added
- Changed
- Deprecated
- Removed
- Fixed
- Security

Do not fabricate historical releases.

For the first changelog in an existing repository:

- label the current baseline;
- document only verified recent changes;
- use `Unreleased` for planned work.

## 12. Code of Conduct Standard

Require:

- respectful communication;
- constructive technical criticism;
- no harassment or discrimination;
- privacy protection;
- responsible disclosure;
- maintainer authority;
- consequences for repeated misconduct.

Do not claim external enforcement affiliations unless true.

## 13. Support Policy Standard

Separate:

- usage questions;
- bugs;
- features;
- security reports;
- academic questions;
- legal/compliance limitations.

State that support is best effort unless an SLA exists, security issues must not be public, and high-risk legal or production decisions require professional review.

## 14. Academic and Learning Standard

A professional course repository should include:

- course title;
- level;
- audience;
- prerequisites;
- learning outcomes;
- module or weekly plan;
- estimated study time;
- guided examples;
- labs or exercises;
- capstone or mini project;
- common mistakes;
- checkpoints;
- references;
- version policy;
- instructor notes where relevant.

Teaching rules:

- plain language before jargon;
- retain necessary English technical terms;
- explain why, not only what;
- distinguish legacy and modern patterns;
- avoid copyrighted reproduction;
- use original examples;
- cite official documentation and research.

## 15. SEO and AI Search Standard

Use semantic headings and natural phrases for:

- technology;
- audience;
- use case;
- project type;
- skill level;
- domain;
- version;
- learning outcome.

Good practices:

- clear H1;
- descriptive opening paragraph;
- meaningful headings;
- consistent terminology;
- concise metadata table;
- verified topics;
- cross-repository links;
- FAQ only when useful.

Avoid keyword stuffing, misleading badges, unsupported marketing claims, unrelated topics, and filler.

## 16. Naming Standard

Prefer lowercase kebab-case for new repositories when practical.

Examples:

- `nodejs-learning-path`
- `typescript-react-api-ai`
- `labour-compliance-dashboard`

Preserve established names when renaming would break links or history unless explicitly authorized.

File naming:

- conventional root files in uppercase;
- lowercase kebab-case for lesson and documentation files;
- avoid spaces and ambiguous abbreviations.

## 17. Commit Standard

Use focused commit messages:

```text
docs: modernize repository README
docs: add security policy
docs: add contribution guide
chore: add pull request template
docs: add repository governance files
fix: correct broken documentation links
```

Do not combine unrelated changes when avoidable.

Always retain commit SHA for reporting.

## 18. Repository Quality Scoring

| Dimension | Weight |
|---|---:|
| README accuracy and usability | 20 |
| License clarity | 10 |
| Security and privacy | 15 |
| Contribution workflow | 10 |
| Documentation structure | 10 |
| Testing and quality evidence | 10 |
| Version and dependency policy | 10 |
| Accessibility and UX | 5 |
| SEO and AI discovery | 5 |
| Maintenance and changelog | 5 |

Score bands:

- 90–100: Gold Standard
- 80–89: Professional
- 70–79: Usable with improvements
- 50–69: Legacy or incomplete
- below 50: High-priority remediation

Do not award points for generic or inaccurate files.

## 19. Decision Matrix

| Condition | Action |
|---|---|
| README absent | Create verified README |
| README placeholder | Rewrite professionally |
| README professional | Preserve and patch gaps |
| License absent | Do not claim open source |
| Upstream license exists | Preserve upstream license |
| Security-sensitive app | Add/improve `SECURITY.md` |
| Public learning repo | Add contribution and content-error process |
| Small private experiment | Keep governance lightweight |
| Legacy dependencies | Add warning and modernization path |
| Legal/HR content | Add traceability and human review |
| AI/API project | Add key hygiene, privacy, output verification |

## 20. Completion Checklist

### Repository Audit

- [ ] Repository type classified
- [ ] Core files inspected
- [ ] Existing professional content preserved
- [ ] License verified
- [ ] Security risks identified
- [ ] Unsupported claims avoided

### README

- [ ] Clear title and summary
- [ ] Verified features and structure
- [ ] Correct setup commands
- [ ] Safe environment-variable documentation
- [ ] Audience and status stated
- [ ] Limitations included where relevant
- [ ] License statement verified

### Governance

- [ ] `SECURITY.md` appropriate to risk
- [ ] `CONTRIBUTING.md` appropriate to collaboration
- [ ] PR template appropriate to project
- [ ] Issue templates appropriate to users
- [ ] `CHANGELOG.md` contains no invented history
- [ ] Support and conduct files added only when useful

### Quality

- [ ] No secrets
- [ ] No personal/confidential data
- [ ] No invented tests or CI claims
- [ ] No broken links introduced
- [ ] Changes verified by readback
- [ ] Commit SHAs recorded
- [ ] Final report separates changed, preserved, deferred items

## 21. Standard Execution Prompt

```text
Audit and modernize the target GitHub repository using the
GitHub Repository Professional Standard Skill.

Requirements:
1. Inspect the repository before making changes.
2. Classify the repository type.
3. Preserve professional existing content.
4. Verify all features, commands, versions, and license claims.
5. Add only governance files appropriate to repository type and risk.
6. Apply security, privacy, academic, SEO, and AI-search standards where relevant.
7. Do not invent repository files or capabilities.
8. Make focused commits.
9. Verify every write by readback.
10. Report changed files, preserved files, commit SHAs, risks, and remaining recommendations.
```

## 22. Output Format

### Repository Assessment

- Repository:
- Type:
- Maturity:
- Risk level:
- Current strengths:
- Priority gaps:

### Changes Applied

| File | Action | Purpose | Commit SHA |
|---|---|---|---|

### Preserved Files

List files retained and explain why.

### Risks or Limitations

List evidence-based risks only.

### Remaining Recommendations

Classify as Required, Recommended, or Optional.

## 23. Governance Philosophy

A professional repository is not measured by the number of files it contains.

It is measured by accuracy, maintainability, traceability, security, usability, learning value, collaboration readiness, and honest documentation.

> Add what the repository needs, preserve what already works, verify every claim, and avoid governance theater.
