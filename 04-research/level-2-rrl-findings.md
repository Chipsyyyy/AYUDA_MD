# AYUDA — Level 2 RRL: Resume Processing, Skill Normalization and Bidirectional Recommendations

> **Source:** Team-submitted `AYUDA- RRL LVL2.pdf`.
> **Status:** Team research findings received; individual citations, metrics, and bibliographic details are not yet independently verified against original publications.
> **Scope:** Faithful searchable text extraction of the entire team-submitted PDF, preserving page boundaries. Embedded diagrams and figures remain in the original PDF; inspect that PDF for figures.
> **Important:** Do not treat the studies as final technology decisions or treat findings from external datasets as AYUDA-specific performance.

## Source PDF page 1

```text
Rai: Résumé information extraction and NLP
RRL 7 — Automated Resume Parsing: A Natural Language Processing Approach

IEEE CSITSS · 2023

This paper investigates résumé parsing through a combination of Named Entity Recognition (NER),
keyword matching, and regular expressions to identify details such as names, contact information,
education, skills, and experience.

IEEE Xplore

What Rai should investigate: How NER and rule-based extraction complement one another, which fields
are extracted, how accuracy is evaluated, and whether the approach can handle varied résumé formats.

AYUDA relevance: Supports converting submitted résumés into structured candidate profiles before job
matching.

Read RRL 7


              Automated Resume Parsing: A Natural Language Processing Approach

 Author(s) and Year      Sougandh et al. (2023)

                         Sougandh, T. G., K, S. S., Reddy, N. S., & Belwal, M. (2023). Automated
                         resume parsing: a natural language processing approach. International
                         Conference on Computation System and Information Technology for
                         Sustainable Solutions (CSITSS), 1–6.
```

## Source PDF page 2

```text
https://doi.org/10.1109/csitss60515.2023.10334236

Research Objective       The study aims to develop an automated résumé parsing system that integrates
                         Named Entity Recognition (NER) and Regex-based keyword and pattern
                         matching to extract and organize structured candidate information, including
                         personal details, skills, education, and work experience, from different résumé
                         formats.

Algorithm / Model




                         The study implements a hybrid résumé parsing approach combining a
                         SpaCy-based Named Entity Recognition (NER) model with keyword and
                         pattern matching using Regular Expressions (Regex). The NER model is
                         trained on annotated résumé data to identify candidate-related entities, while
                         Regex extracts information using predefined patterns. The extracted outputs
                         are combined, filtered for duplicate or irrelevant values, and presented as
                         structured candidate information. Supporting tools include PDFMiner,
                         docx2txt, Python, Pandas, and YAML.

Dataset                  The researchers assessed the NER model using a testing dataset and
                         demonstrated the extraction of candidate information through sample outputs
                         and a graphical interface. However, no numerical evaluation metrics, such as
                         precision, recall, F1-score, or accuracy, were reported for the proposed parser.

Evaluation Metrics       The researchers assessed the NER model using a testing dataset and
                         demonstrated the extraction of candidate information through sample outputs
                         and a graphical interface. However, no numerical evaluation metrics, such as
                         precision, recall, F1-score, or accuracy, were reported for the proposed parser.

Key Findings             The proposed résumé parser demonstrated the extraction of candidate
                         information, including names, contact details, skills, education, work
                         experience, languages, and CGPA, using a combination of NER and
                         Regex-based pattern matching. The extracted information was presented in a
                         structured format, with a graphical interface supporting résumé comparison.
                         Although the authors described the approach as reliable and efficient, the
                         study did not report numerical accuracy or processing-time measurements to
                         substantiate these claims.

Limitations / Research   Although the study presents an automated résumé parser combining NER and
Gap                      Regex-based extraction, its evaluation lacks detailed dataset information,
                         including the number of résumés and training/testing split. Furthermore, the
                         researchers did not report numerical performance metrics, making it difficult
                         to assess the parser's extraction accuracy, efficiency, and consistency across
                         different résumé formats.

Relevance to AYUDA       The study is relevant to AYUDA's proposed résumé processing and candidate
                         profiling module because it demonstrates how NER and Regex-based
                         extraction can organize candidate information from résumé documents into
                         structured records. This approach could reduce repetitive manual encoding,
                         support efficient retrieval and reuse of previously sourced candidates, and
                         provide verified candidate information for the proposed candidate-to-job
                         matching system.

Implement Decision       Adapt / Further Investigate. The study's combination of NER and
```

