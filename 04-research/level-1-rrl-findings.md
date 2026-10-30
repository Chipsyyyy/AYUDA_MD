# AYUDA — Level 1 RRL: Candidate-to-Job Matching and Explainable DSS

> **Source:** Team-submitted `AYUDA- RRL LVL1.pdf`.
> **Status:** Team research findings received; individual citations, metrics, and bibliographic details are not yet independently verified against original publications.
> **Scope:** Faithful searchable text extraction of the entire team-submitted PDF, preserving page boundaries. Embedded diagrams and figures remain in the original PDF; inspect that PDF for figures.
> **Important:** Do not treat the studies as final technology decisions or treat findings from external datasets as AYUDA-specific performance.

## Source PDF page 1

```text
/;




Rai — Recommendation Methods and Career-Based Matching
RRL 1: Job Recommender Systems: A Systematic Literature Review (2025)

Focus on content-based, collaborative, knowledge-based, hybrid, and reciprocal recommendation
approaches.

Job recommender systems: a systematic literature review, applications, open issues, and challenges

 Author(s) and Year      Ertuğrul and Bitirim (2025)

                         7th Gen APA Citation:
                         Ertuğrul, D. Ç., & Bitirim, S. (2025). Job recommender systems: a systematic
                         literature review, applications, open issues, and challenges. Journal of Big
                         Data, 12(1). https://doi.org/10.1186/s40537-025-01173-y

 Research Objective      The study aims to systematically review and critically analyze existing Job
                         Recommender Systems (JRSs), identify commonly used methodologies,
                         classify performance evaluation metrics, examine their applications in Human
                         Resource Management (HRM), and identify research trends, limitations, and
                         gaps.

 Algorithm / Model       Collaborative filtering approaches reviewed include item-based
                         recommendation, similarity ranking, fuzzy mathematics, and models
                         incorporating historical interactions and résumé information. Representative
                         studies include Guan et al.'s enterprise–talent recommendation system and Yi
```

## Source PDF page 2

```text
et al.'s optimized item-based collaborative filtering algorithm.



Dataset




                         The study analyzed 57 Job Recommender System research articles and 19
                         related survey articles published between 2010 and 2023. The reviewed
                         studies utilized different datasets involving candidate profiles, job postings,
                         and historical interactions. As a systematic literature review, the study did not
                         use a single experimental dataset to evaluate all recommendation approaches.

Evaluation Metrics       The study reviews predictive accuracy (MAE, MSE, RMSE),
                         classification-based accuracy (precision, recall, F1-score), ranking-based
                         accuracy (Precision@K, MAP, MRR, NDCG), and non-accuracy metrics
                         (scalability, diversity, coverage).

Key Findings             The study found that collaborative, content-based, hybrid, and
                         knowledge-based filtering are commonly represented in Job Recommender
                         System research, while reciprocal filtering remains comparatively
                         underexplored. Commonly discussed methodologies include similarity-based
                         techniques such as cosine similarity and TOPSIS, machine learning models
                         such as XGBoost and LSTM, and knowledge-based approaches such as
                         ontologies and the Semantic Web. Precision, recall, and F1-score were among
                         the most frequently used evaluation metrics.

                         The reviewed approaches demonstrate different methods of supporting job
                         recommendations, including fuzzy-mathematics-based talent ranking and
                         collaborative filtering that combines historical interactions with résumé
                         information.

Limitations / Research   The review identifies cold-start problems, data sparsity, scalability,
Gap                      interpretability, and data privacy as challenges affecting recommender
                         systems. Collaborative filtering can be particularly constrained by limited
                         historical interaction data, while reciprocal recommendation approaches
                         remain comparatively underexplored in the reviewed literature.

                         (These are limitations of recommendation approaches and gaps identified
                         across the literature)

Relevance to AYUDA       The study is relevant to AYUDA's proposed Candidate-to-Job Matching and
                         Explainable DSS because it examines recommendation approaches for
                         matching candidate information with job requirements. Its discussion of
                         recommendation architectures, historical-data limitations, and evaluation
                         methods provides a basis for comparing algorithms according to AYUDA's
                         data availability, matching requirements, and need for understandable
                         recommendations.
```

## Source PDF page 3

