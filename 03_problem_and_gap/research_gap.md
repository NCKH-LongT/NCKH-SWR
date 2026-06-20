# Research Gap

## Group Information

- **Class:** SE2037
- **Group:** 04
- **Leader:** Nguyễn Hoàng Anh Khoa
- **Members:** Trần Anh Vinh, Phan Phúc Thịnh, Nguyễn Thị Quỳnh Trúc, Nguyễn Quang Trường

---

## How to Read This Section

Each gap below is derived by reading the **Limitations** and **Possible Improvement** sections of each paper summary, then asking:
> *"What does this paper admit it could not do — and what does that leave unresolved for our research topic?"*

---

## Gap 1: Automated Question Generation Systems Do Not Link Generated Questions to Specific Course Learning Outcomes (CLOs)

**Derived from:** Paper 01, Paper 02, Paper 03

**Paper 01 (Chen & Shiu, 2025)** integrates Bloom's Taxonomy and Item Response Theory (IRT) to control cognitive difficulty, but the system was deployed for professional certification exams at Taiwan's National Institute of Environmental Research — not in a university LMS context with a syllabus-defined CLO structure. No step in the system requires the user to select a specific CLO before generating questions.

**Paper 02 (Maity et al., 2025)** explicitly acknowledges this in its Possible Improvement section: *"Adjust the few-shot examples in the Hybrid Model's prompt to directly reflect the cognitive levels required by the selected Course Learning Outcomes (CLOs)"* — confirming that CLO alignment was not implemented and is identified as a necessary next step.

**Paper 03 (Hamidi et al., 2025)** similarly states in its Possible Improvement section: *"Configure prompts and the knowledge base to allow the system to generate multi-domain questions in Vietnamese/English aligned with CLOs"* — confirming that the current system has no CLO alignment mechanism.

**The gap:** None of the seven papers implements a workflow where an instructor selects a target CLO from the course syllabus → the system generates questions targeting that CLO → each generated question is tagged with the CLO for coverage tracking. This gap is directly confirmed by the papers themselves.

---

## Gap 2: The Instructor Review Step Exists in Practice But Is Not Specified as a Set of System Requirements

**Derived from:** Paper 02, Paper 03

**Paper 03 (Hamidi et al., 2025)** describes a human-in-the-loop expert review step as part of its research methodology, and provides a Next.js interface that allows instructors to edit and approve generated questions. However, the Limitations section notes: *"The quality of the generated questions has not been verified using standard automated RAG evaluation frameworks (such as Ragas)"* — meaning there is no automated mechanism to alert instructors when a generated question is of low quality. The paper also reports approximately 10% schema deviation (the model failing to follow the JSON output template) and around 15% difficulty misalignment, but does not describe how the system handles these cases.

**Paper 02 (Maity et al., 2025)** states directly in its Limitations: *"The system does not integrate a direct review or edit interface for teachers before publishing questions to an LMS"* — acknowledging this as an explicit gap.

**The gap:** Paper 03 has a review interface, but it is described as a research procedure, not as a formally specified set of functional requirements. No paper defines: what edits the instructor can make to a generated question; what happens when a question is rejected; what the system should display when schema deviation or difficulty misalignment is detected; or whether instructor approval is required before questions are visible to students. Paper 02 lacks even a review interface.

---

## Gap 3: LLM-Generated Feedback Has a 35% Error Rate But No Quality Control Requirements Are Specified

**Derived from:** Paper 04

**Paper 04 (Reddig et al., 2025)** reports in its Results section: *"35% of hints were rated as erroneous because they were too general, explained concepts incorrectly, or directly revealed the correct answer (bottom-out hint), defeating the pedagogical purpose of self-study."* The paper also notes: *"Only 35% of the feedback passed the automated simulated student usefulness test."*

The Limitations section explicitly states two problems:
- *"An error rate of 35% in generated hints or answer leaks is too high for a fully automated real-world educational deployment."*
- *"Lack of RAG: The system relies entirely on zero-shot/few-shot prompts without integrating RAG to retrieve background knowledge from course materials."*

The Possible Improvement section proposes: *"Integrate RAG to retrieve formulas, definitions, or specific lecture slides related to the student's error"* — confirming that the absence of RAG is identified as the primary cause of feedback errors.

**The gap:** Paper 04 provides clear quantitative evidence that LLM-generated feedback is unreliable at a 35% error rate, but does not specify what system requirements would address this: what confidence threshold should trigger a quality alert, how the instructor should be notified, and which feedback items are sent directly to students versus which require prior review.

---

## Gap 4: The CLO-Aligned Feedback Framework in SE Education Requires Heavy Manual Effort and Has Not Been Automated

**Derived from:** Paper 06

**Paper 06 (Modi et al., 2023)** proposes the "Focus" framework, which models learning objectives and relates feedback across different software engineering tasks to help students see their overall CLO progress. However, the Limitations section states: *"The framework's success depends on the initial mapping of CLOs to specific course tasks, which requires significant effort from instructors."* The paper also notes it was *"evaluated in a limited number of class cohorts."*

Paper 06 does not use AI or RAG to automate any part of the process — CLO mapping and feedback generation are both performed manually by instructors.