## Source PDF page 3

```text
Regex-based extraction may serve as a foundation for AYUDA's proposed
                          résumé processing module. However, additional capabilities for information
                          standardization, recruiter verification, and structured candidate profiling
                          would need to be investigated to support candidate rediscovery and
                          explainable job matching. The use of pretrained NLP models and rule-based
                          extraction will be considered as a potentially feasible approach, subject to
                          further research and validation.

 Synthesis
                          Sougandh et al. (2023) demonstrate the use of NER and Regex-based
                          extraction to convert résumé information into structured candidate data. While
                          the approach provides a potential foundation for automated candidate
                          profiling, the study does not establish quantitative extraction performance or
                          demonstrate how the extracted information can support explainable
                          candidate-to-job matching. For AYUDA, the approach may be adapted as a
                          supporting technology, with further research needed on data standardization,
                          verification, and integration with the proposed DSS.




RRL 8 — Resume Parsing Across Multiple Job Domains Using a BERT-Based NER
Model

IEEE AICS · 2023 conference, indexed 2024

The researchers fine-tuned a BERT-based NER model using annotated résumés from IT, HR, consultancy,
and engineering. The paper emphasizes the importance of dataset size, annotation quality, and domain
variation.

IEEE Xplore

What Rai should investigate: BERT fine-tuning, annotated training data, entity extraction metrics,
generalization across job domains, and limitations of small datasets.

AYUDA relevance: Helps assess whether a trained NLP model is practical compared with a simpler
extraction pipeline.

Read RRL 8


          Resume Parsing Across Multiple Job Domains Using a BERT-Based NER Model

 Author(s) and Year       Srivastava and Greaney (2023)

                          Srivastava, M., & Greaney, P. (2023). Resume parsing across multiple job
                          domains using a BERT-Based NER model. Irish Conference on Artificial
                          Intelligence and Cognitive Science (AICS), 1–4.
                          https://doi.org/10.1109/aics60730.2023.10470917

 Research Objective       The study aims to develop and evaluate a fine-tuned BERT-based Named
                          Entity Recognition (NER) model for extracting structured candidate
                          information from résumés across multiple job domains using limited
                          annotated training data, while investigating how dataset size and annotation
                          quality influence model performance and generalization.
```

## Source PDF page 4

```text
Algorithm / Model




                     The study implements a fine-tuned BERT-based Named Entity Recognition
                     (NER) model using SpaCy's training pipeline. The pretrained BERT model
                     generates contextual representations of résumé text, which are processed by an
                     NER classifier consisting of a feedforward network and softmax activation to
                     identify four entity categories: job title, experience, skill, and education. The
                     model is fine-tuned using manually annotated résumé samples from multiple
                     job domains.

Dataset




                     The study utilized approximately 2,400 résumé samples sourced from
                     LiveCareer.com, originally in PDF format. From this collection, 180 résumés
                     across four job domains—Human Resources, Information Technology,
                     Consultancy, and Engineering—were manually annotated for job titles, skills,
                     education, and experience. Three experiments were conducted using 100, 140,
                     and 180 annotated résumés, containing 4,940, 6,216, and 7,425 entities,
                     respectively. Each experiment used an 80:20 training-validation split.

Evaluation Metrics   The study evaluated the fine-tuned BERT-based NER model using precision,
                     recall, and F1-score across three experiments involving 100, 140, and 180
                     annotated résumés. The 180-sample experiment achieved the highest overall
                     validation F1-score of 0.7714, with a precision of 0.7539 and recall of 0.7896.
                     Entity-level evaluation showed the highest validation F1-score for job titles
                     (0.9474) and the lowest for education (0.7101).

Key Findings         The study demonstrated that fine-tuning a pretrained BERT-based NER model
                     can support résumé information extraction across multiple job domains using
```

## Source PDF page 5

