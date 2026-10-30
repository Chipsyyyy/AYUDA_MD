# AYUDA — Level 3 RRL: Candidate Rediscovery and Recruitment Workflow

> **Source:** Team-submitted `AYUDA- RRL LVL3.pdf`.
> **Status:** Team research findings received; individual citations, metrics, and bibliographic details are not yet independently verified against original publications.
> **Scope:** Faithful searchable text extraction of the entire team-submitted PDF, preserving page boundaries. Embedded diagrams and figures remain in the original PDF; inspect that PDF for figures.
> **Important:** Do not treat the studies as final technology decisions or treat findings from external datasets as AYUDA-specific performance.

## Source PDF page 1

```text
Level 3 — Supporting recruitment-management research

Assigned member: Sam · Three studies

These papers are intended to justify Modules 1 and 4, particularly candidate search, rediscovery, and
workflow management. Sam does not need to identify a new AI algorithm for each standard module.

RRL 13 — Searching for Talent: The Information Retrieval Challenges of Recruitment
Professionals

Russell-Rose & Chamberlain · Business Information Review · 2016

This study examines how recruitment professionals search for candidates, formulate and refine search
queries, and assess results.

Tony Russell-Rose, Jon Chamberlain, 2016

What Sam should investigate: Search criteria, retrieval difficulties, query refinement, candidate
availability, and the importance of up-to-date candidate information.

AYUDA relevance: Supports the candidate rediscovery module and the need for searchable, reusable
talent records.

Read RRL 13

     Searching for Talent: The Information Retrieval Challenges of Recruitment Professionals

 Author(s) and Year       Russell-Rose, T., & Chamberlain, J. (2016). Searching for talent: The
                          information retrieval challenges of recruitment professionals. Business
                          Information Review. https://doi.org/10.1177/0266382116631849. The
                          uploaded author manuscript does not specify the final volume, issue, or page
                          range.

 Research Objective
                          To investigate the information-seeking behavior, search strategies, query
```

## Source PDF page 2

```text
formulation techniques, result evaluation practices, and search-system
                         requirements of recruitment professionals. The study addresses the limited
                         understanding of recruiters' complex information retrieval needs and how
                         existing search tools support their candidate sourcing activities.


Algorithm / Model
                         Survey-based Information Retrieval (IR) analysis. The researchers conducted
                         a 40-question online questionnaire covering recruiter demographics, search
                         tasks, query formulation, result evaluation, and ideal search-system features.
                         They examined the use of Boolean queries, synonyms, query expansion,
                         filtering, and relevance ranking. The paper also discussed attribute-based
                         searching and search-by-example as potential improvements, but did not
                         implement or evaluate these as new algorithms.

Dataset
                         The study analyzed 64 valid responses from recruitment professionals
                         collected between June 9 and August 1, 2015. The survey initially received
                         416 responses, of which 69 were complete; five were excluded because of
                         contradictory or nonsensical answers. Respondents were recruited through
                         professional social media groups and SurveyMonkey Audience's North
                         American HR panel. The survey contained 40 questions across five sections.


Evaluation Metrics
                         The study used descriptive survey statistics, including response percentages,
                         medians, and weighted average scores on five-point Likert scales.
                         Measurements included search task duration, number of queries submitted,
                         query formulation time, time spent assessing results, frequency of search
                         criteria, and perceived importance of search features. It did not report
                         machine-learning metrics such as accuracy, precision, recall, F1-score, or
                         NDCG.


Key Findings
                         Candidate search was reported by 76% of respondents, while 52% used
                         proprietary internal databases. The median candidate search task took 3 hours,
                         involved 5 queries, and required 5 minutes per query to formulate. Boolean
                         logic (4.25/5), synonyms (4.16/5), and query expansion (4.02/5) were highly
                         valued. Recruiters primarily filtered results by job function (4.34/5) and
                         location (4.29/5). The recency of retrieved candidate information received the
                         highest search-management importance score (4.21/5). The study also found
                         that recruiters frequently refined searches and evaluated results until they
                         identified a sufficient number of suitable candidates.


Limitations / Research
Gap                      The study relied on a relatively small sample of 64 recruiters and self-reported
                         survey responses, which may not fully represent actual search behavior. The
                         authors acknowledged possible demographic and recruitment-method biases.
                         Since the number of professionals reached was unknown, the survey
                         participation rate could not be calculated. The study did not implement or
                         experimentally compare proposed search improvements, nor did it evaluate
                         candidate retrieval accuracy or operational efficiency using actual
                         recruitment-system logs.


Relevance to AYUDA
                         The study directly supports AYUDA's proposed candidate search and
                         rediscovery module by identifying practical recruitment search challenges. Its
                         findings provide a basis for searchable candidate records, structured filters for
                         job function and location, synonym-aware search, reusable search criteria, and
                         relevance-based candidate ranking. The emphasis on information recency also
                         supports tracking when candidate profiles and availability were last verified,
                         helping recruiters assess whether previously stored candidates remain suitable
                         for new vacancies.
```