```text
Implement Decision      Compare / Further Investigate. The study will serve as a foundation for
                         comparing content-based, collaborative, knowledge-based, hybrid, and
                         reciprocal recommendation approaches. Further investigation will determine
                         which methods are most feasible for AYUDA based on available candidate
                         data, job requirements, explainability, and evaluation criteria.

 Synthesis               The reviewed literature establishes different approaches to candidate-job
                         recommendation and identifies the importance of matching accuracy,
                         explainability, and data availability. Further comparison and experimental
                         evidence are required to determine the most appropriate approach for
                         AYUDA.




RRL 4: Your Career Path Matters in Person-Job Fit (2024)

Focus on how previous work experience and career progression influence candidate-to-job matching.

Expected contribution: Identify and compare possible matching approaches that AYUDA could use.

                            Your Career Path Matters in Person-Job Fit

 Author(s) and Year      Gong et al. (2024)

                         APA 7th Gen:
                         Gong, Z., Song, Y., Zhang, T., Wen, J., Zhao, D., & Yan, R. (2024).

                                 Your career path matters in Person-Job fit. Proceedings of the

                                 AAAI Conference on Artificial Intelligence, 38(8), 8427–8435.

                                 https://doi.org/10.1609/aaai.v38i8.28685


 Research Objective      The study aims to improve person-job matching by developing a Work
                         Experience Enhanced Person-Job Matching (WEPJM) framework that
                         incorporates candidates' previous work experiences and career-path
                         preferences, specifically consistency, likeness, and continuity, to better assess
                         their suitability for job opportunities.

 Algorithm / Model




                         The study proposes the Work Experience Enhanced Person-Job Matching
                         (WEPJM) framework, which uses pre-trained BERT, Bi-LSTM, and an
                         attention mechanism to process résumé statements, chronological work
                         experiences, and job descriptions. It incorporates three auxiliary learning
                         tasks: Career Path Identification (CPI) for consistency, Career Path
```

## Source PDF page 4

```text
Reconstruction (CPR) for continuity, and Job-Career Contrastive Learning
                         (CL) for likeness. The resulting representations are combined and processed
                         through a Multi-Layer Perceptron (MLP) to predict candidate-job matching
                         scores.

Dataset                  The study utilized an anonymized real-world recruitment dataset consisting of
                         82,362 job postings, 33,285 résumés, and 117,780 work experiences. It
                         included 119,031 positive and 359,721 negative person-job pairs, labeled
                         according to candidate-recruiter interactions and job-viewing behavior on the
                         recruitment platform.

Evaluation Metrics       The study evaluated WEPJM using Accuracy, Precision, Recall, F1-score, and
                         Area Under the Curve (AUC). The proposed model achieved an accuracy of
                         0.850, precision of 0.844, recall of 0.829, F1-score of 0.837, and AUC of
                         0.929, outperforming the evaluated baseline models.

Key Findings




                         The proposed WEPJM framework outperformed the evaluated baseline
                         models, achieving an accuracy of 0.850, F1-score of 0.837, and AUC of
                         0.929. Ablation studies demonstrated that incorporating career-path learning
                         tasks improved matching performance, with Career Path Identification (CPI)
                         providing the strongest individual contribution. Case studies further illustrated
                         how considering career progression could produce recommendations more
                         aligned with candidates' professional seniority and development. However,
                         performance declined for candidates with limited work experience.

Limitations / Research   Existing person-job matching approaches have given insufficient attention to
Gap                      candidates' career progression. Although WEPJM addresses this gap, its
                         performance decreases for candidates with limited work experience.
                         Additionally, the study's use of recruitment interactions as positive and
                         negative matching labels may not fully reflect actual candidate qualifications
                         or job suitability.

Relevance to AYUDA       The study is relevant to AYUDA's proposed Candidate-to-Job Matching and
                         Explainable DSS because it demonstrates the importance of considering
```

## Source PDF page 5

