# Paper 01 Summary

## Citation

- **Title:** Analysing generative artificial intelligence capabilities to advance customer requirement processing
- **Author(s):** Aaro Vasama
- **Year:** 2024
- **Source:** Master’s Thesis - International Design Business Management (IDBM) Master's Programme, Aalto University, in collaboration with Nokia Solutions & Networks Oy.
- **DOI/Link:** URN:NBN:fi:aalto-202408255761 / https://urn.fi/URN:NBN:fi:aalto-202408255761

## Problem

The study addresses the inefficiency, high time-consumption, and human error prone nature of manually processing and analysing massive customer requirement documents and Requests for Proposals (RFPs), which frequently exceed 100 pages. It targets the inherent ambiguity and incompleteness of natural language in software requirements engineering (RE). Additionally, it tackles corporate concerns regarding data privacy, security risks, and the high operational costs associated with sending sensitive proprietary data to public cloud-based Large Language Models (LLMs) via commercial APIs.

## Method

The researcher deployed an empirical prototyping methodology combined with a comprehensive literature review:

1. **RAG (Retrieval-Augmented Generation) Architecture:** Built a local RAG pipeline using LangChain and LlamaIndex frameworks (leveraging NVIDIA Chat with RTX) to embed extensive open technical standard databases (O-RAN Specifications) into a local Vector Database.
2. **Comparative Empirical Experimentation:** Implemented a real-world validation scenario based on an EIRENE railway voice service customer story. Through precise Prompt Engineering, the study quantitatively (using Recall) and qualitatively compared 2 local, open-source models with RAG integration (Meta Llama2 13B and Mistral 7B) against a leading proprietary commercial cloud model without RAG (OpenAI GPT-4o).
3. **Expert Evaluation:** Conducted structured surveys using a 5-point Likert scale with 9 domain experts and managers (categorized into advanced knowledge and basic knowledge groups) at Nokia to evaluate the generated specifications across three metrics: Accuracy, Usability, and Coherency.

## Context

The empirical research was embedded within the production workflows of Nokia Solutions & Networks Oy. The domain context is strictly bound to Requirements Engineering (RE) within cellular and mobile telecommunications network manufacturing, where software and hardware specifications are highly complex and must stringently comply with global international standards to ensure interoperability.

## Key Findings

1. Small-scale local open-source models (under 20 billion parameters) like Mistral 7B, when augmented with local RAG and structured Prompt Engineering, can achieve a requirement extraction performance that closely approaches that of premium cloud-based models like GPT-4o.
2. The implementation of RAG significantly mitigates hallucination issues inherent in smaller models, keeping the generated content anchored to domain-specific knowledge and providing verifiable standard references (e.g., O-RAN).
3. Combining the outputs of a local RAG model (e.g., Mistral 7B, which excels at pinpointing precise technical parameters) with GPT-4o (which excels at macro-level synthesis and structural coherence) can achieve a 100% text-coverage recall rate.
4. Junior staff (under 5 years of experience) showed a higher tendency to trust and highly rate AI-generated outputs compared to senior engineers. This highlights a powerful upskilling vector but also exposes risks if junior professionals blindly accept subtly flawed parameters.

## Limitations

1. The sample size for expert validation was small (9 experts) due to strict enterprise scheduling constraints, which limited deeper statistical significance (Mann-Whitney U tests did not achieve a p-value < 0.05).
2. The RAG pipeline operated on flat data chunks (PDF standards) without sophisticated chunking optimization or semantic connection modeling, leaving room for contextual noise (the system did not utilize a Knowledge Graph).
3. The baseline of a local model _without_ RAG was excluded from formal comparison because preliminary tests showed it completely failed to generate accurate technical compliance recommendations.

## Relevance to our topic

This paper serves as an ideal reference for **RQ1** and **RQ3**. It provides concrete academic evidence of how Generative AI and Retrieval-Augmented Generation (RAG) are transforming software requirements processing. The findings suggest that future Business Analysts may require stronger competencies in AI-assisted requirements engineering, prompt design, RAG-based knowledge management, and critical validation activities. These capabilities are increasingly important for supervising AI-generated outputs and mitigating risks associated with hallucinated or inaccurate information.