```text
limited annotated training data. Increasing the dataset to 180 résumés
                         improved the overall validation F1-score to 0.7714, although overfitting
                         remained evident. Entity-level results showed varying performance, with job
                         titles achieving the highest validation F1-score (0.9474) and education the
                         lowest (0.7101). The findings emphasize the importance of dataset size,
                         annotation quality, and model optimization in résumé information extraction.

Limitations / Research   The study was limited by a relatively small annotated dataset of 180 résumés
Gap                      covering four job domains, resulting in persistent overfitting and varying
                         extraction performance across entity categories. The researchers also
                         emphasized the importance of annotation quality and consistency, noting that
                         larger, more diverse datasets and improved annotation procedures are needed
                         to strengthen model generalization. Increasing the dataset size alone may not
                         fully resolve the observed overfitting.

Relevance to AYUDA       The study is relevant to AYUDA's proposed résumé processing and candidate
                         profiling module because it demonstrates the potential of BERT-based NER to
                         extract structured candidate information, including job titles, skills, education,
                         and work experience, across multiple job domains. Its findings emphasize the
                         importance of extraction accuracy and data quality, which are essential for
                         developing reliable candidate profiles that can support candidate rediscovery
                         and the proposed explainable job-matching DSS. The study also provides a
                         basis for evaluating the feasibility of pretrained NLP approaches with recruiter
                         verification rather than immediately adopting custom model fine-tuning.

Implement Decision       Compare / Adapt. The study's BERT-based NER approach will be considered
                         as a research alternative rather than directly adopted. Given the challenges of
                         limited annotated training data and overfitting, AYUDA's proposed system
                         will initially investigate using an existing pretrained NLP model supplemented
                         by rule-based extraction and manual verification of candidate information.
                         This approach may reduce the need for custom model training while
                         supporting structured candidate profiling and the proposed matching DSS. Its
                         suitability will require further evaluation and client validation.

Synthesis
                         Sougandh et al. (2023) and Srivastava and Greaney (2023) demonstrate the
                         potential of NLP-based approaches for extracting structured candidate
                         information from unstructured résumés. Sougandh et al. combined Named
                         Entity Recognition (NER) with Regex-based pattern matching to extract
                         multiple candidate fields, while Srivastava and Greaney employed a
                         fine-tuned BERT-based NER model to recognize job titles, skills, education,
                         and experience across different job domains. Although the latter provided
                         measurable extraction performance, its findings revealed challenges involving
                         limited annotated data, overfitting, and varying accuracy across entity
                         categories.

                         For AYUDA, these studies support investigating an adaptable
                         résumé-processing approach that combines pretrained NLP with rule-based
                         extraction and recruiter verification. However, further evaluation is needed to
                         establish whether this approach can reliably produce structured candidate
                         profiles suitable for candidate rediscovery and explainable job matching.
```

## Source PDF page 6

```text
Fiona: Skill and job requirement normalization
RRL 9 — Joint Extraction and Classification of Danish Competences for Job Matching

Li & Lioma · ECIR / Springer · 2023

This study proposes a BERT-like model that both extracts and classifies skills, occupations, and
knowledge from job postings. It uses structured competence labels and reports improved efficiency
compared with the models evaluated in the study.

University of Copenhagen Research Portal

What Fiona should investigate: Competence extraction, classification, ESCO labels, the relationship
between extraction and normalization, and whether the method transfers to English-language recruitment
records.

AYUDA relevance: Supports converting different descriptions of skills and qualifications into comparable
categories.

Read RRL 9

        Joint Extraction and Classification of Danish Competences for Job Matching

 Author(s) and Year            Li, Q., & Lioma, C. (2023). Joint extraction and classification of Danish
                               competences for job matching. In J.Kamps, L. Goeuriot, F. Crestani, M.
                               Maistro, H. Joho, B. Davis, C. Gurrin, U. Kruschwitz, & A. Caputo
                               (Eds.), Advances in information retrieval: 45th European Conference on
                               Information Retrieval, ECIR 2023 (Lecture Notes in Computer Science,
                               Vol. 13981, pp. 475–483). Springer.
                               https://doi.org/10.1007/978-3-031-28238-6_38

 Research Objectives           The study aimed to develop a BERT-based model that automatically
                               extracts and classifies Danish competences, including skills,
                               occupations, and knowledge areas, from job postings using ESCO
                               labels. The model was designed to support job matching and improve
                               recruiter efficiency by processing competence information accurately
                               and quickly.

 Algorithm/Model




                               The study proposed a single BERT-based model for jointly extracting
                               and classifying Danish competences. It used DaBERT and DaJobBERT
                               as text encoders. The model first used Named Entity Recognition to
                               detect competence terms and then classified them using ESCO
                               categories, such as skills, occupations, and knowledge.

                               The model was trained jointly but performed extraction and
                               classification sequentially during prediction. It was compared with
                               SkillSpan plus Kompetencer, a separate detection-and-classification
                               model, and an all-class NER model.
```

