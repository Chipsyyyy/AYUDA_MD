# Conceptual Architecture — Provisional

```text
Recruiter/Admin Web UI         Optional Applicant/Client UI
            \                       /
             \                     /
              Backend API + Authentication/RBAC
                 |        |         |
        Candidate Data  Job Data  Application/Workflow Data
                 \       |        /
                 Matching & Explanation Service
                         |
             Verified Profile / Requirements
                         ^
                Resume Processing Service
                         |
                Secure Document Storage
```

## Key design boundaries
- One candidate master record; separate application/endorsement record per vacancy.
- Verified fields and provenance feed matching; unknowns are not automatic failures.
- Client-company users (if approved) see only authorized vacancies and endorsed records.
- Recruiters retain endorsement decisions; clients retain hiring decisions.
- Web and mobile access the same authorized backend and consistent data.
- Specific technologies, hosting and model deployment remain undecided.

## Possible workflow sequence
Vacancy entered -> candidate sourced/rediscovered -> résumé processed and verified -> criteria evaluated -> explained suggestions -> recruiter review -> application stage/follow-up history.