## Source PDF page 3

```text
Implement Decision
                           Adapt. AYUDA should adapt the study's user-centered information retrieval
                           principles by providing structured candidate search, relevant filters, reusable
                           searches, and indicators of candidate-information recency. Synonym
                           expansion and search-by-example can be considered for further evaluation.
                           The study should be used as a requirements and workflow-design reference,
                           rather than a benchmark for machine-learning performance, because it does
                           not present a tested matching algorithm.


 Synthesis
                           Russell-Rose and Chamberlain (2016) investigated the information retrieval
                           challenges experienced by recruitment professionals through a survey of 64
                           respondents. The study found that candidate sourcing involves complex and
                           iterative search processes, with recruiters relying on Boolean queries,
                           synonyms, query expansion, and multiple information sources to identify
                           suitable candidates. Results showed that a typical search task required a
                           median of three hours and five queries, while job function, location, and the
                           recency of candidate information were important factors in evaluating search
                           results. The researchers also identified limitations in existing recruitment
                           search tools, particularly their support for query formulation and refinement.

                           The study provides a practical foundation for AYUDA's proposed candidate
                           search and rediscovery module by emphasizing the need for efficient retrieval
                           of existing candidate records. Its findings support structured search filters,
                           reusable search criteria, synonym-aware retrieval, and indicators of candidate
                           information recency. However, the study relied on self-reported survey data
                           and did not experimentally evaluate an improved retrieval system. Therefore,
                           AYUDA can adapt its user-centered search principles while validating the
                           proposed features against the client's actual recruitment workflow and
                           candidate database.




RRL 14 — Understanding Recruiters' Information Seeking Behavior in Talent Search

Kaya & Bogers · ACM CHIIR · 2023

This paper investigates recruiter search behavior and the ways recruiters formulate, refine, and evaluate
searches during talent sourcing.

ir.webis.de+1

What Sam should investigate: Search sessions, information retrieval methods, filtering, recruiter
workload, and how recommendations could be incorporated into the existing workflow.

AYUDA relevance: Helps justify integrating candidate rediscovery and matching recommendations into a
recruiter-controlled search process.

Read RRL 14


                Understanding Recruiters’ Information Seeking Behavior inTalent Search

 Author(s) and Year        Kaya, M., & Bogers, T. (2023). Understanding recruiters’ information

                                   seeking behavior in talent search. Conference on Human

                                   Information Interaction and Retrieval, 14–23.

                                   https://doi.org/10.1145/3576840.3578311

                           Kaya and Bogers (2023)
```

## Source PDF page 4

```text
Research Objective
                     The study investigated recruiters' information-seeking behavior, focusing on
                     search sessions, query refinement, filtering practices, and candidate
                     evaluation. It examined how search behavior changes across recruitment tasks
                     and how search characteristics relate to candidate response rates.


Algorithm / Model




                     Figure 1: The interface of the CV search engine. Personal information has
                     been masked. The interface consists of four main components: (1) the search
                     bars, which allow for keyword search, location-based search, and search for
                     job titles and job categories; the regular (2) and advanced (3) filter panes; and
                     (4) the search results, which contain teaser representations for each CV.
                     Matching terms are automatically highlighted in yellow in the CV teasers in
                     the results list.

Dataset
                     The study analyzed recruiter search logs from Jobindex, a Danish recruitment
                     platform, covering September 2016 to November 2021. The original dataset
                     contained 157,046 search tasks and approximately five million queries. After
                     filtering, 128,133 sessions containing approximately four million queries
                     remained, consisting of 92,020 matching tasks and 36,113 recruiting tasks.


Evaluation Metrics
                     The researchers measured session duration, query count, query length, term
                     diversity, advanced search operator usage, and recruitment-specific filter
                     usage. Positive candidate response rate was used as a proxy for search
                     success. ANOVA, Tukey's HSD tests, effect sizes, correlation analysis, and an
                     independent-samples t-test were used to examine differences and relationships
```