```text
previous work experiences and career progression when assessing job
                     suitability. Its findings could support incorporating candidates' evolving skills,
                     responsibilities, and professional seniority into the matching process, allowing
                     recruiters to identify opportunities that align more closely with candidates'
                     qualifications and career direction.

Implement Decision   Adapt. The study's career-path-aware matching concepts may be incorporated
                     into a simpler, explainable candidate-to-job matching approach rather than
                     implementing the complete WEPJM framework. AYUDA's proposed system
                     could consider verified work experience, career progression, and job
                     requirements as matching criteria while providing understandable
                     explanations for recruiter review. The specific algorithm and criteria will be
                     determined through further research and client validation.

Synthesis            Gong et al. (2024) demonstrate that incorporating career-path information can
                     improve person-job matching performance compared with the evaluated
                     baseline models. Their findings complement earlier research on content-based
                     and explainable recommendations by highlighting the importance of previous
                     work experiences, career progression, and professional seniority. For
                     AYUDA, these concepts may support a simpler, transparent matching
                     approach that considers career history alongside qualifications and job
                     requirements without requiring the complete WEPJM architecture.
```

## Source PDF page 6

```text
Fiona — Explainable DSS and Fairness
RRL 2: Explainable Person–Job Recommendations: Challenges, Approaches, and Comparative Analysis
(2025)

Focus on explanation methods, interpretability, and how matching recommendations can be justified.

   Explainable person–job recommendations: challenges, approaches, and comparative analysis

 Author (s) and Year    Tang, F., Zhu, R., Yao, F., Wang, J., Luo, L., & Li, B. (2025). Explainable
                        person–job recommendations: Challenges, approaches, and comparative
                        analysis. Frontiers in Artificial Intelligence, 8, Article 1660548.
                        https://doi.org/10.3389/frai.2025.1660548

 Research Objectives    To review explainability methods for person–job recommendation systems and
                        determine how these methods improve transparency, fairness, and user trust
                        compared with black-box approaches. The study specifically examines how
                        recommendations can be understood and justified by job seekers and
                        recruiters.

 Algorithm/Model




                        The study is a systematic review and does not implement one new algorithm. It
                        reviews existing person–job recommendation models, including content-based,
                        collaborative-filtering, and hybrid approaches. It also organizes explainability
                        methods into three layers: the data layer, which explains feature extraction and
                        weighting; the model layer, which explains how candidate and job information
                        are processed; and the output layer, which explains recommendation results
                        using methods such as SHAP, LIME, natural-language explanations, and
                        counterfactual explanations.

 Data Set               The study did not use one original dataset because it was a systematic review.
                        It searched Google Scholar, Web of Science, and CNKI and reviewed English-
                        and Chinese-language studies published from 2019 to August 2025. From 150
                        screened studies, 85 were included.

                        The reviewed systems commonly used resumes, job descriptions, job
                        requirements, candidate preferences, recruiter preferences, and interaction
                        histories as data sources.

 Evaluation Metrics     The paper discusses recommendation measures such as HR@10, Recall@K,
```

## Source PDF page 7

```text
AUC, and accuracy. In its comparative analysis of six explanation-method
                          families, it used HR@10, fidelity, sparsity, user trust, and the combined
                          Explainability–Performance (E-P) score.

 Key Findings             The study found that person–job recommendation systems may become black
                          boxes because users cannot clearly see how data was extracted, how feature
                          weights were assigned, how the model made its decision, or why a
                          recommendation was produced.

                          Explainability can help users understand recommendations, identify possible
                          system problems, support fairness, and improve trust. However, more complex
                          models may provide strong performance while becoming more difficult to
                          interpret.

 Limitations /            The study was limited to selected databases, studies from 2019–2025, and
 Research Gap             English or Chinese publications. The researchers also did not pre-register the
                          review. The explanation methods have limitations: some may not fully show
                          the model’s reasoning, while others may be difficult to understand, require
                          more data, or need greater computing resources. Many systems also do not
                          adapt to user feedback.

                          Therefore, the study does not identify one explanation method that is best for
                          every recruitment system.

 Relevance to             The findings support AYUDA’s need for transparent candidate-to-job
 AYUDA                    recommendations. AYUDA can show which candidate information was used,
                          which job requirements matched, which requirements were missing, and which
                          information still needs verification. This can help recruiters review and justify
                          recommendations before endorsement.

 Implement Decision       Adapt selected principles rather than implementing every advanced
                          method. AYUDA may begin with a transparent rule-based or structured
                          explanation layer that displays match-gap breakdowns, visible criteria, source
                          evidence from the candidate profile and job requirements, and recruiter
                          verification. SHAP, LIME, counterfactual explanations, or complex knowledge
                          graphs should only be considered if they are technically feasible and approved.

 Synthesis                The study shows that a person–job recommendation system should not only
                          produce a match score. It should also show how the input data was used, how
                          the matching process was performed, and why the recommendation was
                          generated. For AYUDA, this supports an Explainable Decision Support System
                          that gives transparent and reviewable recommendations while keeping the final
                          decision with authorized recruiters and client companies.




RRL 6: Mapping Stakeholder Needs to Multi-Sided Fairness in Candidate
Recommendation for Algorithmic Hiring (2025)

Focus on fairness and the different needs of applicants, recruiters, and client companies.

Expected contribution: Determine how AYUDA's proposed DSS could provide transparent and
responsible recommendations.


Mapping Stakeholder Needs to Multi-Sided Fairness in Candidate Recommendation for
Algorithmic Hiring

 Author(s) and Year                 Kaya, M., & Bogers, T. (2025). Mapping stakeholder needs to
                                    multi-sided fairness in candidate recommendation for algorithmic
                                    hiring. n RecSys ’25: Proceedings of the Nineteenth ACM
                                    Conference on Recommender Systems (pp. 257–267). Association for
                                    Computing Machinery. https://doi.org/10.1145/3705328.3748079
```

