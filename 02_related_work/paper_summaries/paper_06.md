# Paper 06 Summary

## Citation

- **Title:** Using Focus to Personalise Learning and Feedback in Software Engineering Education
- **Authors:** Bansri Amish Modi, Andrew Cain, Guy Wood-Bradley, Jake Renzella
- **Year:** 2023
- **Source:** 2023 IEEE/ACM 45th International Conference on Software Engineering: Software Engineering Education and Training (ICSE-SEET), Melbourne, Australia, May 17-19, 2023, pp. 296-301
- **DOI/Link:** https://doi.org/10.1109/ICSE-SEET58685.2023.00033

## Problem

Traditional assessment approaches in higher education often result in feedback being used primarily to justify marks awarded, which students frequently disregard once the assessment is complete. In software engineering education specifically, courses involve a wide variety of tasks and topics across multiple assessments, making it difficult for students to connect feedback from individual tasks to their overall learning trajectory. Providing timely, personalized feedback that is meaningfully tied to Course Learning Outcomes (CLOs) is challenging due to large class sizes, diverse student backgrounds, and the absence of a unified mechanism to relate feedback across different tasks and assessments.

## Research Methodology

This study uses a case study approach, deploying the Focus framework in undergraduate software engineering courses and evaluating its impact on student reflection and CLO tracking across a limited number of class cohorts. The evaluation focuses on practical usability and pedagogical effectiveness as observed by instructors and students within the framework deployment context.

## Method

The authors propose the **Focus** framework, which models learning objectives and relates feedback across different software engineering tasks. The framework works by:
1. **CLO-to-Task Mapping:** Instructors manually map each course task or assessment to one or more CLOs, establishing a structured relationship between assessments and learning outcomes.
2. **Focus Areas:** The framework identifies specific topic areas that require student attention based on their performance across tasks mapped to each CLO.
3. **Personalized Feedback Delivery:** Feedback from individual tasks is aggregated and presented to students in relation to their overall CLO performance, helping them see their cumulative learning trajectory rather than isolated task results.
4. **Student Reflection Support:** Students are guided to reflect on their performance across multiple tasks in relation to the same CLO, making the feedback actionable for self-directed study.

## Dataset

The framework was deployed in undergraduate software engineering courses at an Australian university. Evaluation was conducted across a limited number of class cohorts. No external or public dataset was used — the study draws on course task data, CLO mappings, and student performance records from the deployment institution.

## Evaluation

The study evaluates the Focus framework through:
1. **Instructor Observation:** Instructors assessed whether the CLO-to-task mapping process was feasible and whether the framework supported their feedback workflows.
2. **Student Reflection Efficiency:** The effectiveness of the framework was assessed by measuring whether students could more clearly connect feedback from different tasks to their overall CLO performance and identify areas for improvement.

## Results

1. **CLO Tracking:** Implementing the Focus framework helped students better connect feedback from multiple assignments to their overall learning goals, making CLO performance more transparent and actionable.
2. **Reflection Efficiency:** The framework improved the efficiency of student self-reflection, enabling students to identify specific focus areas for further study based on their cumulative CLO performance.
3. **Instructor Workload:** The initial CLO-to-task mapping process required significant effort from instructors, and the framework was evaluated in a limited number of class cohorts, raising questions about scalability.

## Limitations

- **High Manual Effort:** The framework's success depends on the initial mapping of CLOs to specific course tasks, which requires significant effort from instructors and does not scale easily to large or frequently changing curricula.
- **Limited Evaluation Scope:** The framework was evaluated in a limited number of class cohorts at a single institution, limiting the generalizability of the findings.
- **No Automation:** The paper does not use AI or RAG — all CLO mapping and feedback generation are performed manually by instructors, leaving the automation of these processes as an open problem.

## Relevance to our topic

This paper is relevant to our requirements engineering focus in two ways. First, it establishes CLO-aligned personalized feedback as a genuine, empirically grounded instructor requirement in software engineering education — directly informing RQ1 about what requirements instructors and students need from a CLO-aligned system. Second, the high manual effort required for CLO-to-task mapping and the absence of any automation directly confirms the need to formally specify functional requirements for automating CLO mapping and feedback generation in a RAG-based system, which is one of the central gaps this study addresses.

## Possible Improvement

- **AI-Assisted CLO Mapping:** Integrate an NLP or embedding-based module to automatically suggest CLO-to-task mappings based on task descriptions and syllabus content, reducing the manual effort currently required from instructors.
- **RAG-Based Feedback Generation:** Connect the Focus framework's CLO tracking logic to a RAG pipeline that retrieves relevant course materials and generates personalized, CLO-grounded feedback automatically.
