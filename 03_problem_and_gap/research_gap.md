# Research Gap

## Group Information

- Class: SE2037
- Group: 03
- Leader: Nguyen Trong Toan
- Members: Huynh Viet Phat, Pham Trong Nghia, Vu Tran Phuc Khang, Phan Bao Duy

## Gap

- Each research gap below is derived from an analysis of the Limitations and Key Findings sections of seven academic papers, aiming to answer the question: "What have previous studies acknowledged they haven't—and what unanswered questions does that leave for our group's topic?"

### Gap 1 - Lack of standardized Requirements Engineering (RE) processes for AI in the educational context.

- Derived from: Paper 03, Paper 04, Paper 05.

- Paper 03 (Franch et al., 2023) presents a vision of the role of RE in AI systems but acknowledges that this is only a theoretical framework (Vision Paper), lacking empirical evidence and risking creating an information "bottleneck" if it focuses only on the role of requirements engineers. Paper 04 (Martins et al., 2025) and Paper 05 (Habiba et al., 2024), through comprehensive studies (Tertiary Study/SMS), indicate that the RE4AI field is currently extremely unbalanced: largely focused on Elicitation and Specification, while Validation and Requirements Management for AI systems are almost completely neglected.

- The gap: Currently, there is no comprehensive and proven RE process to translate pedagogical needs (of instructors/mentors) into technical specifications for AI models, particularly lacking verification steps to see if these requirements actually help reduce the rate of high-risk students.

### Gap 2 - Important non-functional requirements (NFRs) such as explainability and ethics lack technical measurement standards.

- Derived from: Paper 01, Paper 04, Paper 06.

- Paper 01 (Barnes et al., 2024) emphasizes the importance of ethics and privacy but acknowledges that these issues still heavily depend on data quality and the lack of specific governance frameworks for each educational institution. Paper 06 (Ngulube & Ncube, 2025) identifies that issues of algorithmic bias and privacy in ML for education remain "unresolved" in current research.

- The gap: Although studies affirm that explainability and fairness are mandatory, no paper defines a specific set of "System Requirements": How to measure explainability for an academic advisor? What is the acceptable threshold for "hallucination" errors in intervention suggestions?

### Gap 3 - The disconnect between model accuracy and the optimal timing for real-world intervention.

- Derived from: Paper 2, Paper 7.

- Paper 2 (Goren et al., 2024) reports that the highest accuracy of the model (AUC) is at the end of the semester (when exam scores are available), but at that point, "there is very little time left for intervention." Paper 7 (Chang et al., 2025) attempts intervention in week 6 but acknowledges that this result is only "local success" in a single subject and depends entirely on the voluntary cooperation of the instructor.

- The gap: Current studies focus too much on optimizing the algorithm (Accuracy/AUC) while neglecting to establish Temporal Requirements: At what week does the system need minimum data to provide a sufficiently reliable warning that is still early enough for academic advisors to act effectively?

### Gap 4 - There is a lack of empirical evidence regarding the long-term "Prediction – Intervention – Evaluation" cycle.

- Derived from: Paper 6, Paper 7.

- Paper 6 (Ngulube & Ncube, 2025) indicates that most current studies only focus on short-term success prediction, lacking longitudinal studies to assess the impact of AI alerts on students' overall learning journey. Paper 7 (Chang et al., 2025) is a rare paper that implements an intervention but lacks randomization due to ethical barriers, making it impossible to definitively establish a causal relationship between AI alerts and student outcomes.

- The gap: No studies have yet combined a structured RE process with a long-term clinical trial to demonstrate that proper implementation of technical requirements from the outset leads to a sustained improvement in student retention rates.

## Summary Table

| Gap                                                          | Related Papers | Evidence from Limitations / Findings                                                                                    | What Remains Missing (Gap)                                                                                               |
| :----------------------------------------------------------- | -------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| G1: Lack of a comprehensive RE process.                      | P03, P04, P05  | The research mostly focuses on proposing solutions, lacking validation within the education industry.                   | A standardized RE process focuses on Validation and Management for the EWS system.                                       |
| G2: NFRs on Explainability & Ethics are not specific enough. | P01, P04, P06  | "Ethics and algorithmic biases have not been fully resolved," and there is a lack of a technical measurement framework. | Detailed technical specifications for Explainability (XAI) and anti-Hallucination constraints.                           |
| G3: The Trade-off Between Accuracy and Timing.               | P02, P07       | The most accurate model is used when it is already too late for effective intervention.                                 | The requirements include "golden timing" and minimum input data to balance accuracy and timeliness.                      |
| G4: Lack of validation of long-term cycles.                  | P06, P07       | Lack of longitudinal studies and randomized allocation; results are only locally successful.                            | Empirical evidence demonstrates the link between requirements design processes and long-term intervention effectiveness. |