## Source PDF page 8

```text
Research Objectives   To identify and map fairness metrics suitable for a multi-stakeholder
                      candidate recommendation scenario and determine how these metrics
                      can support the development of fairness-aware machine-learning
                      systems.

                      The study also aims to map and incorporate understanding and the
                      lived experience of stakeholders into fairness metric design, although
                      we consider multiple different stakeholders.

Algorithm/Model       The study used semi-structured interviews with 40 stakeholders and
                      thematic analysis to identify fairness concerns in algorithmic hiring.
                      It describes an existing content-based candidate recommendation
                      system using a cross-encoder model to match CVs with job postings
                      and rank candidates.

                      Rather than implementing a new fairness-aware algorithm, the study
                      mapped stakeholder needs to existing fairness metrics and proposed
                      their use in future auditing and fairness-aware system development.

Data Set              The study’s algorithmic hiring scenario used Jobindex’s CV
                      database, which contained more than 160,000 candidate CVs. The
                      system also used job-posting text to calculate candidate–job
                      matching scores. For the qualitative study, the researchers collected
                      data from 40 stakeholder interviews and a screening survey with 246
                      job seekers.

                      However, they did not analyze an actual recommendation-outcome
                      dataset or publicly release a machine-learning dataset.

Evaluation Metrics    The study mapped stakeholder concerns to possible fairness metrics,
                      including Conditional Demographic Parity, rank-aware fairness,
                      diversity, coverage, the Gini index, and company parity. These
                      metrics may be used to examine whether qualified candidates and
                      companies receive fair opportunities. However, the researchers did
                      not calculate these metrics using actual recommendation outcomes.
                      They proposed them for future algorithmic auditing and
                      fairness-aware system development.

Key Findings




                      The screening survey showed that 74 out of 246 job seekers, or
                      30.1%, reported experiencing discrimination or unfair treatment
                      while seeking employment. Among these respondents, age was the
                      most commonly suspected factor, followed by gender. This finding
                      highlights why fairness should be monitored in algorithmic hiring
                      systems. However, the survey did not prove that the unfair treatment
                      was caused by the recommendation algorithm.

                      During the interviews, many participants emphasized that candidates
                      should first meet the qualifications stated in the job advertisement.
                      After considering qualifications, many participants believed that
                      candidates should be treated equally regardless of other personal
                      characteristics. The study also found that fairness should consider
                      multiple stakeholders, including job seekers, recruiters, companies,
```

## Source PDF page 9

