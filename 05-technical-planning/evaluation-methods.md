# Potential Evaluation Methods — Not Finalized

| Component | Candidate measures | Caution |
|---|---|---|
| Matching/ranking | Precision@K, Recall@K, NDCG@K, recruiter-rated relevance | Requires valid labeled examples and explicit relevance criteria |
| Eligibility | Rule correctness, mandatory-criterion handling | Unknown must differ from confirmed noncompliance |
| Explainability | Clarity, usefulness, understanding, appropriate trust | Need structured user evaluation |
| Rediscovery | Retrieval time, relevant previously sourced candidates found | Establish current-process baseline |
| Résumé extraction | Field precision/recall/F1, correction rate, encoding time | Vary by résumé format; use authorized test data |
| Follow-ups | On-time action completion, overdue actions | External client reply speed not under AYUDA control |
| System | Functional tests, usability, RBAC/security checks | Test only with authorized or synthetic data |

No target performance values have been approved. Evaluation design depends on available data and client/professor review.

## Task-based explanation evaluation
In addition to subjective ratings, ask users to correctly identify (1) the verified factors behind a recommendation, (2) unmet mandatory criteria, (3) unverified/unknown information, and (4) the consequences of changing a stated preference. Measure comprehension and errors; do not claim a method improves decisions without a suitable comparison and human evaluation.
