# Security Policy

## Scope

This repository contains legal, HR, compliance, governance, and AI-agent knowledge assets. Security includes technical security, source integrity, privacy, confidentiality, and prevention of misleading high-risk output.

## Reporting a vulnerability

Do not disclose vulnerabilities, exposed credentials, confidential records, or sensitive personal data in a public issue.

Report privately to the repository maintainer through an appropriate private GitHub contact channel. Include:

- affected file, workflow, or component;
- impact and severity;
- reproduction steps without real confidential data;
- suggested remediation;
- whether credentials or personal data may have been exposed.

## Supported scope

Security maintenance applies to the current `main` branch and actively maintained content. Historical examples and deprecated materials may receive documentation warnings rather than full remediation.

## Secrets and credentials

Never commit API keys, passwords, tokens, cookies, private keys, production connection strings, or real `.env` files. Use placeholders and `.env.example` files only.

Immediately rotate any credential that may have been exposed. Removing a secret from the latest commit does not remove it from Git history.

## Personal and confidential data

Do not commit identifiable employee records, health information, disciplinary records, payroll data, legal correspondence, litigation strategy, witness details, or unredacted confidential documents.

Use anonymized or synthetic data and apply data minimization, purpose limitation, retention controls, and access restrictions.

## Legal-source integrity

High-risk legal output must:

- identify the source and access date;
- distinguish quotation, paraphrase, inference, and recommendation;
- avoid invented judgment numbers, statutory sections, or holdings;
- verify current law where the conclusion depends on legislative status;
- receive human legal review before operational use.

## AI and model risks

Treat model-generated output as unverified until reviewed. Key risks include hallucinated citations, outdated law, omitted exceptions, source conflation, prompt injection, and disclosure of confidential information to external providers.

Do not submit confidential data to an AI provider unless authorization, contractual controls, and data-governance requirements have been confirmed.

## Dependency and automation risks

GitHub Actions and third-party actions should be pinned to trusted versions where practical. Workflow changes require review for excessive permissions, untrusted input, secret exposure, and supply-chain risk.

Use least-privilege permissions and avoid running untrusted pull-request code with write credentials.

## Production-use warning

This repository is not, by itself, a production legal decision system. It must not autonomously determine dismissal, discipline, compensation, litigation, or regulatory outcomes.
