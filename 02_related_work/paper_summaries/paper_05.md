# Paper 05 Summary

## Citation

- **Title:** How mature is requirements engineering for AI‑based systems? A systematic mapping study on practices, challenges, and future research directions
- **Authors:** Umm-e-Habiba, Markus Haug, Justus Bogner, Stefan Wagner
- **Year:** 2024
- **Source:** Springer
- **DOI/Link:** https://link.springer.com/article/10.1007/s00766-024-00432-3

## Problem

- This paper addresses the core issue of the lack of clarity regarding the current state, maturity, and challenges in Requirements Engineering (RE) for artificial intelligence (AI)-based systems. Specifically, the issues that the paper focuses on clarifying include:
  - High failure rate of AI projects: Data shows that approximately 87% of AI projects never reach production. A major reason is that AI changes the way traditional software development is done (from deductive to inductive), making it difficult to predict and understand system behavior.
  - Inadequateness of traditional RE methods: Existing requirements engineering methods are difficult to apply to AI systems due to their probabilistic nature and the need for continuous adaptation. It remains unclear whether older methods are sufficient or if new methods need to be developed.
  - The emergence of new types of requirements: AI systems present new challenges in defining and validating requirements, such as explainability requirements or newly emerging ethical aspects.
  - The gap between stakeholders: There is a disconnect in communication and accountability between data scientists (who often prioritize data quality) and software engineers or end users (who are concerned with stakeholder requirements).
  - Lack of a comprehensive view of RE4AI research: Prior to this research, the research and practice community lacked a holistic picture of what had been achieved, what practices were available, and what research gaps still needed to be addressed.

## Method

- This paper uses Systematic Mapping Study (SMS) as its primary research method. Specific details regarding the paper's methodology include:
  - Reasons for choosing SMS: The authors chose SMS over Systematic Literature Review because the goal was to capture the overall landscape of the research field, understand the diversity and scope of the studies already conducted, and classify them according to various perspectives.
  - Research Procedure: The study was conducted under the guidance of Petersen et al. The procedure included the following steps:
    - Identifying Research Questions (RQs): Establishing five main research questions to guide the scope of the investigation.

    - Search Strategy: Combining query string search on digital libraries (IEEE Xplore, ACM Digital Library, Google Scholar, Web of Science) and an extended "snowballing" method (both forward and backward) to ensure no important studies were missed.

    - Selection Criteria: Applying strict inclusion and exclusion criteria resulted in the final selection of 126 primary studies for analysis.

  - Data Analysis and Synthesis Methods:
    - Quantitative and Qualitative Analysis: Both were used to classify the collected data.

    - Thematic Analysis: Used to synthesize results and identify challenges and future research directions.

    - Classification Framework: The SWEBOK classification scheme was used for technical requirements topics, and the classification by Wieringa et al. was used to assess research types (such as solution proposals, validation studies, evaluation studies, etc.).

## Context

- This paper, conducted in the field of Software Engineering, focuses on the maturity and landscape of Requirements Engineering (RE) for Artificial Intelligence (AI)-based systems (RE4AI). It is a systematic mapping study combining query string search and extensive snowballing to evaluate the effectiveness of existing and new RE practices across 126 primary studies. The study, on a global research scale, analyzed literature published between 2010 and July 2023 to compare research topics, maturity levels, and methodologies within the SWEBOK framework. The main focus was on addressing the challenges of specifying AI requirements, explainability, and the communication gap between ML engineers and end-users to support the development of more reliable AI systems and optimize project success rates.

## Key Findings

1. Strong Growth in the RE4AI Field (RQ1): Research shows that this field began to emerge in 2017 and has seen a steady increase in the number of publications each year. While academia remains dominant, interest from industry (such as IBM and Fujitsu) has increased significantly since 2019, particularly with the recent explosion of large language models (LLMs).

2. Uneven Distribution of Topics (RQ2): The majority of research focuses on the Requirements Analysis (104 papers) and Requirements Inspiration (87 papers) phases. Conversely, aspects of requirements engineering tools and fundamentals have not received adequate attention, indicating that the field is in a transition from traditional methods to AI-specific solutions.