## Source PDF page 7

```text
Data Set                     The study used 217,661 Danish sentences from the Jobindex database,
                             including job-posting descriptions and candidate education and
                             work-experience information. The data were annotated with ESCO
                             labels for skills, occupations, knowledge, and other competences. The
                             dataset was divided into training, validation, and test sets using an 8:1:1
                             ratio. The data were provided by Jobindex and were not publicly
                             available.

Evaluation Metrics           The study evaluated ESCO competence extraction using the F1-score,
                             which measured whether tokens were correctly identified as part of an
                             ESCO competence. It evaluated ESCO competence classification using
                             the weighted Macro-F1 score, which measured whether extracted
                             competences were assigned to the correct ESCO categories. The study
                             also measured efficiency using the average processing time per job,
                             based on 100 randomly selected job postings. Model size and inference
                             time were additionally reported for comparison, but model size itself is
                             not an evaluation metric.

Key Findings                 The proposed joint BERT-based model achieved the strongest
                             competence classification performance among the compared approaches
                             and processed job postings more than 50% faster than the SkillSpan +
                             Kompetencer pipeline. Joint training improved classification
                             performance, while competence extraction remained comparable to
                             other models. The results also showed that DaBERT and DaJobBERT
                             performed similarly when trained with sufficient in-domain data

Limitations / Research Gap   The study was limited to Danish-language data and used a dataset that
                             was not publicly available. The model was evaluated for competence
                             extraction and classification but was not integrated into a complete
                             automatic job recommendation framework. Therefore, its effectiveness
                             in other languages and in actual job-matching scenarios remains
                             uncertain. Future research should test the model on publicly available
                             English datasets and integrate it into a complete job recommendation
                             system.

Relevance to AYUDA           The study is relevant to AYUDA because its BERT-based model
                             supports automatic competence extraction and classification from job
                             postings and candidate profiles. This can guide AYUDA’s resume
                             processing, skill normalization, and candidate-to-job matching features.

                             However, the approach must be adapted and validated using English or
                             Filipino recruitment data because the original model was developed
                             using Danish-language data from Jobindex.

Implement Decision           Adapt. AYUDA may adapt the study’s BERT-based competence
                             extraction and classification approach for resume processing and
                             candidate-to-job matching. The model must be retrained or validated
                             using English or Filipino recruitment data because the original study
                             used Danish-language data and a Jobindex dataset. Implementation
                             should depend on data availability, technical feasibility, and system
                             testing.

Synthesis
                             Li and Lioma (2023) demonstrated that a BERT-based model can jointly
                             extract and classify competences from job postings and candidate
                             information using ESCO categories. The model achieved strong
                             classification performance and processed job-related text efficiently.
                             However, it was limited to Danish-language data and was not tested in a
                             complete job recommendation system.

                             For AYUDA, the study provides a basis for developing NLP-assisted
                             resume processing, skill normalization, and candidate-to-job matching.
                             The approach should be adapted and validated using English or
                             Philippine recruitment data before implementation. Therefore, the study
                             supports AYUDA’s proposed system by showing how standardized
                             competence extraction can make candidate matching more organized
                             and efficient.
```

## Source PDF page 8

