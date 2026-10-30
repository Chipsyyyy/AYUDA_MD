# Six Proposed Modules — Working Functional Reference

**Not an approved specification.** Each module below includes user, workflow, inputs, outputs, example, and open technical requirements. Module 3 is the current main academic focus.

## M1 — Candidate Sourcing and Centralized Talent Database
- **Users:** Recruiters/management; applicants only through approved interfaces.
- **Functions:** Create/update profiles, search skills and experience, track availability, previous applications, sourcing history, duplicate candidates and profile freshness.
- **Inputs:** Verified candidate details, résumé-derived fields, sourcing notes, contact/availability timestamps.
- **Outputs:** Searchable reusable talent records; candidates flagged for reconfirmation.
- **Workflow:** Source or retrieve candidate -> inspect master profile/history -> verify current contact and interest -> consider for new vacancy.
- **Example:** An eight-month-old BPO profile resurfaces for a new opening; recruiter confirms current availability before using it.
- **Technical needs:** Relational schema, indexing/search, duplicate heuristics, freshness thresholds, audit trail and access control.

## M2 — Résumé Information Processing
- **Users:** Recruiters; applicants if intake is approved.
- **Functions:** PDF/DOCX upload, direct text extraction, OCR fallback for scanned files, field/skill extraction, normalization, human correction; optional endorsement template prefilling.
- **Inputs:** Résumé document, supported format, skill dictionaries/taxonomy.
- **Outputs:** Draft structured profile fields with verification status.
- **Workflow:** Upload -> detect readable text -> OCR if necessary -> identify fields -> normalize -> verify -> save.
- **Example:** 'MS Excel' maps to 'Microsoft Excel'; verified work history is reused in an endorsement draft.
- **Technical needs:** Document parsing, OCR, NLP/NER or rules, file security, validation and extraction accuracy testing.

## M3 — Candidate-to-Job Matching and Explainable DSS
- **Users:** Recruiters; applicants/clients if validated.
- **Functions:** Eligibility checks, matching/ranking, multi-option comparisons, clear explanation of matched, missing and unverified criteria, human review.
- **Inputs:** Verified candidate profile, structured vacancy requirements, candidate preferences, confirmed matching rules.
- **Outputs:** Candidate or job suggestions, reasons, gaps, unknowns and review actions.
- **Workflow:** Normalize inputs -> check mandatory requirements -> compare relevant attributes -> rank suitable alternatives -> explain -> human decision.
- **Example:** Candidate meets skills and experience but on-site availability is unknown; system explains this rather than rejecting them.
- **Technical needs:** Algorithm comparison (rules, multi-criteria, text/semantic, hybrid), explainability, relevance evaluation, fairness and privacy.
- **Status:** **Primary innovation research candidate**, not yet validated as an operational necessity.

## M4 — Visual Recruitment Workflow Monitoring
- **Users:** Recruiters and management.
- **Functions:** Application-specific stage tracking, notes, assignment, endorsement/feedback history, reminders and overdue priorities.
- **Inputs:** Candidate-vacancy applications, timestamps, stage changes, due dates, staff assignments.
- **Outputs:** Kanban/status view, follow-up queue, activity history.
- **Workflow:** Screen -> interview -> endorse -> await feedback -> coordinate offer; monitor due actions throughout.
- **Example:** An overdue feedback follow-up is shown ahead of a routine check-in due next week.
- **Technical needs:** State transitions, transactional updates, task scheduling, notifications and permissions.
- **Status:** Core supporting feature, not main novelty.

## M5 — Job Opening and Client Requirements Management
- **Users:** AYUDA recruiters; client representatives only if approved.
- **Functions:** Record vacancies for **existing clients**, distinguish mandatory/preferred requirements, normalize skills and job terminology, track opening status and assigned recruiters.
- **Inputs:** Job description, qualifications, location, work arrangement, vacancy count and approved requirements.
- **Outputs:** Structured job record suitable for M3 matching.
- **Workflow:** Receive requirement -> structure fields -> preserve original wording -> verify -> publish for authorized matching.
- **Example:** 'Customer Care' and 'Customer Service' map to a shared category when context supports equivalence.
- **Technical needs:** Relational schema, controlled vocabulary, validation, optional text extraction and audit trail.
- **Boundary:** Does not discover prospective B2B leads or scrape contact lists.

## M6 — Applicant-Facing Job Discovery
- **Users:** Applicants, if AYUDA and professor approve.
- **Functions:** Registration, profile/preferences, vacancy browsing, applications, explainable multi-job suggestions.
- **Inputs:** Candidate profile, verified skills, preferences, authorized vacancies.
- **Outputs:** Job recommendations and explanations; submitted applications.
- **Workflow:** Register -> provide qualifications/preferences -> browse/recommend -> compare -> apply -> recruiter reviews.
- **Example:** Applicant prefers hybrid work in Metro Manila; job suggestions explain setup and location tradeoffs.
- **Technical needs:** User accounts, mobile/web UX, shared matching service, secure data boundaries.
- **Status:** Optional/scope-controlled; not yet client-validated.

## Cross-module data rule
One reusable candidate profile can link to many applications, each with independent recruitment statuses and outcomes. Job recommendations are suggestions, never automatic hiring decisions.