```text
and recruitment agencies.


 Limitations / Research Gap
                                  The study identified that fairness is difficult to quantify because there
                                  is no single definition or universally correct fairness metric.
                                  Although the researchers mapped stakeholder perspectives to
                                  possible fairness metrics, they did not empirically test these metrics
                                  using actual candidate recommendation outcomes.

                                  The study was also limited by the lack of diversity among the
                                  participating job seekers and companies. In addition, most
                                  participants came from Denmark and were connected to one
                                  recruitment agency, so the findings may not fully apply to other
                                  countries, cultures, or recruitment systems. These limitations show
                                  the need for future research using real recruitment data and more
                                  diverse stakeholders.


 Relevance to AYUDA               This study is relevant to AYUDA because it emphasizes the need for
                                  fair and transparent candidate recommendation systems. Its focus on
                                  qualifications, fairness metrics, stakeholder needs, and algorithmic
                                  auditing can guide AYUDA in developing a DSS that recommends
                                  suitable candidates while reducing bias. AYUDA can apply a
                                  qualification-first approach, provide explanations for
                                  recommendations, monitor whether qualified candidates are fairly
                                  considered, and maintain human recruiter review before final
                                  decisions are made.

                                  This supports a more responsible and multi-stakeholder hiring
                                  process for applicants, recruiters, and client companies.

 Implement Decision               Adopt and adapt. AYUDA can adopt the study’s multi-stakeholder
                                  fairness approach and adapt its proposed metrics for system auditing.
                                  However, the metrics should be tested using AYUDA’s own
                                  candidate and recruitment data before full implementation.

 Synthesis                        Kaya and Bogers (2025) emphasized that algorithmic hiring systems
                                  should consider fairness for multiple stakeholders, including job
                                  seekers, recruiters, companies, and recruitment agencies. Their study
                                  identified fairness metrics for evaluating qualified candidates and
                                  company access, but it did not implement or test a fairness-aware
                                  recommendation algorithm using actual hiring outcomes. In
                                  comparison, AYUDA can apply these insights by developing a
                                  qualification-based and transparent candidate recommendation DSS
                                  with fairness monitoring, explanations, and human recruiter review.
                                  Thus, the study provides a foundation for making AYUDA’s
                                  recommendations more responsible and fair.




Tine — Matching Algorithms and Practical Evaluation
RRL 3: Enhancing Person-Job Fit for Talent Recruitment (2018)

Focus on the Ability-aware Person-Job Fit Neural Network (APJFNN), its architecture, algorithms, and
evaluation results.

  Enhancing Person-Job Fit for Talent Recruitment:An Ability-aware Neural Network Approach

 Author(s) and Year      Qin, C., Zhu, H., Xu, T., Zhu, C., Jiang, L., Chen, E., & Xiong, H. (2018).
                         Enhancing person-job fit for talent recruitment: An ability-aware neural
                         network approach. In Proceedings of the 41st International ACM SIGIR
                         Conference on Research & Development in Information Retrieval (pp.
                         25–34). Association for Computing Machinery
```

## Source PDF page 10

```text
Research Objective       To improve Person-Job Fit prediction by automatically analyzing job
                         requirements and candidate experiences, reducing dependence on manual
                         feature evaluation, and providing more interpretable recruitment matching
                         results.

Algorithm / Model




                         The study proposed the Ability-aware Person-Job Fit Neural Network
                         (APJFNN), which uses Bidirectional Long Short-Term Memory
                         (BiLSTM) networks for semantic text representation and four hierarchical
                         ability-aware attention mechanisms to identify important job requirements and
                         relevant candidate experiences. A fully connected prediction network
                         estimates Person-Job Fit.

Dataset                  The researchers used anonymized historical recruitment records from a
                         high-technology company in China. The original dataset contained 17,766 job
                         postings and 898,914 resumes. After preprocessing, the retained dataset
                         included 3,652 job postings, 533,069 resumes, 12,796 successful applications,
                         and 1,058,547 failed applications. The data covered technology, product, user
                         interface, and other job categories.

Evaluation Metrics       Accuracy, Precision, Recall, F1-score, and Area Under the ROC Curve
                         (AUC). The researchers also evaluated performance across different
                         training-data proportions and examined computational efficiency.

Key Findings             APJFNN outperformed the evaluated baseline models, achieving 75.59%
                         accuracy, 75.45% precision, 76.03% recall, 75.74% F1-score, and 0.8316
                         AUC on the balanced evaluation dataset. The hierarchical attention
                         mechanisms improved predictive performance compared with the basic
                         RNN-based model (BPJFNN) and helped highlight important requirements
                         and relevant candidate experiences.

Limitations / Research   The study relied on historical recruitment outcomes from a single company,
Gap                      which may limit generalizability. Its original dataset was highly imbalanced,
                         requiring undersampling for evaluation. The model also requires substantial
                         labeled recruitment data and a relatively complex neural architecture.
                         Additionally, the study did not establish whether its attention-based
                         explanations faithfully represent all factors influencing predictions or whether
                         the model performs fairly across different applicant groups.

Relevance to AYUDA       The study supports AYUDA's proposed candidate-to-job matching and
                         candidate rediscovery features by demonstrating how semantic analysis can
                         identify relationships between job requirements and candidate qualifications
                         beyond exact keyword matching. Its attention-based approach also provides a
                         conceptual basis for highlighting relevant skills and experiences, helping
                         recruiters understand candidate recommendations.

Implement Decision       Adapt and Benchmark. AYUDA can adapt the study's concepts of semantic
                         matching, requirement weighting, and explainable candidate
                         recommendations without necessarily implementing the complete APJFNN
                         architecture. The proposed matching approach should be evaluated against
                         simpler baseline methods using AYUDA's available recruitment data before
                         selecting a final model.
```