```text
RRL 10 — RINX: A System for Information and Knowledge Extraction from Resumes

Data & Knowledge Engineering · 2023

This study describes an end-to-end résumé information extraction system designed to process varied
résumé structures and organize candidate information.

ScienceDirect

What Fiona should investigate: How extracted information is represented, whether structured knowledge
is created, how different résumé layouts are handled, and how output fields could be mapped to
standardized job requirements.

AYUDA relevance: Provides an additional technical foundation for creating consistent candidate
information.

This is primarily an information-extraction study, not a dedicated skill-taxonomy study. Fiona should
distinguish those contributions in the matrix.

Read RRL 10
https://www.researchgate.net/publication/280944384_RINX_Information_Extraction_Search_and_Insight
s_from_Resumes


                RINX: Information Extraction, Search and Insights from Resumes


 Author(s) and Year             Srivastava, R., Palshikar, G. K., & Hingmire, S. (2011). RINX:
                                Information extraction, search and insights from resumes. Tata Research
                                Development and Design Centre, TACTiCS 2011.

 Research Objectives            To develop RINX, a system that extracts important information from
                                unstructured résumés and stores it in a structured repository for
                                candidate search, shortlisting, workforce analysis, and recruitment
                                support.

 Algorithm/Model




                                RINX uses classical information-extraction methods, including
                                handcrafted extraction patterns, dictionaries or gazetteers, regular
                                expressions, WordNet, and lexical, syntactic, semantic, and domain
                                knowledge. It extracts information such as roles, service lines,
                                technologies, education, employers, and project details. The system can
                                also rank candidates based on a position profile and provide matching
                                justifications.
```

## Source PDF page 9

```text
Data Set
                             The verification set contained 160 free-form IT résumés. The case study
                             processed approximately 65,000 employee résumés from a large IT
                             organization. The résumés were mainly written in English and focused
                             on the IT domain.


Evaluation Metrics
                             The study used precision, recall, and F-measure to evaluate information
                             extraction. It also examined false positives and false negatives. For
                             example, the extracted email information achieved 0.98 recall, 0.93
                             precision, and 0.95 F-measure.


Key Findings                 The study found that RINX can extract and organize information from
                             unstructured and varied résumé formats using handcrafted patterns,
                             gazetteers, regular expressions, and linguistic and domain knowledge. It
                             produced structured candidate information that supported résumé search,
                             candidate shortlisting, competency analysis, workforce profiling,
                             recruitment planning, team formation, and training decisions. However,
                             PDF-to-text conversion errors sometimes caused important information
                             to be missed.

Limitations / Research Gap
                             The approach depends heavily on manually created patterns and
                             domain-specific dictionaries. It primarily focused on English résumés in
                             the IT domain, so it may require adaptation for other industries,
                             languages, and résumé formats. PDF-to-text conversion errors caused
                             some information to be missed, and the system used only limited
                             document-structure information.


Relevance to AYUDA           RINX supports AYUDA’s centralized candidate database by extracting
                             and organizing résumé information such as skills, roles, education, and
                             work experience. Its standardization and search functions can help
                             AYUDA rediscover candidates and compare candidate profiles with
                             client job requirements.

Implement Decision           Adapt. AYUDA may adapt RINX’s structured résumé extraction,
                             candidate search, and skill or role standardization concepts. However,
                             the approach must be updated for Philippine recruitment terms, different
                             industries, modern résumé formats, OCR support, and recruiter
                             verification.

Synthesis
                             Srivastava, Palshikar, and Hingmire (2011) demonstrated that RINX can
                             extract important information from unstructured résumés and organize it
                             into structured records using linguistic knowledge, dictionaries,
                             handcrafted patterns, and regular expressions. The system supported
                             candidate search, shortlisting, workforce analysis, and
                             recruitment-related decisions. However, it mainly focused on English IT
                             résumés and may require adaptation for other industries, languages, and
                             résumé formats.

                             For AYUDA, the study provides a foundation for developing centralized
                             résumé processing, structured candidate profiles, candidate rediscovery,
                             and job matching. The approach should be adapted to Philippine
                             recruitment terms, modern résumé formats, OCR processing, and
                             recruiter verification. Therefore, the study supports AYUDA’s proposed
                             system by showing how automated résumé information extraction can
                             make candidate management and matching more organized and
                             efficient.
```

## Source PDF page 10

