# Paper 05 Summary

## Citation

Title: Generative AI for Requirements Engineering: A Systematic Literature Review

Authors: Haowei Cheng; Jati H. Husen; Yijun Lu; Teeradaj Racharak; Nobukazu Yoshioka; Naoyasu Ubayashi; Hironori Washizaki

Year: 2025

Source: Software: Practice and Experience

DOI/Link: https://doi.org/10.1002/spe.70029

## Problem

The paper addresses the growing adoption of Generative AI (GenAI) in Requirements Engineering (RE) and the lack of a comprehensive understanding of how these technologies are being applied across RE activities.

The authors aim to systematically analyze existing research on GenAI for RE, identify publication and methodology trends, evaluate the maturity of current research, examine challenges and limitations, and provide future research directions for both researchers and practitioners.

## Method

The study employs a Systematic Literature Review (SLR).

The authors conducted a comprehensive search across Scopus, ACM Digital Library, IEEE Xplore, Web of Science, Google Scholar, and arXiv. After applying inclusion and exclusion criteria, removing duplicates, and performing backward and forward snowballing, a final corpus of 238 studies published between 2019 and 2025 was analyzed.

The review used a structured data extraction framework covering publication metadata, GenAI models, prompt engineering approaches, evaluation methods, outputs and resources, quality assessment, industrial adoption status, challenges, and future directions. A quality assessment process was also performed to evaluate methodological rigor across the reviewed studies.

## Context

The study was conducted in the context of software engineering, specifically Requirements Engineering.

The review examines how Generative AI technologies, particularly Large Language Models (LLMs), are being applied throughout the RE lifecycle, including requirements elicitation, analysis, specification, validation, and management.

The analyzed studies span academic research and early-stage industrial experimentation across multiple application domains, including healthcare, finance, and other software-intensive environments.

## Key Findings

The review found that research on GenAI for Requirements Engineering has grown exponentially since 2023, reflecting increasing interest in applying Large Language Models to RE activities.

Requirements analysis received the greatest research attention (30.0%), followed by elicitation (22.1%) and specification (22.1%). Requirements validation accounted for 19.0% of studies, while requirements management remained significantly underexplored at only 6.8%.

GPT-based models dominated the field. GPT-4 accounted for 36.7% of implementations and GPT-3.5 for 25.3%, while GPT-family models collectively represented 67.3% of all reviewed studies.

More than 90% of studies relied on pretrained models without domain-specific fine-tuning, indicating strong dependence on general-purpose foundation models.

Few-shot prompting was the most frequently used learning paradigm (43.6%), followed by zero-shot prompting (37.7%). Instruction-based prompting was the dominant prompt design strategy, appearing in 62.2% of studies.

The review identified three highly interconnected challenges affecting GenAI adoption in Requirements Engineering:

- Reproducibility (66.8%)
- Hallucinations (63.4%)
- Interpretability (57.1%)

The authors found strong co-occurrence relationships among these challenges, suggesting that they should be addressed collectively rather than as isolated issues.

Industrial adoption remains limited. More than 90% of studies were classified as early-stage research or prototype development, while only 1.3% reported production-level deployment.

The overall methodological quality of the literature was high, with an average quality assessment score of 3.76 out of 4.0 and 72.7% of papers achieving the maximum quality score.

## Limitations

The review focuses exclusively on Generative AI approaches and explicitly excludes BERT-based studies and other non-generative AI methods.

Most reviewed studies were conducted in academic or experimental settings, limiting the availability of evidence regarding long-term industrial deployment and real-world effectiveness.

The literature exhibits uneven coverage across Requirements Engineering phases, with requirements management receiving substantially less attention than analysis, elicitation, and specification.

The field lacks standardized evaluation benchmarks, widely available datasets, and consistent reporting practices, creating challenges for reproducibility and comparison across studies.

The heavy reliance on proprietary GPT-family models may limit the diversity of explored approaches and reduce the generalizability of findings.

## Relevance to our topic

This paper contributes primarily to RQ1 and indirectly to RQ3.

For RQ1, the paper provides strong evidence regarding the AI-related competencies increasingly relevant to Requirements Engineering activities, which are traditionally performed by Business Analysts in software development projects. The review demonstrates that professionals working with AI-assisted requirements processes must understand Large Language Models, prompt engineering techniques, requirements analysis automation, requirements elicitation support, AI-assisted specification generation, and the limitations of GenAI systems such as hallucinations, interpretability issues, and reproducibility challenges. These findings help identify AI-related knowledge and skills that may become essential for Business Analysts operating in AI-enabled software development environments.

For RQ2, the contribution is limited because the study is based on academic literature rather than job advertisements. It does not analyze labor market demand or recruitment practices for Business Analyst positions.

For RQ3, the paper provides an important academic perspective that can be compared against findings from industry job postings. The review highlights AI-related capabilities emphasized by researchers, including prompt engineering, GenAI-assisted requirements tasks, understanding of Large Language Models, and awareness of AI limitations. These competencies can be compared with the skills requested in Business Analyst job advertisements to identify potential gaps between academic recommendations and real-world employer expectations.

Overall, this paper is highly relevant as a literature source for identifying AI-related skills and knowledge areas associated with requirements engineering activities that overlap significantly with Business Analyst responsibilities in software development environments.