## Source PDF page 5

```text
in the recorded data.


Key Findings
               The study found that matching sessions averaged 27 queries and
               approximately 27 minutes, while recruiting sessions averaged 42 queries and
               approximately five hours and 28 minutes. Recruiters progressively formulated
               longer and more diverse queries and increased their use of advanced search
               operators and filters. Location was the most frequently used filter, appearing
               in approximately 88% of matching sessions and 81% of recruiting sessions.
               The overall positive candidate response rate was 12.8%, while search duration
               showed a negligible relationship with response rates. These findings
               demonstrate that talent search involves iterative refinement and substantial
               candidate assessment effort.




               Figure 2: Mean query duration of queries issued at different(normalized)
               points in time during a search session for bothmatching jobs (top, N = 92,020)
               and recruiting jobs (bottom, N= 36,113). Both plots include the three search
               stages accordingto the partitioning described in Section 3.2.3.




               Figure 3: Changes in filter usage across the three different search stages for
               the eight metrics in Table 2 with the highest effectsize 𝜂2. Error bars based on
               standard error are included, but are nearly invisible due to the low standard
               deviation and highsample size. With the exception of the difference in use of
               the job title filter (b) between recruiting stages 2 and 3, all means forthe three
               stages are statistically significant different for both matching and recruiting at
               p < 0.001 with multiple comparison onthe ANOVA results using the Tukey’s
```

## Source PDF page 6

```text
HSD test.




                         Figure 4: Time series plot of response rate (black) and unem-ployment rate
                         (red). All hard and soft lockdowns during theCovid-19 pandemic have been
                         added as areas shaded in darkand light blue respectively


Limitations / Research
Gap                      The study relied on search logs from a single Danish recruitment organization
                         and lacked detailed clickstream data, preventing the researchers from tracing
                         individual queries to shortlisted candidates. Its division of search sessions into
                         three stages was approximate, while positive response rates did not establish
                         actual applications or hiring outcomes. Additionally, the study did not
                         evaluate an AI-based recommendation system, leaving its potential
                         effectiveness in supporting recruiter searches untested.


Relevance to AYUDA
                         The study supports AYUDA's proposed Candidate Sourcing and Talent
                         Database by emphasizing the importance of iterative searching, advanced
                         filtering, and efficient candidate information retrieval. Its findings provide a
                         basis for developing flexible search functions that help recruiters locate and
                         reconsider previously sourced candidates. The study also informs how
                         AI-assisted recommendations could complement existing recruitment
                         workflows while maintaining recruiter involvement in candidate evaluation.


Implement Decision
                         Adapt and Benchmark. AYUDA can adapt the study's keyword-searching,
                         structured-filtering, and iterative-search principles for its centralized talent
                         database. AI-assisted semantic retrieval may be investigated as an additional
                         feature, although it was not evaluated in the study. The proposed approach
                         should be benchmarked against conventional search methods using retrieval
                         relevance, search completion time, and recruiter usability.


Synthesis
                         Kaya and Bogers (2023) examined recruiters' information-seeking behavior
                         using 128,133 search sessions containing approximately four million queries
                         from Jobindex. Their findings demonstrated that talent search involves
                         repeated query refinement, advanced filtering, and substantial candidate
                         assessment, with longer recruitment tasks requiring considerably more time.
                         The study provides a research foundation for AYUDA's proposed Candidate
                         Sourcing and Talent Database by supporting flexible information retrieval and
                         iterative candidate searching. However, because the researchers did not
                         evaluate AI-based recommendations, AYUDA must independently assess
                         whether semantic retrieval and explainable decision support improve
                         candidate rediscovery and recruitment efficiency.
```

## Source PDF page 7

