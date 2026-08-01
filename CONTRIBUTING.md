# Contributing Guide

Thank you for helping improve the Labour Dika Agent Skill Library.

## Accepted contributions

- new or improved agent skills;
- corrections to legal citations or source metadata;
- taxonomy and legal-register improvements;
- case-brief, search-log, precedent-table, and memo templates;
- anonymized examples;
- documentation and governance improvements;
- quality, accessibility, and automation enhancements.

## Before contributing

1. Search existing issues and pull requests.
2. Confirm that the contribution fits the repository purpose.
3. Remove personal, confidential, privileged, and production data.
4. Verify that third-party content may legally be included.
5. Use official or reliable sources for legal propositions.

## Branch and commit guidance

Use a focused branch name such as:

```text
feature/add-dismissal-taxonomy
fix/correct-case-citation
docs/improve-review-checklist
```

Use focused Conventional Commit-style messages:

```text
docs: improve legal memo template
fix: correct judgment source metadata
feat: add precedent comparison skill
chore: add markdown validation workflow
```

## Writing standard

- Use clear Thai for legal analysis.
- Retain English technical terminology where it improves precision.
- Use one clear H1 per Markdown document.
- Keep headings semantic and navigable.
- Define the purpose, inputs, outputs, workflow, limitations, and review requirements of each skill.
- Do not claim a capability that the repository does not implement.

## Legal-source standard

A legal contribution should record, where available:

- judgment number and court;
- date;
- material facts;
- issue;
- holding or legal principle;
- applicable statute and section;
- source reference and access date;
- analytical limitations;
- human-review status.

Clearly distinguish direct source content from paraphrase, inference, recommendation, and model-generated text.

## Skill-file standard

A professional skill should contain:

1. name and purpose;
2. scope and exclusions;
3. expected inputs;
4. required source hierarchy;
5. step-by-step workflow;
6. output schema;
7. validation checklist;
8. legal, privacy, and copyright guardrails;
9. version or change information when material.

## Privacy and security

Never include:

- API keys or tokens;
- real employee records;
- medical, payroll, or disciplinary data;
- confidential legal documents;
- production database exports;
- authentication cookies;
- personal contact details without authorization.

Security issues must be reported privately under `SECURITY.md`.

## Copyright and licensing

Contributors confirm that they have the right to submit their work under the repository's MIT License. Third-party judgments, statutes, articles, books, images, and datasets retain their own legal status and must not be reproduced beyond lawful limits.

## Pull request checklist

- [ ] Scope is focused and explained.
- [ ] Sources and citations are traceable.
- [ ] No secrets or personal data are included.
- [ ] Copyright and license implications were checked.
- [ ] Links and Markdown structure were reviewed.
- [ ] Legal conclusions are marked for human review.
- [ ] `CHANGELOG.md` was updated for material changes.
- [ ] Existing terminology and file contracts remain compatible, or migration guidance is provided.

## Review expectations

Maintainers may request changes for accuracy, source quality, privacy, security, copyright, structure, or repository-scope alignment. Acceptance does not constitute legal endorsement of the contributed analysis.
