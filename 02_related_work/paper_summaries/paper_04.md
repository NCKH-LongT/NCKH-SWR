# Paper 04 Summary

## Citation

- **Title:** Requirements Engineering for Machine Learning-Based AI Systems: A Tertiary Study
- **Authors:** Mariana Crisostomo Martins, Lívia Mancine C. Campos, João Lucas R. Soares, Taciana Novo Kudo, Renato F. Bulcão-Neto
- **Year:** 2025
- **Source:** Journal of Software Engineering Research and Development (JSERD)
- **DOI/Link:** https://doi.org/10.5753/jserd.2025.4892

## Problem

- The paper addresses the mismatch and lack of integration between traditional Requirements Engineering (RE) practices and the unique characteristics of Machine Learning (ML)-based AI systems. The behavior of ML systems is inherently data-driven and uncertain, rendering conventional, deterministic software requirements engineering methodologies inadequate. 
- While numerous primary and secondary studies (such as systematic mapping studies and literature reviews) have investigated Requirements Engineering for Machine Learning (RE4ML), the literature remained fragmented. Prior to this work, no tertiary study had comprehensively synthesized the existing secondary literature to assess study quality, compile common solutions, map challenges, and establish a unified research agenda.

## Method

- The authors conducted a systematic tertiary study (a review of secondary studies) following established guidelines in software engineering (Kitchenham et al., Cruzes & Dybå, and Kudo et al.):
  - **Search Strategy:** Executed an automatic search query across six major digital libraries (ACM Digital Library, IEEE Xplore, Scopus, Engineering Village, Wiley, and Web of Science), supplemented by recursive backward and forward snowballing.
  - **Study Selection:** Applied strict inclusion and exclusion criteria to select 9 high-quality secondary studies published between 2019 and 2023.
  - **Quality Assessment:** Evaluated the selected secondary studies using 8 quality criteria (QC) adapted from the Centre for Reviews and Dissemination (CDR).
  - **Synthesis:** Categorized and synthesized the findings based on the core RE activities defined in the SWEBOK v4.0 framework (elicitation, analysis, specification, validation, and management).

## Context

- The research is situated within the global Software Engineering for AI (SE4AI) and RE4ML domain. It evaluates RE activities across various software systems that integrate ML components, with a strong focus on high-stakes and safety-critical application domains such as autonomous driving, computer vision, aviation, and healthcare. The study investigates how software development teams, data scientists, and domain experts collaborate under the technical uncertainties of data-driven systems.

## Key Findings

- **RE Phase Imbalance:** The majority of existing research concentrates on the Requirements Elicitation and Specification phases, whereas Requirements Validation and Management remain severely under-researched.
- **Critical Non-Functional Requirements (NFRs):** The synthesis highlights that explainability, transparency, trust, safety, security, fairness, privacy, and reliability are the most crucial and frequently discussed NFRs in ML-based systems.
- **Elicitation & Specification Approaches:** Brainstorming and ad-hoc methods are the most common elicitation techniques. For specification, goal-oriented requirements engineering (GORE) frameworks (such as GR4ML) and UML-based modeling are the most prevalent, alongside specifying requirements as experimental hypotheses.
- **Major Gaps & Challenges:**
  - Lack of standardized, integrated tool support and tailored methodologies for RE4ML.
  - High difficulty in specifying data-specific requirements (e.g., data quality, completeness, and bias).
  - Inadequate traceability between requirements, datasets, and model versions.
  - Poor collaboration and communication gaps between traditional software engineers and data scientists due to differing vocabularies and expectations.
- **Research Agenda:** The study proposes a 9-point research agenda targeting critical areas such as NFR trade-offs, traceability, performance metrics, and industry-academic collaboration.

## Limitations

- **Timeline Constraint:** The search process was completed in October 2023, meaning that secondary studies published in late 2023, 2024, or 2025 were not included in the analysis.
- **Primary/Secondary Study Dependency:** As a tertiary study, the validity and generalizability of the findings are inherently limited by the quality, accuracy, and biases of the original secondary and primary studies it synthesizes (e.g., the scarcity of large-scale industrial validation in primary studies).

## Relevance to our topic

- **Guidance for Non-Functional Requirements (NFRs):** For our Student Early Warning System (SEWS), this study underscores that we cannot treat the machine learning model as a black box. We must formally specify NFRs such as explainability (how risk predictions are explained to academic advisors) and fairness (ensuring predictions do not introduce bias against specific student demographics).
- **Data & Model Specification:** It guides our team to document and specify data requirements (e.g., student attendance records, LMS activity patterns) and model requirements separately, treating model performance thresholds as testable hypotheses.
- **Mitigating Communication Gaps:** It serves as a reminder to establish clear, shared terminologies between our software developers (handling the frontend and warning pipeline) and data scientists (handling the risk prediction models) to avoid integration failures.