**The gap:** Paper 06 establishes the need for CLO-aligned personalized feedback in software engineering education but admits that manual implementation is costly and does not scale. No paper in the reviewed set connects a CLO-tracking framework like "Focus" with a RAG system that automates both steps: generating CLO-tagged questions and producing feedback grounded in course materials.

---

## Gap 5: LMS Adoption Research in Vietnam Does Not Cover AI-Assisted Features and Does Not Translate Findings into System Requirements

**Derived from:** Paper 07

**Paper 07 (Bui Thanh Khoa et al., 2020)** applies TAM2 to investigate Vietnamese lecturers' intention to adopt LMS platforms, finding that lecturer workload in creating and managing digital content is a major bottleneck. The study identifies output quality and result demonstrability as significant predictors of perceived usefulness.

However, the Limitations section states directly: *"The study is limited to the survey dataset from specific Vietnamese universities and does not evaluate technical enhancements (like AI integrations) that could resolve these adoption barriers."*

**The gap:** Paper 07 identifies instructor workload as the primary barrier to LMS adoption in Vietnam but stops there. No paper in the reviewed set tests whether a RAG-based quiz generation system reduces that workload in the Vietnamese context, and no paper translates the TAM2 factors (output quality, result demonstrability, ease of use) into concrete non-functional requirements for an AI-assisted LMS feature.

---

## Gap 6: Technically Advanced Systems Are Too Complex to Integrate into Lightweight LMS Platforms

**Derived from:** Paper 01

**Paper 01 (Chen & Shiu, 2025)** states in its Limitations section: *"Setting up knowledge graphs and the multi-agent system combined with the DDS communication protocol requires substantial computing resources and complex engineering, making it difficult to integrate directly into lightweight LMS platforms."*

The Possible Improvement section proposes: *"Remove the complex DDS mechanism and replace it with a sequential RAG workflow integrated directly into the LMS API to optimize response time."*

**The gap:** Paper 01 achieves strong technical results — stable IRT calibration, Bloom-level alignment, difficulty misclassification rate of only 6.7% — but its architecture is too heavyweight for real-world LMS deployment. No paper in the reviewed set specifies non-functional requirements such as maximum response time, deployment infrastructure constraints, or acceptable computational overhead for a RAG-LMS in institutions with limited infrastructure such as Vietnamese universities.

---

## Gap 7: No Paper Combines All Three Evaluation Dimensions — Technical, Pedagogical, and User Acceptance — in a Single Framework

**Derived from:** Paper 02, Paper 03, Paper 05 (from matrix), Paper 07

Looking across all seven papers:
- **Paper 02** evaluates using NLP metrics (BLEU, ROUGE, BERTScore) and a 5-criterion pedagogical Likert scale — but does not measure user acceptance.
- **Paper 03** measures retrieval Precision@5 and includes a small informal pilot — but its Limitations section explicitly states it *"lacks automated RAG evaluation (like Ragas)"*, and usability was assessed only through informal qualitative feedback.
- **Paper 05 (from matrix)** uses a 9-item expert rubric for pedagogical quality — but does not measure RAG faithfulness or user acceptance.
- **Paper 07** measures user acceptance through TAM2 survey instruments — but has no AI system to evaluate.

**The gap:** No single paper evaluates all three dimensions simultaneously: (1) RAG faithfulness — are generated questions grounded in the uploaded course materials?; (2) CLO alignment — does the question accurately target the selected CLO and Bloom level?; and (3) user acceptance — do instructors and students find the system useful and trustworthy enough to adopt? These three dimensions are all necessary for a production LMS deployment, but each paper addresses only one or two of them in isolation.

---

## Summary Table

| Gap | Related Papers | Evidence from Limitations / Possible Improvement | What Remains Missing |
|-----|---------------|--------------------------------------------------|----------------------|
| G1: No CLO traceability | P01, P02, P03 | P02 & P03: "CLO alignment" listed as Possible Improvement | CLO selection feature, CLO tagging per generated question |
| G2: Instructor review not specified as requirements | P02, P03 | P02: "does not integrate a direct review or edit interface". P03: has UI but no spec, no RAG quality alert | Functional requirements for the approve/reject/edit instructor workflow |
| G3: 35% feedback error rate, no quality gate | P04 | "35% of hints were too general, incorrect, or give away the correct answer". "Lack of RAG" | Requirements for feedback quality threshold and human-in-the-loop gate |
| G4: CLO feedback framework is manual, not automated | P06 | "requires significant effort from instructors", "evaluated in a limited number of class cohorts" | Automation of CLO mapping and feedback generation via RAG |
| G5: No AI-assisted LMS research in Vietnam context | P07 | "does not evaluate technical enhancements like AI integrations" | Non-functional requirements for AI LMS adoption in Vietnamese universities |
| G6: System too complex for lightweight LMS integration | P01 | "difficult to integrate directly into lightweight LMS platforms" | Non-functional requirements for deployment constraints and response time |
| G7: No integrated evaluation framework | P02, P03, P05, P07 | Each paper covers only 1–2 dimensions; P03 admits missing Ragas | A unified framework combining faithfulness + CLO alignment + user acceptance | 