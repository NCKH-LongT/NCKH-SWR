# Research Gap

## Group Information

- **Class:** SE2037
- **Group:** 04
- **Leader:** Nguyễn Hoàng Anh Khoa
- **Members:** Trần Anh Vinh, Phan Phúc Thịnh, Nguyễn Thị Quỳnh Trúc, Nguyễn Quang Trường

---

## How to Read This Section

Each gap below is derived by reading the **Limitations** and **Possible Improvement** sections of each paper summary, then asking:
> *"What requirements engineering problem does this paper's limitation reveal — and what does that leave unresolved for our research topic?"*

---

## Gap 1: No Paper Formally Specifies the Requirements for CLO Selection, Question Tagging, and Coverage Tracking as a Requirements Artifact

**Derived from:** Paper 01, Paper 02, Paper 03

**Paper 01 (Chen & Shiu, 2025)** integrates Bloom's Taxonomy and Item Response Theory to control cognitive difficulty, but the system was deployed for professional certification exams at Taiwan's National Institute of Environmental Research — not in a university LMS context with a syllabus-defined CLO structure. The system encodes cognitive levels as internal parameters rather than as instructor-selectable requirements tied to a specific CLO. No step in the system requires the instructor to specify a target CLO before generation, and no output is tagged with a CLO identifier for coverage tracking purposes.

**Paper 02 (Maity et al., 2025)** explicitly acknowledges in its Possible Improvement section: *"Adjust the few-shot examples in the Hybrid Model's prompt to directly reflect the cognitive levels required by the selected Course Learning Outcomes (CLOs)"* — confirming that CLO alignment was not implemented and is identified as a necessary next step. Critically, the paper does not treat CLO selection as a stakeholder requirement to be elicited and specified; it treats it as a prompt engineering problem.

**Paper 03 (Hamidi et al., 2025)** similarly states in its Possible Improvement section: *"Configure prompts and the knowledge base to allow the system to generate multi-domain questions in Vietnamese/English aligned with CLOs"* — confirming that the current system has no CLO alignment mechanism. Again, the paper frames this as a configuration problem rather than a requirements specification problem.

**The gap:** None of the seven papers specifies, as a formal requirements artifact, what an instructor needs to do to select a target CLO, how generated questions should be tagged with CLO identifiers, and how CLO coverage should be tracked across a quiz session. This is a missing functional requirements specification for CLO traceability — not merely a missing technical feature.

---

## Gap 2: The Instructor Review Workflow Exists in Practice But Its Functional Requirements Have Never Been Formally Specified

**Derived from:** Paper 02, Paper 03

**Paper 03 (Hamidi et al., 2025)** describes a human-in-the-loop instructor review step as part of its research methodology and provides a Next.js interface that allows instructors to edit and approve generated questions. However, this workflow is described as a research procedure, not as a set of formally specified functional requirements. The paper's Limitations section notes: *"The quality of the generated questions has not been verified using standard automated RAG evaluation frameworks (such as Ragas)"* — meaning no acceptance criteria were defined for what constitutes a question good enough to publish without instructor intervention. The paper also reports approximately 10% schema deviation and around 15% difficulty misalignment, but does not specify what the system should do when these conditions are detected — whether to flag the question, reject it automatically, or escalate to the instructor.

**Paper 02 (Maity et al., 2025)** states directly in its Limitations: *"The system does not integrate a direct review or edit interface for teachers before publishing questions to an LMS"* — acknowledging this as an explicit gap.

**The gap:** No paper defines the functional requirements for the instructor review workflow as a requirements artifact. What edits can an instructor make to a generated question? What happens when a question is rejected? What conditions should trigger a quality alert before instructor review? Is instructor approval a mandatory precondition for publishing questions to students? These are unspecified functional requirements, not merely unimplemented features.

---

## Gap 3: The 35% Feedback Error Rate Is Documented But No Non-Functional Requirements for Feedback Quality Thresholds Are Specified

**Derived from:** Paper 04

**Paper 04 (Reddig et al., 2025)** reports in its Results section that 35% of generated hints were rated as erroneous — either too general, factually incorrect, or directly revealing the correct answer. The paper also notes that only 35% of feedback passed the automated simulated student usefulness test. The Limitations section explicitly states: *"An error rate of 35% in generated hints or answer leaks is too high for a fully automated real-world educational deployment."* The Possible Improvement section proposes integrating RAG to retrieve course material as a grounding mechanism — but frames this entirely as a technical fix.

**The gap:** Paper 04 provides clear quantitative evidence that ungrounded LLM feedback fails at an unacceptable rate, but does not ask the prior requirements question: what quality threshold should a feedback system be required to meet before deployment? What non-functional requirements — such as a maximum error rate, a minimum faithfulness score, or a mandatory human review gate — should be specified upfront to make the system acceptable to instructors and students? Without these non-functional requirements being formally specified, any technical improvement remains unvalidatable against stakeholder expectations.

---

## Gap 4: CLO-Aligned Feedback in SE Education Is Established as a Stakeholder Need But Its Automation Requirements Have Never Been Specified

**Derived from:** Paper 06

**Paper 06 (Modi et al., 2023)** proposes the "Focus" framework to model learning objectives and relate feedback across software engineering tasks to track CLO performance. The Limitations section states: *"The framework's success depends on the initial mapping of CLOs to specific course tasks, which requires significant effort from instructors."* The paper also notes it was *"evaluated in a limited number of class cohorts."* Importantly, Paper 06 does not use AI or RAG — all CLO mapping and feedback generation are performed manually by instructors.