## Source PDF page 11

```text
Synthesis
                         Qin et al. (2018) demonstrated the potential of deep learning in improving
                         Person-Job Fit prediction through their proposed Ability-aware Person-Job Fit
                         Neural Network (APJFNN). By integrating Bidirectional Long Short-Term
                         Memory (BiLSTM) networks with four hierarchical attention mechanisms, the
                         model analyzes the semantic relationships between job requirements and
                         candidate experiences while identifying the qualifications most relevant to a
                         position. The study achieved an accuracy of 75.59%, an F1-score of 75.74%,
                         and an AUC of 0.8316, outperforming the evaluated baseline models. These
                         findings suggest that ability-aware semantic matching can improve
                         recruitment predictions while providing greater interpretability through the
                         identification of important requirements and relevant experiences.

                         The study provides a valuable foundation for AYUDA's proposed
                         candidate-to-job matching and candidate rediscovery features. Its approach
                         demonstrates how recruitment systems can move beyond traditional keyword
                         matching by considering the contextual relevance of candidate qualifications.
                         However, the model's dependence on extensive historical recruitment data, its
                         computational complexity, and its limited evaluation within a single
                         organization highlight the need for adaptation. Therefore, AYUDA can adopt
                         the principles of semantic matching and explainable recommendations while
                         evaluating simpler and more practical approaches suited to its available data
                         and operational requirements.




RRL 5: Analyzing the Effects of a Human-in-the-Loop Candidate Recommendation
Algorithm at Jobindex (2026)

Focus on SPBERT, human-in-the-loop recommendations, recruiter adoption, and real-world evaluation.

Expected contribution: Assess the technical feasibility of matching models and how recommendation
performance should be measured.

Analyzing the Effects of a Human-in-the-Loop Candidate Recommendation Algorithm at Jobindex

 Author(s) and Year      Kaya, M., & Bogers, T. (2027). Analyzing the effects of a human-in-the-loop
                         candidate recommendation algorithm at Jobindex. ACM Transactions on
                         Recommender Systems, 5(2), Article 26. https://doi.org/10.1145/3801092

 Research Objective      To develop, deploy, and evaluate an AI-based candidate recommendation
                         system that supports recruiters in identifying suitable candidates while
                         maintaining human oversight. The study also investigated how recruiter
                         engagement with AI-generated recommendations affects recruitment
                         productivity, candidate response rates, and search effort in real-world
                         operations.
```

## Source PDF page 12

