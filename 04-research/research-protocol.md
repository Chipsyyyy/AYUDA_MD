# Research Protocol — Methodology Only (No RRL Findings Yet)

This document defines **how** future RRL findings should be documented. It does **not** assert that the team has completed any study analyses. The research folder is included for protocol only.

## Nine-column literature matrix

| Column | What to extract |
|---|---|
| 1. Authors and year | Verified APA 7 bibliographic details, DOI or stable URL |
| 2. Research objective | Actual research problem/question |
| 3. Algorithm / model / methodology | What authors **implemented/evaluated** versus merely cited in related work |
| 4. Dataset | Source, size, labeling, population and limitations, if reported |
| 5. Evaluation metrics | Actual measures and protocols used |
| 6. Key findings | Precisely reported results, baselines and qualifications |
| 7. Limitations / gap | Author-stated limitations versus team's own interpretation |
| 8. Relevance to AYUDA | Specific module, requirement and evidence status |
| 9. Implementation decision | Adopt, adapt, benchmark or exclude — **provisional** with rationale |

## Verification rules

- Read full text where possible; do not rely on abstracts for detailed algorithms or quantitative results.
- Verify author names, year, venue, DOI, title, tables and page references. Record exact page/section for claims.
- Do not invent datasets, scores, software libraries, versions, source code availability or reported limitations.
- Separate authors' findings from our inference and from client-specific assumptions.
- Do not transfer reported model accuracy to AYUDA without comparable data and evaluation.
- Record whether a study reviews an algorithm or actually implements/tests it.
- Compare methods against feasible baselines and the team's constraints.

## Academic literature versus technology documentation

**Peer-reviewed RRL** can justify problem framing, algorithmic methods, reported evaluations and limitations. **Official library/framework documentation** can justify API availability, compatibility, licensing, version requirements and supported integration. Neither alone proves that a stack is optimal for AYUDA. Record engineering trade-offs separately.

## Research intake template

- File/link and citation verified:
- Reader and date:
- Source type and quality:
- Full nine-column matrix entry:
- Direct evidence pointers (page/table/section):
- Confirmed findings vs interpretation:
- AYUDA module(s):
- Open questions and stack implications:
- Review status: awaiting peer check / reviewed

**Status:** Level 1–3 member findings are pending and must be added later; no results are populated here.
