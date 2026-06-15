# Paper 07 Summary

## Citation

- **Title:** Developing an Early Warning System with Personalized Interventions to Enhance Academic Outcomes for At-Risk Students in Taiwanese Higher Education
- **Authors:** Yuan-Hsun Chang, Feng-Chueh Chen, Chien-I Lee
- **Year:** 2025
- **Source:** Google Scholar
- **DOI/Link:** https://www.mdpi.com/2227-7102/15/10/1321

## Problem

- This paper focuses on addressing core issues related to supporting students at risk of academic underperformance within the context of higher education in Taiwan. Specifically, the main issues include:
  - The delays of traditional warning systems: Conventional academic warning systems often rely on end-of-semester grades, which causes significant delays and limits opportunities for timely intervention to support students before it's too late. The current approach is more reactive than proactive.

  - The challenge from the expansion of higher education in Taiwan: The shift from an elite to a mass education model, coupled with a declining birth rate, has led to a shortage of academic preparation among newly enrolled students. The university enrollment rate in Taiwan has increased from 70% in 2000 to nearly 98% in 2024, creating diversity but also causing significant disparities in academic ability and motivation.
  - Cultural barriers stemming from Confucianism: In the Taiwanese context, Confucian values ​​emphasize the authority of teachers and the expectation that students will overcome difficulties on their own. This makes developing proactive, data-driven support systems not only a technical challenge but also a crucial socio-cultural need.

  - Gap in current research: The majority of current studies focus only on improving the accuracy of predictions, lacking empirical validation of the effectiveness of interventions.

## Method

- This paper uses a sequential two-phase quantitative research design to address the research questions. Specifically, it follows these steps:
  1. Phase I: Building and Validating the Predictive Model:
  - Utilizing Educational Data Mining (EDM) and Machine Learning methods.

  - Data was extracted from the Learning Management System (LMS) and Student Information System (SIS) of 2,856 students across 64 courses.

  - Algorithms compared included Decision Trees, Random Forests, and XGBoost to find the optimal model for identifying students at risk of academic underperformance.
  2. Phase II: Quasi-experimental design:
  - After building the model, the paper conducted a quasi-experimental experiment (n = 48) to evaluate the effectiveness of the interventions.

  - Students were divided into an experimental group (receiving personalized intervention when the alert system was activated) and a control group (learning according to the normal procedure).

  - Statistical methods such as t-test and analysis of covariates (ANCOVA) were used to compare learning outcomes between the two groups to determine the true impact of the alert system and the intervention.

## Context

- This paper, conducted in the field of Higher Education in Taiwan, focuses on the application of Educational Data Mining and Machine Learning (ML) to develop an early warning system for identifying students at risk of academic failure. It utilizes a sequential two-phase research design combining administrative data from a Student Information System (SIS) and behavioral traces from a Learning Management System (LMS) to evaluate the predictive performance of models such as Decision Trees, Random Forest, and XGBoost. The study, conducted at a comprehensive university, analyzed data from 2,856 students across 64 courses to construct robust, course-specific predictive models. The main focus was on bridging the gap between prediction and intervention by addressing the trade-off between early prediction (at week 6) and model accuracy (achieving an AUC of 0.85) to support timely, culturally responsive interventions tailored to Confucian educational values.

## Key Findings

1. Outstanding predictive model performance:

- The model achieved a balanced AUC of 0.85, indicating good differentiation between at-risk and normal students.

- The most important predictive variables included: previous semester grades, attendance rate, and timely assignment submission patterns.

2. Significant intervention effectiveness (Most important finding):

- Impressive pass rate: 73% of students in the at-risk group (experimental group) achieved a passing grade (≥ 60 points) after receiving the intervention. This is significantly higher than the historical success rate of approximately 55% (corresponding to a failure rate of 45%).

- Strong improvement in academic performance: The intervention group showed an average score increase of 18.77 points with a large effect size (Cohen’s d = 0.91).

- Narrowing the gap: The learning ability gap between the at-risk group and the normal group narrowed significantly after the intervention (group-determined score variability decreased from 51% on the pre-test to 10.1% on the post-test).

