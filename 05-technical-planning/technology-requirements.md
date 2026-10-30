# Module-Level Technical Requirements — Before Stack Selection

**Goal:** Identify what each module technically requires, then use RRL and official documentation to justify candidate technologies. No final stack yet.

| Module | Core technical requirement | Decisions to research |
|---|---|---|
| M1 Talent database | Relational records, search, duplicate detection, freshness/audit | Schema, indexing, full-text vs semantic search, retention |
| M2 Résumé processing | Secure upload, PDF/DOCX parsing, OCR fallback, NLP/rules, verification | Parsing tools, OCR, NER, taxonomy, accuracy testing |
| M3 Matching/DSS | Mandatory checks, ranking, explanations, human review | Rule-based, weighted scoring, TF-IDF, embeddings, hybrid; fairness |
| M4 Workflow | Application-specific stages, tasks, reminders, audit | State transitions, scheduling, notifications, concurrency |
| M5 Job requirements | Structured mandatory/preferred criteria, terminology normalization | Relational modeling, validation, skills vocabulary |
| M6 Applicant discovery | Secure profile/preferences, job browse/apply, shared recommendations | Web/mobile UX, account roles, recommendation reuse |

## Cross-cutting requirements
- Web/mobile clients and backend API.
- Role-based access and secure personal-data handling.
- Candidate master records separate from candidate-vacancy applications.
- File storage and extraction verification.
- Matching service shared across authorized user experiences.
- Explainability, auditability, data quality and evaluation.

## Evidence requirements
Academic literature supports methods/algorithms. Official product/library documentation supports specific APIs, compatibility and versions. Team capability and available budget support feasibility. If a source does not specify a framework or dataset, record **not reported**.

## Additional technical investigations required before stack selection

### A. Data availability and model feasibility
- Confirm whether AYUDA can supply enough **authorized**, de-identified candidate/job examples and **reliable relevance judgments** for training and evaluation.
- Distinguish pretrained inference, fine-tuning, and training from scratch. Supervised sentence-pair models such as SPBERT may require substantial labeled examples to adapt effectively.
- If data is limited, compare transparent rules, weighted scoring and TF-IDF baselines before promising trained deep models.
- Record dataset size, label provenance, class imbalance, access restrictions, compute and annotation effort as **unknown until verified**.

### B. Candidate availability, consent and rediscovery
Do **not** conflate these states:

| State | Meaning / design consideration |
|---|---|
| Available | Candidate currently confirms interest/availability |
| Accepted another offer | May be unavailable for the present opportunity; future contact rules must be verified |
| Availability unknown | Must be checked before treating candidate as available |
| Does not wish to be contacted | Contact preferences/restrictions must be respected |

Rules for transitions, expiry, consent and permissible recontact must come from AYUDA's answers and applicable law, not assumptions.

### C. Explanation comprehension evaluation
Besides clarity/usefulness/trust ratings, test whether users can correctly identify **why** a recommendation appeared, which mandatory criteria were not met, and which fields remain unverified. Prefer task-based comprehension checks alongside surveys.

### D. Security and Philippine privacy obligations
Investigate applicable **Philippine Data Privacy Act of 2012 (RA 10173)** and relevant National Privacy Commission guidance before implementation. Assess lawful basis/consent where appropriate, privacy notices, role-based access, minimization, retention, secure deletion, document access and auditability. These are research obligations, **not confirmed AYUDA policies**; obtain authorized organizational requirements.

## Cross-cutting feasibility checks (not yet confirmed AYUDA policy)

1. **Data availability:** Determine whether authorized candidate–job pairs and reliable recruiter relevance labels exist. Supervised models such as fine-tuned sentence-pair BERT may need substantial labeled examples; small datasets may favor transparent rules and simpler baselines. Do not assume training data availability.
2. **Candidate availability and contact preference:** Distinguish `available`, `accepted another offer`, `unknown`, and `does not wish to be contacted`. These are *conceptual states*, not approved AYUDA business rules. Ask how transitions, consent and rediscovery eligibility work.
3. **Explainability testing:** Test whether users can correctly identify why a match was suggested, which mandatory requirements are unmet and which information is unverified, in addition to clarity/usefulness ratings.
4. **Privacy/security:** Investigate applicable Philippine Data Privacy Act obligations, appropriate lawful basis, access restrictions, retention and secure deletion. These are research requirements, not assertions about AYUDA's current policies.
