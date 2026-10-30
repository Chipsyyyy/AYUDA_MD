# Preliminary Ishikawa / Fishbone Analyses

**Warning:** These are brainstorming diagrams, not validated causal models. Do not claim matching inaccuracy as established.

## Fishbone A — Candidate rediscovery
**Effect:** Difficulty efficiently retrieving/reusing previously sourced candidates.

| Category | Potential factor | Evidence status |
|---|---|---|
| Methods | Manual Gantt-chart/spreadsheet tracking | Client-supported |
| Technology | No dedicated ATS; several tools | Client-supported context; causality not measured |
| Data | Contact-entry errors; names missing from tracking list | Client-supported |
| Manpower | Recruiters manage multiple candidates/vacancies | Client-supported context; workload impact unmeasured |
| Measurement | Retrieval time and rediscovery success rate unknown | Pending |
| Environment | Varied client requirements | Known context; not confirmed as rediscovery cause |

## Fishbone B — Candidate-to-job matching
**Provisional effect:** Potential difficulty consistently identifying, comparing and recommending suitable candidates.

| Category | Hypothesis to test |
|---|---|
| Manpower | Time pressure or variation in recruiter judgments |
| Methods | Unstandardized matching criteria/comparisons |
| Technology | Lack of decision-support comparison tools |
| Data | Incomplete/old candidate records and varied vacancy descriptions |
| Measurement | No baseline for matching time or recommendation relevance |
| Environment | Changing client requirements and candidate availability |

**Validation step:** Ask AYUDA whether there is a matching decision problem at all. If decisions are accurate but slow, revise the effect to decision time/efficiency rather than accuracy.

## Visual evidence labels
The revised diagrams explicitly identify reported conditions, contextual factors, hypotheses and unknowns. A reported condition is not automatically a proven root cause. Original illustrative PNGs are retained only under `assets/legacy-unverified/` for historical reference; do not use them for defense.

## Cause-to-solution traceability (provisional)

| Potential cause/problem | Proposed system response | Validation status |
|---|---|---|
| Difficulty retrieving previously sourced candidates | Centralized search and rediscovery | **Problem client-reported; solution proposed** |
| Incorrect/inconsistent candidate information | Recruiter verification, structured profiles, normalization | **Partial client evidence; exact extent unmeasured** |
| Difficulty comparing candidates | Explainable matching and side-by-side comparison | **Problem not yet confirmed** |
| Outdated candidate availability | Freshness prompts and availability verification | **Specific operational rules pending** |
| Manual follow-up monitoring | Due-date reminders and prioritized task queue | **Client-reported follow-up issue; prioritization proposed** |

Keep the original fishbone category tables. Visual diagrams should be attached as **separate, labeled preliminary assets** and should not be treated as verified causal proof. No unsupported cause should be labeled confirmed.

## Revised visual diagrams

- [Candidate rediscovery — preliminary, evidence-labelled SVG](assets/candidate-rediscovery-preliminary.svg)
- [Candidate-to-job matching — preliminary, evidence-labelled SVG](assets/candidate-job-matching-preliminary.svg)

The **matching diagram** deliberately avoids claiming that AYUDA makes inaccurate matching decisions. Its provisional effect is: **Potential difficulties identifying, comparing and recommending suitable candidates**.

Both diagrams preserve six categories (Manpower, Methods, Technology, Data/Materials, Measurement, Environment). Revalidate all causal claims when AYUDA replies. SVG assets are editable source files and can be exported to PNG for slides.
