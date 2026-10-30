# Current Proposed System Overview

**Current academic research direction:** Candidate-to-job matching and potential explainable DSS.  
**Confirmed client need:** Candidate rediscovery/reuse.  
**Status:** Proposed, not final.

## Intended value
Help AYUDA identify new and previously sourced candidates for active vacancies, compare candidate qualifications with structured requirements, explain relevant matches/gaps/unknowns, and retain recruiter control over screening and endorsement. Optionally allow applicants to compare jobs and authorized clients to review endorsed candidates, **only if validated**.

## Conceptual information flow
Existing client vacancy (M5) + new or rediscovered candidate (M1, optionally M6) -> résumé text processing and verified fields (M2) -> candidate-job matching and explanations (M3) -> human review -> recruitment tracking and follow-up (M4). M6 may use the same matching engine for applicant job discovery.

## Example
A client needs technical support personnel. Recruiters retrieve previously sourced candidates with troubleshooting experience; the system checks mandatory criteria, explains relevant skills and flags unknown availability. The recruiter contacts candidates before endorsement. A candidate may also be shown several suitable jobs with location/setup tradeoffs if applicant recommendations are approved.

## Constraints
No automated hiring/rejection; no unrestricted candidate database access for clients; no Apollo-like prospective-company discovery; no payroll; no finalized model or stack.
