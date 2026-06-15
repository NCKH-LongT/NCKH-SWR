# Paper 01 Summary

## Citation

- **Title:** Ethical Imperatives and Challenges: Review of the Use of Machine Learning for Predictive Analytics in Higher Education
- **Authors:** Emily Barnes, James Hutson, Karriem Perry
- **Year:** 2024
- **Source:** Digital Commons@Lindenwood University
- **DOI/Link:** https://digitalcommons.lindenwood.edu/cgi/viewcontent.cgi?article=1645&context=faculty-research-papers

## Problem

- This paper focuses on the ethical implications and challenges associated with the increasing integration of machine learning (ML) for predictive analytics within higher education institutions (HEIs).
  - Data Privacy and Informed Consent: Balancing the benefits of data-driven decisions with the need to protect sensitive student data and ensure students understand how their information is being used.
  - Algorithmic Bias: The risk that ML models may unintentionally amplify or perpetuate existing biases present in historical data, leading to unfair outcomes for certain student populations.
  - Transparency and Accountability: The need for clear communication regarding how algorithms operate and who is responsible for the decisions they influence.
  - Institutional Frameworks: The current lack of robust ethical guidelines and technological infrastructures necessary to navigate these challenges effectively.

## Method

- Databases and Sources: The authors used the following main databases to ensure high academic accuracy and reliability:
  - JSTOR: Access to multidisciplinary research on educational technology and ethics.

  - Scopus: Search for articles discussing the potential and limitations of machine learning.

  - Web of Science: Access to journals with high impact factors.

  - Google Scholar: Access to grey literature and the latest unindexed editions.

- Search Strategy and Selection Criteria: The authors used specific keywords such as:
  - Keywords such as "machine learning in higher education," "ethics of educational technology," "data privacy in academia," "algorithm bias in education," and "transparency and accountability in machine learning applications" were used to ensure a thorough exploration of the topic.
  - Inclusion criteria:
    - Articles published within the last 10 years to capture current trends.

    - Specifically focus on the application of machine learning in the context of higher education.

    - Ethical issues (privacy, transparency, fairness, etc.) must be discussed.

    - Sources must be peer-reviewed.

- Analysis Framework:
  - Initial coding: Annotating text segments related to machine learning and ethics.
  - Topic aggregation: Grouping code into consistent topics to represent the dataset.
  - Using a theoretical framework: Analysis is guided by ethical theories (Utilitarianism, Obligation), technology acceptance models (TAM, UTAUT), and data privacy principles (GDPR).

- Literature Review: Reference materials are evaluated based on strict criteria:
  - Quality: Peer review status, number of citations, prestige of the journal and author.

  - Bias: Consideration of author definitions, publication bias, geographic diversity, and methodology.

## Context

- This paper, conducted within the field of Higher Education, focuses on the application of Machine Learning (ML) for predictive analytics in Higher Education Institutions (HEIs) to optimize learning outcomes. This is a systematic review combining stakeholder interviews to assess the current situation and associated ethical challenges. The study is global in scope, examining key legal frameworks such as FERPA and GDPR in the context of organizations striving to improve operational efficiency. The central focus is on resolving the conflict between the need for technological innovation and the responsibility to protect student privacy and transparency.

## Key Findings

1. Optimizing educational outcomes: Machine learning is identified as a powerful transformative tool that accurately predicts academic success, identifies students at risk of dropping out early, and personalizes the learning experience to enhance operational efficiency.
2. Core ethical challenge: The use of sensitive data raises serious issues of privacy, consent, and transparency, requiring schools to balance technological innovation with protecting student autonomy.
3. Risk of algorithmic bias: ML models tend to repeat or exacerbate biases already present in historical data, causing injustice to disadvantaged student groups if not properly mitigated and controlled.
4. Need for a governance framework: Research emphasizes that establishing robust ethical frameworks, forming oversight boards, and promoting interdisciplinary collaboration (technology, law, ethics) are prerequisites for responsible ML deployment.

## Limitations

1. Heavy reliance on data quality and the flaw of incomplete data: The performance of ML models is severely impaired if the input datasets are incomplete or inconsistent. Acquiring high-quality, accurate data to feed the system remains a highly complex and critical task for institutions.
2. Algorithmic bias and the risk of exacerbating existing disparities: ML algorithms can unintentionally amplify or reinforce existing historical biases embedded within the training data. This leads to unfair predictive outcomes that could potentially worsen discrimination against certain student groups.
3. Data privacy violations and the challenges of securing informed consent: Managing sensitive student data involves substantial risks regarding privacy violations and data misuse. Striking a balance between data-driven decision-making and maintaining continuous, transparent informed consent from students is inherently difficult.
4. A shortage of longitudinal research and geographic diversity in literature: Current academic literature suffers from significant gaps, notably a lack of longitudinal studies to understand long-term impacts on students. There is also an urgent need for comparative studies across different geographic regions to rectify regional bias.

## Relevance to our topic

- Defining Non-functional Requirements: The article explicitly addresses core non-functional requirements (NFRs) that are essential for our topic and for the Software Requirements Specification (SRS), including student data confidentiality, algorithmic transparency, and fairness through bias mitigation. This research helps define precise non-functional constraints ensuring that AI system operates ethically and reliably without violating student trust.
- Defining technical constraints and data input requirements: This paper helps derive critical technical and data requirements relevant to our topic, as it emphasizes that incomplete datasets, model overfitting, and distribution shifts over time can severely degrade predictive performance. It also helps identify technical constraints in the requirements engineering process, including rigorous data preprocessing, input data completeness, and continuous system validation pipelines to maintain model integrity.
- Formulating user interface and stakeholder requirements: The article analyzes the necessity of continuous informed consent and the ability for students to challenge data-driven decisions, which directly informs functional and interface requirements. These insights help specify requirements for stakeholder-specific user interfaces, such as privacy-management modules for students and explainable AI dashboards that transparently communicate risks to teachers while preventing student stigmatization.