```text
Algorithm / Model




                         The researchers implemented Sentence-pair BERT (SPBERT), a
                         Transformer-based model that jointly processes job postings and resumes to
                         predict candidate relevance. The model uses a pre-trained BERT encoder, a
                         multilayer perceptron (MLP) classification layer, and binary cross-entropy
                         loss for training. It was compared with Job Title-based Recommendation with
                         Item History (JTIH), Person-Job Fit Neural Network (PJFNN), Basic
                         Person-Job Fit Neural Network (BPJFNN), and Sentence-BERT (SBERT).
                         The deployed system followed a Human-in-the-Loop (HITL) approach,
                         allowing recruiters to review recommendations and make final shortlisting
                         decisions.

Dataset                  The offline experiments used historical recruitment data from Jobindex,
                         Denmark, covering April 2018 to May 2022. The dataset contained
                         approximately 138,000 job postings, 120,941 CVs, and 2,427,288 job–resume
                         pairs. For the online A/B test, 38 recruiters processed 1,334 job postings over
                         25 days in March 2023. The subsequent deployment analysis covered 41,390
                         recruitment tasks over 17 months (April 2023–September 2024), examining
                         recruiters' interactions with recommended candidates and their responses.

Evaluation Metrics       Offline evaluation used Area Under the ROC Curve (AUC) for classification
                         and Normalized Discounted Cumulative Gain at 20 (NDCG@20) for
                         candidate ranking. Online evaluation used Positive Response Rate (PRR) and
                         Contacted From Recommendations (CFR). The longitudinal analysis
                         additionally measured Negative Response Rate (NRR), number of contacted
                         candidates, positive and negative responses, number of search queries, and
                         effort required to identify relevant candidates.

Key Findings             SPBERT outperformed the evaluated baseline models in offline experiments,
                         achieving 0.946 AUC and 0.186 NDCG@20. In the online A/B test, SPBERT
                         achieved a PRR of 13.5% and CFR of 41.1%, compared with JTIH's 12.7%
                         PRR and 24.75% CFR. The CFR improvement was statistically significant,
                         while the PRR difference was not. During the 17-month deployment,
                         recruiters who engaged with recommendations achieved a 12.72% higher
                         PRR, contacted 15.92% more candidates, and submitted 22.73% fewer search
                         queries than those who skipped recommendations. These findings indicate that
                         AI-assisted recommendations can support recruitment efficiency when
                         integrated into existing workflows.

Limitations / Research   The study identified challenges involving recruiter distrust of AI, inconsistent
Gap                      adoption, and insufficient explanations for recommended candidates. Its skill
                         and occupation highlighting mechanism did not always provide satisfactory
                         evidence of candidate relevance. The study also acknowledged possible
                         self-selection bias in recruiter feedback and limitations in categorizing
                         engagement into only two groups: Check and Skip. Furthermore, the system
```

## Source PDF page 13

```text
was evaluated within Jobindex's recruitment environment, which may limit
                     generalizability to other organizations. The longitudinal comparison was
                     observational, so differences between Check and Skip groups should not
                     automatically be interpreted as causal effects.

Relevance to AYUDA   The study supports AYUDA's proposed AI-assisted candidate
                     recommendation, semantic job matching, and candidate rediscovery features.
                     SPBERT demonstrates how job postings and resumes can be jointly analyzed
                     to identify relevant candidates despite differences in terminology and
                     document structure. Its HITL approach also supports AYUDA's objective of
                     assisting recruiters without replacing their professional judgment.
                     Additionally, the findings on skill highlighting, recruiter trust, and workflow
                     integration provide a basis for designing explainable recommendations that
                     recruiters can review before shortlisting candidates.

Implement Decision   Adapt and Benchmark. AYUDA can adapt the study's semantic matching and
                     Human-in-the-Loop principles by incorporating AI-generated candidate
                     recommendations into the existing recruitment workflow while retaining
                     recruiter control over final decisions. SPBERT should be considered a
                     candidate model for benchmarking against simpler semantic matching
                     approaches using AYUDA's available recruitment data. The system should
                     also prioritize relevant skill highlighting, recommendation explanations, and
                     recruiter feedback to improve usability and trust.

Synthesis
                     Kaya and Bogers (2027) investigated the development and deployment of a
                     Human-in-the-Loop candidate recommendation system at Jobindex using
                     Sentence-pair BERT (SPBERT). The model jointly analyzes job postings and
                     resumes to predict candidate relevance, addressing limitations of traditional
                     keyword matching and structured-input neural models. SPBERT achieved an
                     AUC of 0.946 and NDCG@20 of 0.186, outperforming the evaluated baseline
                     algorithms. The 17-month deployment analysis further showed that recruiters
                     who engaged with AI-generated recommendations achieved higher positive
                     response rates, contacted more candidates, and performed fewer search
                     queries. However, the study identified challenges involving recruiter trust,
                     recommendation explainability, and inconsistent system adoption.

                     The findings provide a methodological foundation for AYUDA's proposed
                     candidate-to-job matching and candidate rediscovery features. In particular,
                     the study demonstrates the potential of Transformer-based semantic matching
                     to process recruitment information while emphasizing the importance of
                     maintaining human oversight. For AYUDA, the proposed approach can be
                     adapted by integrating explainable candidate recommendations into recruiters'
                     existing workflows and benchmarking semantic matching models against
                     available recruitment data. This supports the development of an AI-assisted
                     recruitment system that improves candidate identification without removing
                     recruiters' responsibility for final decisions.
```
