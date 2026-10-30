# AYUDA SYSAD — Claude Plan Mode Trial

**Purpose:** Test Claude's Plan Mode for preliminary technical planning using the team's newly submitted Level 1–3 RRL analyses. This is a planning exercise for title defense, **not authorization to implement a system or finalize the stack**.

## Instructions to Claude

You are supporting the developer/technical lead of Team InterLink (FEU Institute of Technology) on a proposed web and mobile recruitment system for **AYUDA Business Management Solutions Inc.**

**First, read** `CLAUDE.md`, `README.md`, and the project Markdown documentation already in this workspace. Then read the three newly provided RRL documents (or their Markdown transcriptions):

- `AYUDA- RRL LVL1.pdf` — matching, explainable DSS, fairness, and human-in-the-loop methods (6 studies).
- `AYUDA- RRL LVL2.pdf` — résumé extraction, skills/requirements processing, and bidirectional recommendation (6 studies).
- `AYUDA- RRL LVL3.pdf` — candidate search, rediscovery, and recruitment workflows (3 studies).

If the PDFs are not in the workspace, **stop and request them** rather than inventing findings. Do not assume they were automatically migrated from another conversation.

## Current project context

- **Approved client:** AYUDA. The revised title, innovation, and system scope are **not yet academically approved**.
- **Main research direction:** Candidate-to-job matching with potential explainable decision support (DSS).
- **Confirmed operational priority:** Candidate rediscovery and reuse of previously sourced talent.
- **Pending validation:** Whether a DSS is actually needed, exact matching criteria, applicant-facing recommendations, direct client-company access, candidate availability rules, and access to usable training/evaluation data.
- **Human oversight:** Recruiters and authorized users make actual recruitment decisions. A matching score is not by itself meaningful decision support.
- **No premature novelty claims:** résumé parsing, candidate rediscovery, ranking, and basic explanations already exist elsewhere.

## The six proposed modules (working reference, not final scope)

| Module | Current function / selected enhancement |
|---|---|
| 1. Candidate Sourcing and Talent Database | Search/reuse profiles; flag contact, availability, or experience for re-verification (profile freshness). |
| 2. Résumé Processing | Extract PDF/DOCX text; OCR when necessary; NLP skill normalization; assist client-specific endorsement prefilling. |
| 3. Candidate-to-Job Matching | Eligibility rules, explainable match-gap analysis, potential candidate recommendations for active vacancies. |
| 4. Visual Recruitment Workflow | AYUDA recruitment stages, activity history, and rule-based follow-up priorities. |
| 5. Job Openings and Requirements | Record vacancies from existing clients and normalize equivalent job requirement terms. |
| 6. Applicant-Facing Job Discovery | Candidate profiles, preferences, applications, explainable job suggestions; **subject to approval**. |

## Trial task — use Plan Mode only

Create a **preliminary technical research and architecture plan** that helps the team prepare a defensible technology-stack proposal for its title defense. **Do not write application code, install packages, or choose a final stack.**

### Phase 1 — Evidence mapping

1. Map each of the 15 RRL analyses to relevant modules, algorithms/methods, and potential technical requirements.
2. Distinguish **methods the studies implemented**, methods they only reviewed, and **our own proposed adaptations**.
3. For every claim, cite the source PDF, study number, and page or section when possible. Mark source-level facts still requiring verification.
4. Flag inconsistencies in bibliographic details in a short *verification backlog*; **do not silently correct or replace them** during this trial.

### Phase 2 — Technical alternatives

Prepare a **module-by-module decision matrix** containing:

- Functional and non-functional requirement
- Candidate algorithm/model or ordinary software method
- Possible libraries, frameworks, databases, APIs, or tools
- Relevant RRL evidence versus official technology documentation needed
- Inputs, outputs, data volume and data quality requirements
- Infrastructure, integration, privacy and maintenance considerations
- Advantages, limitations, feasibility for a student team
- Decision status: **Research candidate / Pending client validation / Pending academic approval**

Investigate alternatives rather than declaring winners. Compare simpler baselines against more complex models, especially for Module 3. Do not assume that an academic paper's model is suitable for AYUDA just because its reported metrics are strong.

### Phase 3 — Coherent architecture options

Develop **two or three provisional end-to-end stack options** covering web, mobile, backend/API, database, document storage, search, résumé processing, matching, explanations, authentication, and hosting. Describe integration and trade-offs. Identify where the same matching service can support recruiter-facing and applicant-facing workflows if approved.

Separate **matching** (compatibility), **ranking** (ordering), **explainability** (reasons and evidence), **decision support** (comparing alternatives and trade-offs), and **human oversight** (final decisions).

### Phase 4 — Risks and validation gates

Explicitly assess:

- Whether AYUDA can supply authorized candidate/job records and reliable relevance judgments; implications for supervised learning and cold-start approaches.
- Candidate availability and contact permissions, including available, accepted another offer, unknown, and do-not-contact states (rules **not yet confirmed**).
- Explanation evaluation: can users correctly identify matched criteria, unmet requirements, and unverified information?
- Privacy and security: role-based access, limited client visibility, lawful processing, retention, and secure deletion; applicable Philippine obligations require further investigation.
- Which recommendations must wait for AYUDA's questionnaire answers or professor approval.

### Phase 5 — Plan Mode deliverables

Return the following **without creating implementation code**:

1. A concise current-state assessment.
2. A prioritized, dependency-aware technical research plan.
3. An RRL-to-module traceability matrix.
4. An initial algorithm/method comparison for Module 3.
5. A shortlist of coherent stack alternatives, each explicitly provisional.
6. A validation and evidence backlog.
7. Likely title-defense technical questions and what evidence would answer them.

For each technical recommendation use this format:

**Problem addressed | Supporting evidence | Module | Proposed approach | Alternatives | Data/infrastructure | Risks | Evaluation | Validation/approval status**

## Rules for this trial

- **Plan, don't build.** No code changes, project scaffolding, dependencies, deployments, or migrations.
- Don't invent AYUDA policies, statistics, client responses, or RRL results.
- Keep client-confirmed facts separate from professor recommendations, academic findings, team proposals, and assumptions.
- Preserve the six modules as a working reference, not a fixed final specification.
- Prefer clear comparisons and unresolved decisions over premature conclusions.
- **Do not update the project's source-of-truth Markdown files** during this trial. Present proposed changes for team review first.
- End with the next **three research decisions** the developer should prioritize, and explicitly identify which depend on new client answers.

**Start by stating what files you actually found and what evidence you can access. Then produce the plan.**
