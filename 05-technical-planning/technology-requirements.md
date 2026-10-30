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