```text
Tine: Applicant-facing and bidirectional job recommendations
RRL 11 — NLP-Based Bi-Directional Recommendation System: Towards
Recommending Jobs to Job Seekers and Resumes to Recruiters

Big Data and Cognitive Computing · 2022

This study proposes a bidirectional recommendation approach that recommends vacancies to job seekers
and candidates to recruiters using textual information and similarity calculations.

MDPI

What Tine should investigate: Its NLP pipeline, similarity method, recommendation directions, dataset,
evaluation metrics, and whether explanations are provided.

AYUDA relevance: Closely resembles the three-sided system direction discussed during your professor
consultation, although the paper's recommendation functions are primarily two-sided.

Read RRL 11

NLP-Based Bi-Directional Recommendation System: Towards Recommending Jobs to Job Seekers
                               and Resumes to Recruiters

 Author(s) and Year       Alsaif, S. A., Sassi Hidri, M., Ferjani, I., Eleraky, H. A., & Hidri, A. (2022).
                          NLP-based bi-directional recommendation system: Towards recommending
                          jobs to job seekers and resumes to recruiters. Big Data and Cognitive
                          Computing, 6(4), Article 147. https://doi.org/10.3390/bdcc6040147

 Research Objective       To develop an NLP-based bi-directional recommendation system that
                          recommends suitable jobs to job seekers and relevant candidate resumes to
                          recruiters. The study aims to improve recruitment matching by analyzing
                          skills extracted from resumes and job descriptions, reducing the limitations of
                          traditional keyword-based information retrieval.

 Algorithm / Model
```

## Source PDF page 11

```text
The researchers implemented a Content-Based Filtering (CBF) approach using
                         Natural Language Processing (NLP). The system uses spaCy Named Entity
                         Recognition (NER) to extract information such as skills, education, names,
                         and locations from resumes and job descriptions. It incorporates Word2Vec
                         and cosine similarity for measuring relationships between extracted terms and
                         generating ranked recommendations in both directions. The workflow
                         includes web scraping, text preprocessing, NER training, skill extraction, and
                         similarity-based matching.

Dataset                  The study used two data sources: resume profiles and job postings. 138
                         annotated resumes from the DataTurks GitHub dataset were used for NER
                         training, while 25 resumes from Hire IT People were used for testing.
                         Approximately 250 job descriptions were scraped from Indeed Saudi Arabia,
                         covering Jeddah, Riyadh, and Dammam. The job postings represented five IT
                         roles: PHP Developer, Data Scientist, Data Engineer, Java Developer, and
                         Back-end Developer.

Evaluation Metrics       The researchers used Accuracy, Precision, Recall, and F1-score to evaluate
                         entity recognition and recommendation performance. A confusion matrix was
                         also used to assess classification errors across the five job categories. Cosine
                         similarity was used to calculate matching scores between job profiles and
                         candidate resumes.

Key Findings             The proposed system achieved 80% overall accuracy in classifying 25
                         resumes across five job categories, correctly identifying 20 resumes. The
                         macro-average Precision and Recall were both 0.80, while the F1-score was
                         0.79. For entity recognition, the reported accuracy values were 99.885% for
                         Name, 99.77% for Location, 99.08% for Skills, and 100% for Education. The
                         system successfully generated ranked job recommendations for candidates and
                         ranked candidate recommendations for recruiters. However, Data Engineer
                         classification performed less effectively, with an F1-score of 0.44, partly due
                         to overlapping skills across related IT roles.

Limitations / Research   The study used a relatively small evaluation dataset of 25 resumes and
Gap                      focused on five IT-related positions in Saudi Arabia, limiting generalizability
                         across industries and recruitment environments. The model also experienced
                         difficulty distinguishing roles with overlapping skills, particularly Data
                         Scientist and Data Engineer. The researchers identified the need to incorporate
                         the recency of work experience, improve skill extraction using skill
                         ontologies, and extend geographic matching to neighboring locations.
                         Additionally, the study did not establish performance through real-world
                         recruiter deployment or evaluate long-term recruitment outcomes.

Relevance to AYUDA       The study supports AYUDA's proposed resume parsing, skill extraction,
                         candidate-to-job matching, and candidate rediscovery features. Its NLP-based
                         approach demonstrates how skills and qualifications can be extracted from
                         resumes and compared with job requirements to generate ranked
```