**The gap:** Paper 06 establishes that CLO-aligned personalized feedback is a genuine and valued instructor requirement in software engineering education, but it does not specify what functional requirements an automated system would need to satisfy to replace or support the manual process. There is no requirements artifact describing what the system must do to automate CLO mapping, what instructor inputs are needed, and what outputs must be produced for the feedback to be pedagogically equivalent to the manual process.

---

## Gap 5: LMS Adoption Factors in Vietnam Are Empirically Identified But Never Translated Into Non-Functional Requirements for AI-Assisted Systems

**Derived from:** Paper 07

**Paper 07 (Nguyen Huu Khoa, 2020)** applies the TAM2 model to identify factors influencing Vietnamese lecturers' intention to adopt LMS platforms, finding that output quality, result demonstrability, ease of use, and workload reduction are significant predictors of perceived usefulness and adoption intention. The Limitations section states directly: *"The study is limited to the survey dataset from specific Vietnamese universities and does not evaluate technical enhancements (like AI integrations) that could resolve these adoption barriers."*

**The gap:** Paper 07 empirically identifies what Vietnamese instructors value in an LMS — but stops short of translating these findings into non-functional requirements for an AI-assisted LMS. Output quality is not specified as a measurable requirement. Ease of use is not defined as a usability threshold. Workload reduction is not quantified as an acceptance criterion. These TAM2 factors are directly usable as non-functional requirements for a RAG-based LMS in the Vietnamese higher education context, but no paper has made this translation.

---

## Gap 6: Technically Advanced Systems Acknowledge Deployment Constraints But No Non-Functional Requirements for Lightweight LMS Integration Are Specified

**Derived from:** Paper 01

**Paper 01 (Chen & Shiu, 2025)** states in its Limitations section: *"Setting up knowledge graphs and the multi-agent system combined with the DDS communication protocol requires substantial computing resources and complex engineering, making it difficult to integrate directly into lightweight LMS platforms."* The Possible Improvement section proposes: *"Remove the complex DDS mechanism and replace it with a sequential RAG workflow integrated directly into the LMS API to optimize response time."*

**The gap:** Paper 01 acknowledges that deployment complexity is a real constraint but does not specify what non-functional requirements — such as maximum response time, minimum hardware requirements, or acceptable API latency — a RAG-based quiz generation system must satisfy to be deployable in institutions with limited infrastructure, such as Vietnamese universities. Without these non-functional requirements being formally specified, it is impossible to evaluate whether any proposed system is actually deployable in the target context.

---

## Gap 7: No Paper Proposes a Requirements Validation Framework That Covers Technical, Pedagogical, and Stakeholder Acceptance Dimensions Simultaneously

**Derived from:** Paper 02, Paper 03, Paper 05, Paper 07

Looking across all seven papers:
- **Paper 02 (Maity et al., 2025)** evaluates using NLP metrics and a 5-criterion pedagogical Likert scale — but does not measure whether the specified system behavior matches instructor and student expectations.
- **Paper 03 (Hamidi et al., 2025)** measures retrieval precision and includes a small informal pilot — but its Limitations section explicitly states it *"lacks automated RAG evaluation (like Ragas)"*, and stakeholder validation was limited to informal qualitative feedback without a structured requirements validation protocol.
- **Paper 05 (Scaria et al., 2024)** uses a 9-item expert rubric for pedagogical quality — but concludes that *"automated evaluation is not on par with human evaluation"*, confirming that no validated requirements-level acceptance criteria exist for Bloom-aligned question quality.
- **Paper 07 (Nguyen Huu Khoa, 2020)** measures stakeholder acceptance through TAM2 instruments — but has no AI system to validate requirements against.

**The gap:** No single paper proposes a requirements validation framework that simultaneously addresses: (1) whether generated questions are faithful to course materials — a functional correctness requirement; (2) whether questions accurately target the selected CLO and Bloom level — a functional alignment requirement; and (3) whether instructors and students find the system useful and trustworthy enough to adopt — a non-functional acceptance requirement. Each paper addresses only one or two of these dimensions in isolation, leaving no validated framework for requirements-level evaluation of a RAG-based CLO-aligned quiz generation system.

---

## Summary Table

| Gap | Related Papers | Evidence from Limitations / Possible Improvement | Requirements Engineering Dimension |
|-----|---------------|--------------------------------------------------|-------------------------------------|
| G1: CLO selection and tagging not specified as requirements | P01, P02, P03 | P02 & P03 list CLO alignment as a Possible Improvement, not a specified requirement | Missing functional requirements for CLO traceability workflow |
| G2: Instructor review workflow not formally specified | P02, P03 | P02: "no review interface"; P03: has UI but no acceptance criteria, no rejection handling spec | Missing functional requirements for instructor approval workflow |
| G3: Feedback quality thresholds not specified as non-functional requirements | P04 | "35% error rate too high for real-world deployment" but no quality threshold requirement defined | Missing non-functional requirements for feedback faithfulness and quality gates |
| G4: Automation requirements for CLO feedback not specified | P06 | "requires significant effort from instructors" — need identified but automation requirements absent | Missing functional requirements for automating CLO mapping and feedback generation |
| G5: TAM2 adoption factors not translated into non-functional requirements | P07 | "does not evaluate technical enhancements like AI integrations" | Missing non-functional requirements derived from Vietnamese instructor adoption needs |
| G6: Deployment constraints not specified as non-functional requirements | P01 | "difficult to integrate into lightweight LMS platforms" but no deployment NFRs defined | Missing non-functional requirements for response time and infrastructure constraints |
| G7: No integrated requirements validation framework | P02, P03, P05, P07 | Each paper covers only 1–2 evaluation dimensions; none covers functional + alignment + acceptance together | Missing requirements validation framework covering all three dimensions |
