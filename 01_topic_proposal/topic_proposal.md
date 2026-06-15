# Topic Proposal

## 1. Group Information

- Class: SE2037
- Group: 03
- Leader: Nguyen Trong Toan
- Members: Huynh Viet Phat, Pham Trong Nghia, Vu Tran Phuc Khang, Phan Bao Duy

## 2. Proposed Title

**English title: Requirements Engineering for an AI-based Student Early Warning System.**

**Vietnamese title: Thiết kế yêu cầu kỹ thuật cho hệ thống cảnh báo sớm dành cho học sinh dựa trên trí tuệ nhân tạo.**

## 3. Research Domain

- Research domain: Student Support/ Learning Management/ Smart Education.

## 4. Problem Statement

- Limitations of Current Academic Warning Systems: Traditional Academic Information Systems (AIS) operate reactively and often generate performance data only at the end of a semester when student attrition or course failure is already irreversible. Consequently, stakeholders cannot intervene timely when a student's attendance drops or learning is interrupted.

- The Resource & Recommendation Issues: While massive amounts of educational materials exist, current platforms lack the capability to dynamically map specific student vulnerabilities to precise remedial resources to help struggling students without a clear, personalized recovery roadmap.

- The Requirements Engineering (RE) Challenge (The Core): From a system design perspective, a critical challenge lies in the paradigm shift from traditional code-defined systems to data-driven AI behaviors. Traditional RE frameworks are built to capture deterministic requirements implemented via hard-coded logic. However, integrating AI components introduces significant non-deterministic errors, such as data bias in predictive models (Random Forest) and hallucinations in generative systems (RAG/LLM). Moreover, engineering a reliable system requires continuous collection of training data and stakeholder feedback. This creates a major methodological gap: current RE frameworks lack the formal processes to systematically translate vague stakeholder expectations, domain feedback, and raw academic data into precise technical workflows, mitigation constraints, and functional specifications for AI components.

## 5. Motivation

1. Practical Motivation:

- Academic failure and dropouts cause big problems for both schools and students. For schools, high dropout rates damage their reputation and reduce their financial income. For students, failing a course wastes their time and money, and easily leads to serious mental health issues like stress and depression. By using AI to warn students early, schools can help them in time and reduce these negative impacts before it is too late.

2. Engineering Motivation:

- Building an AI educational system without a clear Requirements Engineering (RE) process is very risky. Without it, engineers might build a flawed AI that gives wrong warnings (causing unnecessary panic for students) or creates incorrect study plans (harming how students learn). Therefore, designing a proper RE framework is the key to success. It ensures the AI system is safe, accurate, and works exactly how teachers and students expect.

## 6. Target Context

1. School managers/ Academic Administrators:

- Role: Monitor overall institutional performance and ensure system data privacy compliance.
- AI Interaction: Rely on macro-level analytics from the predictive model to manage school resources.

2. Teachers/ Academic Advisors:

- Role: Review AI-generated warnings and study plans before they reach students.
- AI Interaction: Provide professional feedback to correct AI errors (hallucinations) and interpret model predictions through explainable interfaces.

3. Students:

- Role: The primary beneficiaries who receive early warnings and personalized remedial roadmaps.
- AI Interaction: Input academic data (grades, attendance) and provide user feedback on the quality of recommended documents to help improve the system.

## 7. Preliminary Research Questions

- RQ1: What requirements should be collected from students, lecturers, and academic advisors to identify early signs of academic risk?

- RQ2: What functional and non-functional requirements are needed for student risk alerts, personalized support plans, and advisor review?

- RQ3: How can academic advisors validate whether the warning messages and suggested support plans are useful and understandable?

## 8. Related Papers (preliminary)

| No  | Title                                                                                                                  | Year | Source                                | Link/DOI                                                                                                        |
| :-- | ---------------------------------------------------------------------------------------------------------------------- | ---- | ------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 1   | Ethical Imperatives and Challenges: Review of the Use of Machine Learning for Predictive Analytics in Higher Education | 2024 | Digital Commons@Lindenwood University | https://digitalcommons.lindenwood.edu/cgi/viewcontent.cgi?article=1645&context=faculty-research-papers          |
| 2   | Student dropout prediction through machine learning optimization: insights from moodle log data                        | 2025 | Scientific Reports                    | https://www.nature.com/articles/s41598-025-93918-1                                                              |
| 3   | Early Prediction of Student Dropout in Higher Education using Machine Learning Models                                  | 2024 | EDM 2024 Short Papers                 | https://www.educationaldatamining.org/edm2024/proceedings/2024.EDM-short-papers.32/2024.EDM-short-papers.32.pdf |