```text
RRL 15 — The impact of human resources information systems and business process
management implementations on recruiting process performance: A case study

Laumer, Maier, & Eckhardt · Journal of Business Economics · 2014

FAU CRIS

What Sam should investigate: Recruitment process measures, workflow monitoring, process
improvement, cycle time, and the limitations of the empirical findings.

AYUDA relevance: Supports the standard recruitment workflow and monitoring functions without
claiming that a Kanban board is an innovation.

The impact of human resources information systems and business process management implementations
on recruiting process performance: A case study



 Author(s) and Year                    Laumer, S., Maier, C., & Eckhardt, A. (2014). The impact of
                                       human resources information systems and business process
                                       management implementations on recruiting process performance:
                                       A case study. In Proceedings of the 20th Americas Conference on
                                       Information Systems (AMCIS). Association for Information
                                       Systems.
                                       https://aisel.aisnet.org/amcis2014/AdoptionofIT/GeneralPresentati
                                       ons/15/

 Research Objectives                   The study aimed to examine how Business Process Management
                                       (BPM) and a Human Resources Information System (HRIS) can
                                       improve the recruitment process by reducing costs, shortening
                                       recruitment cycle time, improving process quality, and increasing
                                       stakeholder satisfaction.

 Algorithm/Model




                                       The study used a research model that examines the effects of
                                       Business Process Management (BPM) implementation and
                                       Human Resources Information System (HRIS) implementation on
                                       recruitment process performance. BPM includes process modeling,
                                       standardization, implementation, execution, controlling, and
                                       optimization. Recruitment performance is evaluated based on time,
                                       cost, quality, and stakeholder satisfaction. The model also
                                       considers how BPM and HRIS work together to improve the
                                       recruitment process.

 Data Set                              The study did not use a conventional numerical dataset. It used a
                                       qualitative case study of one Swiss financial service provider
                                       that had implemented BPM and an HRIS for its recruitment
                                       process. The researchers collected data during the
                                       post-implementation phase, after the new process had been
                                       operating for at least one year. The data included interviews with
                                       project-management personnel, HR management, and affected
```

## Source PDF page 8

```text
employees, as well as project documents and process-controlling
                             results. The interviews were recorded, transcribed, coded
                             according to the research model, and cross-checked by the
                             researchers.

Evaluation Metrics           The study evaluated recruitment process performance using
                             recruitment cost, recruitment cycle time, process quality, and
                             stakeholder satisfaction. It also examined process-related
                             indicators, such as job-posting costs, cost per hire, and
                             career-website visits. The relationships between BPM, HRIS
                             implementation, and recruitment performance were analyzed using
                             survey-based measures and linear regression analysis.

Key Findings                 The study reported that the company reduced its total
                             staff-recruitment cost by 50% between 2007 and 2010, particularly
                             the costs of job postings and cost per hire. The company also
                             observed an increase in career-website visits and changes in
                             impressions per job advertisement after reducing offline job
                             advertisements and increasing the use of online job boards. These
                             findings show that HRIS and BPM can support cost reduction,
                             recruitment monitoring, and data-based process improvement.




                             Figure 2 shows a decrease in cost per hire after the Applicant
                             Tracking System and BPM were implemented. It also shows an
                             increase in career-website visits and impressions per job
                             advertisement after the personnel-marketing strategy was adjusted.

Limitations / Research Gap   The study was limited because it focused on only one
                             organization, one information-system implementation, and only
                             the recruitment process. Therefore, the findings may not apply to
                             other organizations, systems, or business processes. Further
                             research should examine different organizations and recruitment
                             settings to determine whether the findings can be generalized.

Relevance to AYUDA           The study is relevant to AYUDA because it shows how BPM and
                             HRIS can organize recruitment activities, monitor workflow
                             progress, reduce delays, and track performance indicators such as
                             process time, cost, quality, and satisfaction. These findings support
                             AYUDA’s proposed standardized recruitment workflow, follow-up
                             monitoring, activity records, and recruiter decision-support
                             functions.

Implement Decision           Adapt. AYUDA can adapt the study’s BPM and HRIS principles
                             for standardized recruitment stages, workflow monitoring, process
                             documentation, follow-up tracking, and performance indicators.
                             However, the approach must be customized for AYUDA’s
                             multi-client recruitment workflow and combined with candidate
                             sourcing, résumé processing, explainable candidate-to-job
                             matching, and recruiter verification.

Synthesis
                             Laumer et al. (2014) demonstrated that combining Business
                             Process Management (BPM) with a Human Resources Information
                             System (HRIS) can improve recruitment performance. The case
                             study showed reduced recruitment costs, shorter process times,
                             improved process transparency, and increased stakeholder
                             satisfaction. However, the study focused on only one organization,
```

## Source PDF page 9

```text
one information system, and one recruitment process.

For AYUDA, the study supports the use of standardized
recruitment stages, workflow monitoring, process documentation,
follow-up tracking, and performance indicators. AYUDA can
adapt these principles to its multi-client recruitment workflow
while extending them with candidate rediscovery, résumé
processing, explainable candidate-to-job matching, and recruiter
decision support.
```