## Source PDF page 12

```text
recommendations. The recruiter-facing recommendation component is
                          particularly relevant to identifying suitable candidates from AYUDA's
                          existing database when new job requests become available.

 Implement Decision       Adapt and Benchmark. AYUDA can adapt the study's NLP-based resume
                          parsing, Named Entity Recognition, and skill-based matching approach. The
                          extracted qualifications can support structured candidate profiles and
                          recommendation explanations. However, the proposed similarity-based
                          matching method should be benchmarked against alternative semantic
                          matching approaches using AYUDA's available recruitment data, particularly
                          for candidates with incomplete resumes or overlapping qualifications.

 Synthesis
                          Alsaif et al. (2022) developed an NLP-based bi-directional recommendation
                          system that uses Content-Based Filtering, Named Entity Recognition,
                          Word2Vec, and cosine similarity to match candidate resumes with job
                          postings. The system extracts relevant information, particularly skills and
                          qualifications, to generate job recommendations for job seekers and candidate
                          recommendations for recruiters. The proposed approach achieved 80%
                          classification accuracy across five IT job categories and demonstrated high
                          accuracy in extracting named entities from resumes. However, the study
                          revealed difficulties in distinguishing job roles with overlapping skills and
                          was evaluated using a relatively small dataset.

                          The study provides a methodological foundation for AYUDA's proposed
                          resume parsing, candidate profiling, and candidate-to-job matching features.
                          Its approach demonstrates how NLP can transform unstructured recruitment
                          documents into structured information that supports candidate
                          recommendations and rediscovery. However, the limitations involving dataset
                          size, overlapping qualifications, and restricted job categories indicate the need
                          for further evaluation. Therefore, AYUDA can adapt the study's NLP-based
                          information extraction and skill-matching techniques while benchmarking
                          more flexible semantic matching methods to improve recommendation
                          reliability across different job positions.




RRL 12 — Modeling Two-Way Selection Preference for Person-Job Fit

Yang et al. · ACM RecSys · 2022

This study investigates person–job fit by modeling selection preferences from both sides of the
recruitment relationship, rather than considering only one party's suitability criteria.

ouci.dntb.gov.ua

What Tine should investigate: How two-way preferences are represented, the model architecture, training
data, evaluation baselines, and how reciprocal preferences differ from simply reversing the direction of
recommendations.

AYUDA relevance: Helps investigate recommendations that consider both the applicant's preferences and
the employer's requirements.

Read RRL 12

                      Modeling Two-Way Selection Preference for Person-Job Fit

 Author(s) and Year       Yang, C., Hou, Y., Song, Y., Zhang, T., Wen, J.-R., & Zhao, W. X. (2022).
                          Modeling two-way selection preference for person-job fit. In Proceedings of
                          the 16th ACM Conference on Recommender Systems (RecSys '22, pp.
                          102–112). Association for Computing Machinery.
                          https://doi.org/10.1145/3523227.3546752

 Research Objective       To improve Person-Job Fit by modeling the two-way selection preferences of
```

## Source PDF page 13