3. Research Maturity is Limited (RQ3): The majority of papers (74) stop at the "Solution Proposal" stage and are primarily validated through case studies rather than extensive real-world testing. The RE4AI field is considered relatively young and lacks rigorous empirical evaluation in a real-world industrial environment.

4. Combination of Traditional and New Practices (RQ4): Traditional techniques such as semi-structured interviews are still commonly used to elicit requirements. However, many new practices (processes, models) have been proposed to address AI-specific issues such as explainability, ethical aspects, and the need for human-centered design.

5. Key Challenges (RQ5): The paper identifies 27 challenges divided into 9 groups, the most prominent of which is the difficulty in defining specific requirements due to the probabilistic nature of AI. Additionally, the knowledge and communication gap between machine learning engineers (ML engineers) and end users is also a major obstacle to project failure.

6. Seven Potential Future Research Directions: The authors propose new directions including: integrating human knowledge into AI system development, adapting legacy requirements frameworks (such as GORE) to AI, and focusing on validating non-functional requirements (such as fairness and security) in a constantly changing environment.

## Limitations

1. Internal Validity: Establishing search queries, selecting search engines, and applying inclusion/exclusion criteria can lead to the omission or inclusion of irrelevant documents. Furthermore, although the research team attempted to minimize researcher bias by having multiple individuals conduct independent reviews, the data screening and extraction process could still be influenced by subjective viewpoints.

2. Data Analysis Challenges: Another limitation is that the initial data analysis was performed by a single researcher. While the results were later discussed and refined by the team, relying on one person at this early stage could still create potential errors in data interpretation.

3. External Validity: The authors acknowledge the risk of not capturing all primary research in the RE4AI field. Despite applying a "snowballing" method until saturation to increase coverage, there is still a possibility that important papers using inconsistent terminology may be missed, affecting the overall coverage of the study.

4. Contextual Limitation: An objective limitation pointed out in the paper is that the RE4AI field is still relatively young. Most of the research surveyed stopped at the "Proposal of Solution" stage and lacked rigorous validation in an industrial environment. This limits the ability to draw immediate, practical conclusions for practitioners.

5. Lack of fundamental aspects: The paper also notes that current research focuses too much on the early stages (initiation, analysis) while neglecting fundamental principles, overall processes, and AI-specific support tools. This imbalance leaves significant gaps in the overall picture of RE4AI.

## Relevance to our topic

- Solving the Explainability (XAI) Problem: Our system not only provides warnings but also suggests support materials and plans. The paper emphasizes explainability as a core non-functional requirement (NFR) of AI.
  - For teachers and schools: They need to understand why the system assesses a student as at risk in order to make accurate intervention decisions.

  - For students: Suggested materials need to include reasons why they are relevant to their current situation to increase persuasiveness. The paper provides new frameworks and methods for extracting these explainability requirements from the user.

- Bridging the Stakeholder Gap: Our project has a very diverse user base: students, faculty, and schools. This paper identifies a major challenge in RE4AI as the communication and knowledge gap between AI engineers (model builders) and end users (those who understand the educational business).
  - Building Personas (User Models): To understand the different needs of instructors compared to students when receiving alerts.

  - Semi-structured interviews and scenario-based design: To elicit personalized requests tailored to each student's state.

- Managing Non-Functional Requirements (NFRs): In an early warning system for education, requirements such as fairness, safety, and ethics are extremely important. This paper points out that traditional methods are insufficient to verify these factors in AI. This resource will help us identify risks such as whether the algorithm is biased towards a particular group of students, and how to design technical requirements to mitigate this from the outset.
- Implement new RE practices:
  - Modeling data as a request source: Because alert quality depends on learning and behavioral data from the LMS, we need specific technical requirements for data collection and labeling.

  - Continuous RE loop: Since student states change over time, system requirements also need to be dynamically adjusted rather than defined once as in traditional software.
