# Problem Statement

## Week 5 questions

### Question 1: Chủ đề này đã được nghiên cứu ở đâu, như thế nào?

- The topic of learning risk prediction and early warning systems (EWS) has been extensively researched globally:
  - Geographically: Representative studies have been conducted in Israel (Tel-Aviv University), Taiwan, and aggregated reports from the international SE4AI (Software Engineering for AI) research community.

  - Methodologically: Much of the focus has been on the technical aspects of Machine Learning, using models such as XGBoost, Neural Networks, and Random Forest. Data is primarily extracted from learning management systems (LMS) such as Moodle and student administrative records.

### Question 2: Còn thiếu nghiên cứu trong bối cảnh nào?

- Although the predictive models achieved high accuracy (AUC > 0.85), the literature still points to significant gaps:
  - Lack of standardized Requirements Engineering (RE) processes: Traditional RE methods are not capable of handling the non-deterministic nature of AI. There are currently very few specific guidelines on how to specify data and models for the education sector.

  - Gap between intervention and experimentation: Most research focuses only on building accurate predictive models while neglecting to verify the effectiveness of practical interventions (the Prediction – Intervention – Evaluation cycle).

  - Cultural and ethical context: Lack of research on how cultural factors (such as respect for teacher authority in East Asian cultures) influence the reception of warnings from AI.

### Question 3: Vấn đề thực tế mà nhóm muốn làm rõ là gì?

- The team focused on the challenge of translating educational business needs into reliable technical specifications for AI. Specifically, they explored how to collect and clean data from stakeholders and verify non-functional requirements (NFRs) such as explainability, fairness, hallucination avoidance, and bias to prevent difficulties in administration and negative psychological impact on students. The goal was to minimize bias, enhance personalization and reliability to ensure instructors could trust and utilize intervention suggestions from the system without creating prejudice or psychological pressure on students.

### Question 4: Nhóm sẽ đặt ra những câu hỏi nghiên cứu nào?

- Main Research Question: How can requirements be specified and validated for an early warning system that helps academic advisors identify and support at-risk students?
  - Sub Research Question:
  - RQ1: What requirements should be collected from students, lecturers, and academic advisors to identify early signs of academic risk?

  - RQ2: What functional and non-functional requirements are needed for student risk alerts, personalized support plans, and advisor review?

  - RQ3: How can academic advisors validate whether the warning messages and suggested support plans are useful and understandable?

  - RQ4: How can we collect and specify data ethics and explainability requirements to ensure the system does not cause bias or negatively impact student psychology?

## Problem Statement

- Traditional academic information systems currently operate primarily on a reactive basis, only providing data when poor academic performance has already occurred and is irreversible. The integration of Artificial Intelligence (AI) promises proactive early warning capabilities, helping to identify students at risk of dropping out as early as the first weeks of a semester. However, building these systems faces a core challenge in Requirements Engineering. Traditional RE frameworks, designed for deterministic logic systems, are completely inadequate to handle the probabilistic and data-driven nature of AI. This leads to serious risks:
  - Ambiguity in specifications: There is no standard process for translating faculty expectations into technical constraints for AI models, leading to forecasting bias or hallucination errors.

  - Non-Reliability Flaws (NFRs): Lack of methods to identify and measure explainability and data ethics requirements. If academic advisors don't understand why the AI ​​issues warnings, they won't be able to implement effective personalized interventions.

  - Disconnection between Stakeholders: There is a significant language and goal gap between data engineers (prioritizing model accuracy) and education professionals (prioritizing the practical needs of students).