```text
job seekers and employers, rather than relying only on resume–job similarity
                         or one-sided recommendations. The study addresses the problem of
                         unsuccessful matches when only one party is interested in the other.

Algorithm / Model




                         The researchers proposed the Dual-Perspective Graph Neural Network
                         (DPGNN), which combines BERT-based text representations with historical
                         candidate–job interactions. The model constructs a dual-perspective
                         interaction graph that represents each candidate and job through active and
                         passive preference nodes. It uses Graph Convolutional Networks (GCN) with
                         hybrid preference propagation, a quadruple-based ranking loss, and
                         dual-perspective contrastive learning to predict mutual matching preferences.

Dataset                  The study used three real-world recruitment datasets from the online
                         recruitment platform BOSS Zhipin, covering 106 days of interaction logs. The
                         Tech dataset contained 56,634 candidates, 48,090 jobs, and 925,193
                         successful matches. The Sales dataset contained 15,854 candidates, 12,772
                         jobs, and 145,066 matches. The Design dataset contained 12,290 candidates,
                         9,143 jobs, and 166,270 matches. Each dataset included candidate resumes,
                         job descriptions, directed interaction records, and successful matching records.

Evaluation Metrics       The researchers used Recall@5, Precision@5, Normalized Discounted
                         Cumulative Gain (NDCG@5), and Mean Reciprocal Rank (MRR@5) to
                         evaluate recommendation performance in both directions: recommending jobs
                         to candidates and recommending candidates to employers. They also
                         conducted ablation experiments, data sparsity analysis, and hyperparameter
                         sensitivity testing.

Key Findings             DPGNN outperformed most evaluated baseline models across the three
                         datasets, achieving average relative improvements of 7.12% for Tech, 4.81%
                         for Sales, and 7.73% for Design over the strongest baselines, as reported by
                         the authors. For the Tech dataset, it achieved Recall@5 of 0.2941 for
                         candidate recommendations and 0.3430 for job recommendations, with
                         NDCG@5 scores of 0.3119 and 0.4410, respectively. Ablation experiments
                         demonstrated that the dual-perspective interaction graph and quadruple-based
                         ranking loss contributed substantially to performance. The model also
                         performed competitively for users with sparse interaction histories.

Limitations / Research   The model depends on historical candidate–job interactions, which may limit
Gap                      its applicability to new candidates or jobs with little behavioral data. Although
                         the study evaluated interaction sparsity, it did not fully establish performance
                         for completely new users without interaction histories. The researchers also
                         identified the need to incorporate additional recruitment factors, including
                         timestamps, salary expectations, working locations, and sequential behavior
                         histories. Furthermore, the study did not directly evaluate fairness between
                         candidates and employers or validate the system through long-term recruiter
                         deployment.

Relevance to AYUDA       The study supports AYUDA's proposed candidate-to-job matching and
                         candidate rediscovery features by demonstrating the importance of
```

## Source PDF page 14

```text
considering both candidate qualifications and recruitment preferences. Its use
                     of BERT-based text representations provides a basis for semantic matching,
                     while its dual-perspective approach highlights the potential value of
                     considering candidate interest, employer requirements, and historical
                     recruitment interactions. This is particularly relevant to reducing unsuitable
                     recommendations when a candidate appears qualified but may not be
                     interested or available for a position.

Implement Decision   Adapt and Benchmark. AYUDA can adapt the study's principle of two-way
                     recruitment matching by considering both employer requirements and
                     candidate preferences, such as preferred roles, locations, and availability.
                     However, implementing the complete DPGNN architecture is not
                     recommended without first assessing whether AYUDA has sufficient
                     historical interaction data. The study's approach can serve as a benchmark or
                     future enhancement, while simpler semantic matching and preference-based
                     filtering methods may be more practical for initial implementation.

Synthesis
                     Yang et al. (2022) proposed a Dual-Perspective Graph Neural Network
                     (DPGNN) to improve Person-Job Fit by modeling the selection preferences of
                     both job seekers and employers. The model integrates BERT-based textual
                     representations with historical recruitment interactions through a
                     dual-perspective interaction graph, Graph Convolutional Networks,
                     quadruple-based ranking loss, and contrastive learning. Experimental results
                     across three real-world recruitment datasets demonstrated improvements over
                     the evaluated baseline models, with average relative performance gains of
                     7.12% for Tech, 4.81% for Sales, and 7.73% for Design. The findings
                     emphasize that effective recruitment matching should consider mutual
                     preferences rather than relying solely on textual similarity or one-sided
                     recommendations.

                     The study provides a conceptual foundation for AYUDA's proposed
                     candidate-to-job matching and candidate rediscovery features by highlighting
                     the importance of combining candidate qualifications with employer
                     requirements and candidate preferences. However, the model's reliance on
                     historical interaction data and its relatively complex graph-based architecture
                     may limit direct implementation in recruitment environments with insufficient
                     behavioral records. Therefore, AYUDA can adapt the principle of two-way
                     preference matching while benchmarking simpler semantic matching and
                     preference-based filtering approaches before considering more advanced
                     graph-based recommendation models.
```
