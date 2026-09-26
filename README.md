# Recruiter Copilot

An AI-assisted applicant-screening workspace that helps recruiting teams review candidates consistently while keeping final hiring decisions with humans.

> This repository contains the public product showcase. The application source code is maintained privately as part of a commercial product under development.

## Product demo

**[Watch the two-minute product demo →](https://youtu.be/-ypX2yC1uTY)**
[Download the original demonstration video](./assets/recruiter-copilot-demo.mp4)

> The demonstration uses synthetic candidate data and deterministic demo
> analysis. It demonstrates the workflow, not validated production-model accuracy.

The demonstration covers:

- Creating a job with structured requirements.
- Adding a candidate from a résumé.
- Queuing and processing an applicant analysis.
- Reviewing an AI-generated recommendation and fit score.
- Keeping the applicant pending until a recruiter makes a decision.
- Confirming or overriding the recommendation through a human review.

> The demonstration uses entirely synthetic candidate data and deterministic demo analysis. It demonstrates the product workflow and user experience—not validated production-model accuracy.

## The problem

Recruiters and placement teams may receive many résumés for a single opening. The first screening pass is repetitive, time-consuming, and difficult to perform consistently.

Important evidence can be missed, while decisions and their reasoning are often scattered between spreadsheets, inboxes, ATS notes, and individual recruiter judgement.

Recruiter Copilot is designed to make that first screening pass faster and more structured without allowing AI to make the final hiring decision.

## How it works

1. **Create a job**

   Define the role, responsibilities, experience requirements, and relevant skills.

2. **Add applicants**

   Add candidate information using résumé text or supported document uploads.

3. **Generate a recommendation**

   The analysis workflow examines the résumé against the canonical job description and produces a structured recommendation.

4. **Inspect the evidence**

   Recruiters can review the fit score, recommendation, relevant experience, matched skills, concerns, and missing evidence.

5. **Make a human decision**

   An AI recommendation does not automatically shortlist or reject a candidate. The applicant remains pending until a recruiter explicitly reviews the result.

6. **Preserve decision history**

   AI recommendations and human decisions are stored separately so that overrides and lifecycle changes remain traceable.

## Core product principles

### AI assists; recruiters decide

The system separates the AI recommendation from the human review status. A candidate recommended for shortlisting remains pending until a recruiter confirms that decision.

### Evidence over opaque scores

A score alone is not sufficient. Recommendations should be supported by résumé evidence, job requirements, identified strengths, and clearly stated gaps.

### No automatic final rejection

AI-generated rejection is advisory. Final rejection requires an explicit human decision.

### Tenant isolation

Jobs, applicants, members, decisions, and usage belong to an organization and are isolated from other organizations.

### Durable processing

Applicant analyses are processed through a durable background queue instead of relying on a long-running browser request.

### Auditable decisions

Important recruiter actions and lifecycle changes are designed to remain attributable and reviewable.

## Current capabilities

- Organization-based recruiter workspaces.
- Owner and recruiter roles.
- Recruiter invitations and membership management.
- Job creation and applicant management.
- PDF and DOCX résumé ingestion.
- Structured applicant analysis.
- Background analysis queue with retry-safe processing.
- Fit scores and evidence-focused recommendations.
- Independent AI recommendations and human review states.
- Applicant shortlisting and rejection workflows.
- Immutable decision history.
- Usage-credit accounting.
- Applicant summary export.
- Responsive web interface.
- Security-conscious authentication and session management.

## Intended users

Recruiter Copilot is being designed for:

- Placement companies.
- Recruitment agencies.
- Small internal recruiting teams.
- Recruiters handling repeated initial résumé screening.
- Organizations that require a human to remain accountable for hiring decisions.

## What is currently being validated

The current validation stage focuses on whether:

- Initial résumé screening is a sufficiently painful and frequent problem.
- Recruiters find the proposed workflow practical.
- The displayed evidence is sufficient to evaluate a recommendation.
- Human confirmation and override controls improve trust.
- Decision history is useful for internal review or client reporting.
- Placement teams are willing to participate in a controlled pilot.

Production model quality will be evaluated separately using labelled, synthetic or properly anonymized candidate datasets before accuracy claims are made.

## Privacy and responsible use

The public demonstration contains no real candidate information.

Recruiter Copilot is being designed around the following requirements:

- Candidate data must not be used casually for experimentation.
- Real résumé processing must use an appropriately governed API and data-retention policy.
- Sensitive data should be minimized and protected.
- AI recommendations must remain advisory.
- Recruiters must be able to inspect and override recommendations.
- Automated decisions should not be based on protected personal characteristics.
- Retention, anonymization, export, and controlled deletion policies must be defined before production deployment.

## Product status

Recruiter Copilot is currently an MVP undergoing product and workflow validation.

The application is not presented as a finished production service. Work still includes:

- Model-quality evaluation and regression testing.
- Controlled pilot testing with recruiting teams.
- Production billing and subscription management.
- Email delivery and account notifications.
- Data-retention and legal-deletion policies.
- Production monitoring, alerting, backups, and operational dashboards.
- Broader automated and end-to-end testing.
- Accessibility and usability validation.


## Source code

The source repository is private because Recruiter Copilot is being developed as a commercial product.

This public repository is intentionally limited to product documentation, demonstration media, screenshots, and validation material.