3. Unexpected findings regarding the control group:

- While the at-risk group progressed, the control group (students initially not subject to the warning system) experienced an average score drop of 10.50 points. This underscores the importance of continuous monitoring, as students who stabilize mid-term may still struggle later.

4. Cultural and systemic value:

- Cultural relevance: The study demonstrates that in the Taiwanese context, teacher- or mentor-led interventions have a stronger impact due to the influence of Confucian values ​​(respect for authority and collectivism) compared to Western autonomous models.

- Closed-loop validation: The paper successfully completed and validated the full cycle: Prediction – Intervention – Evaluation, something very few previous studies have achieved.

## Limitations

1. Limitations in research design (Lack of randomization): Due to ethical constraints (the inability to refuse support to students identified as at risk), the study used a quasi-experimental design instead of a randomized controlled trial (RCT). This limited the ability to fully control for confounding variables such as personal motivation or personality traits, resulting in the study establishing an association rather than definitive evidence of causality.
2. Narrow scope of implementation: The intervention phase was only carried out on a single general education course (History of Physical Education) with one cooperating instructor. Therefore, this result can be considered a "local success" and its effectiveness cannot yet be confirmed across all types of courses or different organizations.
3. Lack of cultural benchmarks: The study lacked a parallel control group representing different cultural orientations (e.g., Western contexts emphasizing autonomy). Therefore, it is difficult to definitively distinguish whether the program's success was due to cultural adaptation or simply to having a structured support system.
4. Lack of long-term data: Current assessments focus only on short-term outcomes within a single semester. The paper acknowledges the lack of longitudinal studies to assess the sustainability of intervention effects on students' long-term learning trajectories or self-regulation skill development.
5. Data quality dependence: The effectiveness of the predictive model (H1) depends heavily on the completeness and reliability of the data at the course level. If the data from the LMS system or student records is incomplete, the accuracy of early warning will be significantly reduced.
6. Generalization: While the research makes a significant contribution to the non-Western educational context, the authors also note that algorithmic thresholds and intervention protocols need further localization to suit diverse linguistic and socio-cultural environments.

## Relevance to our topic

- Technical requirements and input data design: This paper identifies specific data requirements for an AI system to make accurate predictions, including:
  - Administrative data (SIS): Previous semester grades, student background characteristics.

  - Real-time behavioral data (LMS): Attendance rate, on-time assignment submission patterns.

  - Technical analysis: Using Information Value (IV) to filter significant variables and comparing algorithms (Decision Tree, Random Forest, XGBoost) to select the optimal model in terms of both accuracy and interpretability—a crucial technical requirement for instructors to understand why students receive warnings.

- Multi-stakeholder alert mechanism (Students, Faculty, School): Our project aims to notify multiple parties, and this paper has implemented that process precisely through a multi-tiered support system:
  - Alert activation: When the AI ​​system detects a risk in week 6, a notification is immediately sent to the responsible faculty member.

  - Information for the school: A list of at-risk students is forwarded to the faculty academic advisor and functional units such as the Teaching and Learning Development Center or the Psychological Counseling Center.

  - Student feedback: Notifications are designed to be "empowering," encouraging students to self-feedback and seek help instead of putting psychological pressure on them.

- Personalized support plans and learning materials: The paper demonstrates the requirement for a "personalized support plan" that we are referring to:
  - State-based interventions: Depending on the cause of the risk (academic or psychological), students will receive different support such as: remedial instruction, one-on-one tutoring, or in-depth psychological counseling.

  - Material suggestions: The system in the paper acts as a "learning environment" providing timely feedback to promote students' self-regulation abilities.

- Socio-Technical Framework: This is the most deeply relevant point. The paper emphasizes that an AI-based EWS system is not just a purely technical tool, but a socio-technical system:
  - Coordination: AI technology is only truly effective when embedded in a network of human support (instructors, mentors) and aligned with the culture (e.g., a culture that values ​​teacher instruction in the East Asian context).

  - Closed-loop cycle: The paper validates the "Prediction – Intervention – Evaluation" cycle, providing a basis for designing requirements not only for the software but also for the system's operational processes in practice.
