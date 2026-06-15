# Paper 06 Summary

## Citation

- **Title:** Predicting Academic Success and Identifying At-Risk Students: A Systematic Review of Data Analytics and Machine Learning Approaches in Higher Education Institutions
- **Authors:** Patrick Ngulube, Mthokozisi Masumbika Ncube
- **Year:** 2025
- **Source:** Google Scholar
- **DOI/Link:** https://www.researchgate.net/profile/Patrick-Ngulube/publication/388481720_Predicting_Academic_Success_and_Identifying_At-Risk_Students_A_Systematic_Review_of_Data_Analytics_and_Machine_Learning_Approaches_in_Higher_Education_Institutions/links/67b930908311ce680c6f60d2/Predicting-Academic-Success-and-Identifying-At-Risk-Students-A-Systematic-Review-of-Data-Analytics-and-Machine-Learning-Approaches-in-Higher-Education-Institutions.pdf

## Problem

- High student dropout and dropout rates: This is a global challenge that affects both developing countries (about 20% of students drop out) and developed countries. Issues such as late graduation and disparities in academic outcomes among diverse student groups are also major obstacles.
- Limitations of traditional methods: Identifying students in need of support currently relies heavily on subjective assessments, limited data sets, and retrospective analyses. This leads to delays in intervention, inaccurate identification of at-risk students, and inequitable allocation of support resources.
- Lack of comprehensive research: Although there has been much research on the application of data and machine learning in education, there is still a lack of comprehensive synthesis on the effectiveness and limitations of these methods in the context of higher education institutions (HEIs).
- Sustainable development goals: This issue becomes even more important as the international community commits to implementing the United Nations Sustainable Development Goals (SDGs), especially SDG 4, which prioritizes quality, inclusive, and equitable education.

## Method

- This paper uses the systematic literature review (SLR) research method:
  - Adherence to PRISMA guidelines: The study strictly adheres to the 2020 PRISMA (Preferred Reporting Items for Systematic Reviews and Meta-Analyses) report to ensure scientific rigor.

  - Utilization of the PICO framework: The authors used the PICO (Population, Intervention, Comparison, Outcome) framework to establish a search strategy and criteria for selecting relevant studies.

  - Quality Assessment using CASP: After initially searching 2414 studies, the authors used the CASP (Critical Appraisal Skills Programme) checklist to assess quality and selected the 33 highest-quality research papers for final analysis.

  - Using supporting tools: The screening process was also supported by specialized software such as Rayyan and ASReview to eliminate duplication and prioritize relevant studies.

## Context

- This paper, conducted in the field of Higher Education, focuses on the application of Data Analytics and Machine Learning (ML) for predictive analytics to identify students at risk of academic difficulty or dropout. It is a systematic literature review adhering to PRISMA 2020 guidelines that synthesizes findings from various data sources, including administrative, learning management systems (LMS), and survey data. The study evaluates a wide range of models, from traditional logistic regression and support vector machines to more advanced ensemble methods and neural networks. On a comprehensive scale, the review analyzed 33 high-quality research articles (selected from an initial pool of 2,414 studies) to provide actionable strategies for Higher Education Institutions (HEIs). The main focus is on facilitating the early identification of at-risk students to support timely interventions, optimize resource allocation, and contribute to Sustainable Development Goal 4 (SDG 4) regarding inclusive and equitable quality education.

## Key Findings

1. Diversity and effectiveness of predictive models: Research indicates a shift from traditional methods such as Logistic Regression to advanced techniques like Ensemble (integrated machine learning) and Neural Networks. These combined methods leverage the strengths of multiple models, minimizing overfitting and significantly improving the accuracy of predicting academic outcomes.

2. Integration of diverse data sources: Building accurate models depends on a combination of administrative data (demographics, scores), data from the LMS system (online interaction), and survey data. This combination provides schools with a multi-dimensional view of student behavior and attitudes, leading to more accurate predictions.

3. Early Identification and Timely Intervention: A key outcome is that machine learning systems can identify students at risk of failure as early as the first few weeks of the semester. This early detection allows universities to implement proactive support measures such as counseling or tutoring before the problem becomes too serious.

4. Personalized Support and Resource Optimization: Machine learning helps universities design support services tailored to the unique needs of each student instead of applying a one-size-fits-all approach. This not only improves student retention rates but also helps universities allocate financial and human resources more efficiently and cost-effectively.

5. Contributing to Sustainable Development Goals: Direct data analytics applications support Sustainable Development Goal (SDG 4) by promoting equity and equality in quality education. This technology helps reduce dropout rates and ensures that all students, regardless of their circumstances, have access to the support they need to succeed.

## Limitations

1. Universality of Research Results: Due to the application of strict selection and exclusion criteria (such as only selecting English-language articles, focusing on higher education), the findings of this paper may be limited in their applicability to all different educational contexts. Readers should assess the relevance of these strategies to their specific organization.

2. Ethical, Privacy, and Bias Issues: The research indicates that ethical aspects of machine learning applications remain unresolved. Issues such as the privacy of students' personal data and algorithmic bias need more attention to ensure predictive models do not cause injustice.

3. Lack of long-term impact studies: The majority of studies reviewed focus only on short-term outcomes within a semester or course. The paper acknowledges the need for more longitudinal studies to truly assess the long-term effectiveness of data-driven interventions on student learning pathways.

4. Gap in interdisciplinary collaboration and new technologies: The paper recognizes the need for closer collaboration among computer scientists, educators, and sociologists. Furthermore, the application of advanced techniques such as natural language processing (NLP) or effective data governance frameworks remains an area requiring further exploration in the future.

## Relevance to our topic

- The basis for the "Early Warning" feature: The article confirms that artificial intelligence (AI) is capable of early identification of at-risk students as early as the first weeks of a semester. A practical example cited in the article is a system that can predict with 74% accuracy after only the first three weeks of school, providing a golden window of opportunity for our system to issue warnings to students and faculty.

- Define diverse stakeholders:
  - For students: Helping them become aware of their learning status early on so they can make proactive adjustments.

  - For faculty: Providing information to implement targeted interventions such as tutoring or academic counseling.

  - For the school: Supporting data-driven decision-making to optimize resource allocation and improve student retention rates across the entire institution.

- Personalized support and learning materials: Our system requires personalized material suggestions and plans, which perfectly aligns with the findings of the paper:
  - Customized learning paths: Machine learning enables the creation of customized educational paths and support services tailored to the unique needs of each individual.

  - Material suggestions: The paper discusses using data from eBooks and interactions on a learning management system (LMS) to understand engagement levels, thereby providing personalized learning interventions.

- Contribute to the "Technical Requirements":
  - AI Model Selection: This paper provides a list of effective algorithms such as Ensemble methods (which improve accuracy) and Neural Networks (for handling complex, multidimensional data).

  - Identifying Input Data Sources: This paper suggests integrating administrative data (demographics, academic history) with behavioral data from the LMS (online interaction) and survey data (attitudes, perceptions) to build a comprehensive feature set for the alert system.

  - Metrics: This paper provides evaluation frameworks such as F1-score, Precision, Recall, and AUC-ROC to incorporate into your technical requirements to ensure reliable system operation, especially to avoid missing students at real risk.
