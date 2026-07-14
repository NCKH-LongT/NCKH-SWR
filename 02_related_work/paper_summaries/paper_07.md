# Paper 07 Summary

## Citation

- **Title:** Lecturers' adoption to use the online Learning Management System (LMS): Empirical evidence from TAM2 model for Vietnam
- **Authors:** Bui Thanh Khoa, Nguyen Minh Ha, Tran Viet Hoang Nguyen, Nguyen Huu Bich
- **Year:** 2020
- **Source:** Ho Chi Minh City Open University Journal of Science – Economics and Business Administration, Vol. 10, No. 1, pp. 3-17
- **DOI/Link:** https://doi.org/10.46223/HCMCOUJS.econ.en.10.1.216.2020

## Problem

While online Learning Management Systems have been widely introduced in higher education institutions globally, actual adoption and active use by lecturers in Vietnam remains limited. Online training has historically been treated as a secondary option alongside offline training, with both students and lecturers preferring face-to-face instruction. The COVID-19 pandemic forced a rapid shift to online learning, making LMS adoption no longer optional but urgent. However, the barriers preventing Vietnamese lecturers from adopting LMS platforms — including technical difficulty, misalignment with pedagogical workflows, and increased workload in preparing digital content — had not been systematically studied in the Vietnamese context prior to this paper.

## Research Methodology

This study uses a mixed methods design combining qualitative and quantitative approaches. Online group discussions were first conducted to explore lecturer perceptions and refine the theoretical model. Online surveys were then administered to collect data from lecturers across Vietnamese universities for quantitative hypothesis testing. The theoretical model is based on TAM2 (Technology Acceptance Model 2) and structural equation modeling is used to analyze relationships between constructs.

## Method

The study applies the **Technology Acceptance Model 2 (TAM2)** to investigate factors affecting Vietnamese lecturers' intention to adopt and use online LMS platforms. The research model includes the following TAM2 constructs tested as hypotheses:
- **Perceived Usefulness (PU):** The extent to which lecturers believe LMS use enhances their work performance.
- **Perceived Ease of Use (PEOU):** The extent to which lecturers believe LMS use requires minimal effort.
- **Subjective Norm (SN):** Social pressure from peers, management, and institutional culture influencing adoption.
- **Image:** Whether using the LMS improves the lecturer's status or reputation among colleagues.
- **Job Relevance:** Whether the LMS is relevant to the lecturer's specific teaching tasks.
- **Output Quality:** Whether the LMS produces outputs that meet the lecturer's pedagogical standards.
- **Result Demonstrability:** Whether the results of using the LMS are visible and communicable to others.

The theoretical model hypothesizes relationships between these constructs and lecturers' adoption intention, following the structure established by Venkatesh and Davis (2000) in the original TAM2.

## Dataset

- **Participants:** Lecturers from multiple Vietnamese universities.
- **Data Collection:** Online group discussions followed by online surveys conducted during the COVID-19 pandemic period (2020).
- **Context:** Higher education institutions in Vietnam during a period of forced transition to online learning due to social distancing measures.

## Evaluation

The study tests the hypothesized TAM2 model through structural equation modeling (SEM) applied to the survey data. Hypotheses are evaluated based on the significance and direction of relationships between constructs. The fit of the theoretical model to the Vietnamese LMS adoption context is assessed against the standard TAM2 conclusions from prior international literature.

## Results

1. **Adoption Predictors Confirmed:** The study confirmed that lecturers' adoption intention to use the LMS is significantly impacted by perceived usefulness, perceived ease of use, and subjective norm — consistent with TAM2 conclusions.
2. **Subjective Norm → Image:** Subjective norm has a positive impact on lecturers' image, meaning that social pressure to use the LMS also improves how lecturers are perceived by peers.
3. **Perceived Usefulness Determinants:** Perceived usefulness of the LMS is determined by perceived ease of use, subjective norm, lecturers' image, job relevance, output quality, and result demonstrability — all six factors positively contribute.
4. **Workload as a Barrier:** Lecturer workload in creating and managing digital content for LMS platforms is identified as a major bottleneck affecting both perceived usefulness and adoption intention.
5. **Managerial Implications:** The study proposes institutional strategies to improve LMS adoption, focusing on reducing workload barriers, improving output quality perception, and demonstrating tangible results from LMS use.

## Limitations

- **Survey-Based Only:** The quantitative findings are based on self-reported survey data and do not capture actual LMS usage behavior or performance outcomes.
- **No AI Integration Evaluated:** The study does not evaluate technical enhancements such as AI integrations that could directly resolve the adoption barriers identified — leaving a gap between the identified problems and possible solutions.
- **Specific Context:** The findings are limited to the Vietnamese university context during the COVID-19 pandemic and may not fully generalize to post-pandemic or other national contexts.

## Relevance to our topic

This paper is relevant to our requirements engineering focus in two ways. First, it provides the only empirical evidence in our literature set about what Vietnamese lecturers actually value in an LMS — output quality, result demonstrability, ease of use, and workload reduction. These TAM2 constructs are directly translatable into non-functional requirements for an AI-assisted LMS in the Vietnamese higher education context, but no paper has made this translation. Second, the identification of lecturer workload as the primary adoption barrier directly supports the motivation for formally specifying functional requirements for automating quiz generation and feedback in a RAG-based LMS, grounding the requirements in empirically validated stakeholder needs rather than assumptions.

## Possible Improvement

- **Translate TAM2 Findings into NFRs:** Future work should translate the empirically validated TAM2 constructs — output quality, ease of use, workload reduction, result demonstrability — into formally specified non-functional requirements for AI-assisted LMS systems targeting Vietnamese higher education.
- **Post-Pandemic Follow-Up:** A follow-up study evaluating lecturers' adoption of AI-assisted LMS features (such as automated quiz generation) using the same TAM2 framework would provide direct evidence for or against the requirements specified in our study.
