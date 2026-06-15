# Paper 03 Summary

## Citation

- **Title:** A Requirements Engineering Perspective to AI-based Systems Development: A Vision Paper
- **Authors:** Xavier Franch, Andreas Jedlitschka, Silverio Martínez-Fernández
- **Year:** 2023
- **Source:** Springer
- **DOI/Link:** https://upcommons.upc.edu/server/api/core/bitstreams/590b8cce-d439-4b67-8958-d00ed7802cef/content

## Problem

- This paper focuses on addressing the challenges and gaps between traditional Requirements Engineering (RE) methods and the development of artificial intelligence (AI)-based systems. Specifically, the main issues raised include:
  - The tension between AI and RE practices: Due to the rapid pace of development, current AI system development often prioritizes creating new models and algorithms to solve complex problems, neglecting methodological aspects and established software engineering practices, including RE.
  - Complexity in system integration: Integrating AI models and algorithms into a large software system creates technical and process challenges that traditional methods cannot fully address.

  - Challenges from the data-oriented nature: Unlike conventional software, AI systems are heavily dependent on data. This creates differences in the development process (such as model training), leading to questions about who is responsible for defining requirements and what requirements should be applied to the data, algorithms, and models.

  - Lack of role definition and scope of requirements: The paper recognizes the need to clarify the roles of stakeholders (such as data engineers, AI experts) and redefine the scope of requirements (not only at the system level but also at the data and model levels) as well as non-functional requirements specific to AI (such as ethics, explainability).

## Method

- In terms of research methodology, this paper does not fall under common experimental research types such as surveys, case studies, or experiments. Instead, it is a Vision Paper. The authors' approach to constructing this paper includes the following main steps:
  - Literature Synthesis: The authors base their work on a review of current research on Requirement Engineering for AI (RE4AI) to identify existing challenges and gaps. They cite and analyze results from other studies (such as the Ishikawa and Yoshioka survey, or the system mapping study by Martínez-Fernández et al.) to support their arguments.

  - Establishing Baseline Positions: For each focus area (Roles, Requirement Scope, and Non-functional Requirements), the paper identifies a "baseline research position" based on existing theories and practices. For example, in the Non-functional Requirements section, they use the ISO/IEC 25010 standard as a basis.

  - Developing a Research Roadmap: Based on these foundational positions, the authors use expert thinking to propose a roadmap comprising potential research lines for the RE community in the future.

  - Conceptual Modeling: This paper uses diagrams and tables to concretize the vision, such as a diagram of the relationships between roles in RE4AI (Figure 1) or a hierarchical structure for quality models (Figure 3).

## Context

- This paper, conducted in the field of Software Engineering, focuses on the role of Requirements Engineering (RE) in the development of artificial intelligence (AI)-based systems to address the tension between current AI practices and traditional software engineering methodologies. It is a vision paper that synthesizes current research and expert experience to propose a research roadmap focusing on three key areas: stakeholder roles, requirements scope, and non-functional requirements. This research, conducted by scientists from Spain and Germany under European Union funding, analyzes the complexity of integrating AI components into large software systems and proposes ways to coordinate new roles such as Data Engineers and AI Specialists. The main focus is on making RE the 'cornerstone' for coordinating development activities, helping to clearly define requirements for data, models, and algorithms to ensure overall quality for the AI ​​system.

## Key Findings

1. RE as the central coordinating body: The paper asserts that Requirements Engineering (RE) must become the "cornerstone" connecting all roles, activities, and items in AI system development. Requirements engineers, with their specialized communication skills, will play a central role in bridging the knowledge gap between customers and engineering teams.

2. Redefining and supplementing roles: The authors propose breaking down the "Data Scientist" role into Data Engineer and AI Specialist to clarify responsibilities. Simultaneously, the paper adds roles such as Ethics Manager and Regulatory Specialist to meet social standards and ensure system transparency.

3. Expanding the scope of requirements: Requirements for AI systems are defined not only at the software level but also extend to the scope of data, algorithms, and hardware. This multi-stakeholder approach helps to better control factors such as the quality of input data and the operational performance of the model on the device.

4. Systematizing Non-Functional Requirements (NFRs): This paper proposes using the ISO/IEC 25010 standard to build hierarchical quality models for each distinct requirements domain. This approach helps to tightly manage critical AI characteristics such as reliability, ethics, and model explainability.

5. Integrated Research Roadmap: The paper concludes by proposing the development of conceptual models (such as ontologies) to link all aspects of roles, scope, and quality into a unified whole. This roadmap aims to provide a guiding framework to help the research and practice community professionalize the AI ​​development process.

## Limitations

1. Narrow scope of research: Due to space limitations, the paper focuses only on three main areas (roles, requirements scope, and NFRs) and does not consider other important aspects such as verification and validation in AI systems.

2. Lack of immediate empirical evidence: As this is a visionary paper, the recommendations are more geared towards future research rather than proven results. The authors acknowledge that real-world impact can only be achieved in the long term after short-term and medium-term studies are completed.

3. Risk of creating a "bottleneck": The model, which focuses on the Requirements Engineer, may create information bottlenecks if all interactions between stakeholders must go through this role.

4. Not entirely flexible (Agile): The proposed role structure still leans towards traditional approaches, lacking modern roles like Product Owner and failing to fully describe the direct, rapid interactions between engineering teams as in the Agile process.

5. Challenges in standard adoption: Proposing the use of standards like ISO/IEC 25010 may be difficult because even in traditional requirements engineering, standard adoption is not yet widespread. In the context of rapidly changing AI, promoting mainstream standards becomes even more challenging.

6. Integrity of requirements scopes: The paper acknowledges that the current list of requirements scopes (data, algorithms, hardware, etc.) may be incomplete and needs further definition to encompass all different contexts.

## Relevance to our topic

- Stakeholder Coordination (Roles) in the Educational Environment: Our system involves multiple stakeholders (students, faculty, school). This paper proposes that the Requirements Engineer (RE) should be the central coordinator to bridge the knowledge gap between the parties:
  - Domain Expert: In our project, these are educational experts or consultants who define what constitutes a student's "risk status."

  - Ethics Manager: Crucial when processing student data to ensure alerts are not biased or violate privacy rights.

  - Data & AI Engineers: Responsible for processing data from the Learning Management System (LMS) and building accurate predictive models.

- Prioritizing Specific Non-Functional Requirements (NFRs): With a system directly impacting an individual's learning path, the non-functional requirements highlighted in this paper become crucial:
  - Explainability: When the system provides warnings or "personalized support plans," instructors and students need to understand why the system is making that suggestion so they can have confidence.

  - Trust and Ethics: Ensuring the system operates fairly, without neglecting disadvantaged student groups, and that support suggestions truly benefit the student's education.

  - Quality in Use: Directly related to whether the suggested materials and support plans are truly "appropriate to the situation" and helpful to the student in practice.
