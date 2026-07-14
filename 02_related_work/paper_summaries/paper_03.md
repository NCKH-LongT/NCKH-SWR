# Paper 03 Summary

## Citation

- **Title:** Enhancing Automated Exam Creation with Retrieval-Augmented Generation for Scalable Educational Assessment
- **Authors:** Charaf Hamidi, Mohamed Badiy, Salma Gaou, Fatima Amounas, Mourade Azrour, Hicham Tribak, Abdullah M. Alnajim, Abdulatif Alabdulatif
- **Year:** 2025
- **Source:** Journal of Advances in Information Technology (JAIT), Vol. 16, No. 10
- **DOI/Link:** 10.12720/jait.16.10.1430-1441

## Problem

The study addresses the problem of automating the creation of multiple-choice and open-ended exam questions with high contextual accuracy, meeting pedagogical needs, and reducing instructor workload. Manual exam creation is highly time-consuming. Meanwhile, pure LLM question generation without RAG is prone to hallucinations and factual inaccuracies, especially for technically strict topics like SQL syntax, and for non-English languages (in this paper, French).

## Research Methodology

This study uses a system design and evaluation approach — the authors build a full-stack RAG-based web application and evaluate it through expert validation by IT instructors and SQL certified experts, and a small classroom pilot with IT students. Performance is assessed through technical metrics (retrieval latency, Precision@5) and practical measures (instructor time saving, question quality ratings).

## Method

The researchers developed a French automated SQL exam generation system based on RAG with an architecture of 4 main components:
1. **Curated Knowledge Base:** Built from French SQL instructional PDF materials, parsed and extracted using LLaMAParse. Text was chunked using MarkdownTextSplitter, combining chunks < 300 words to avoid context fragmentation.
2. **Advanced RAG Pipeline:**
   - Vectorized text using a French-compatible embedding model: `all-MPNet-base-v2`.
   - Stored and searched using FAISS similarity search to retrieve the top $k=25$ chunks.
   - Applied noise filtering (removing TOC, ellipses, text blocks < 30 words) and re-ranked using the zero-shot classification model `facebook/bart-large-mnli` to retain the most relevant chunks.
3. **NLP-driven Question Generation:** Used LLaMA 3.2 (run locally via OLLaMA) to generate multiple-choice questions (MCQs) or open-ended questions conforming to a strict JSON Schema. The system allows selecting 3 difficulty levels: "débutant" (beginner), "intermédiaire" (intermediate), and "avancé" (advanced) aligned with Bloom's Taxonomy.
4. **Interactive UI:** A user-friendly Next.js interface for instructors to configure exams, edit/approve generated questions (Human-in-the-loop), allow students to take exams, view real-time answer verification, and view real-time grading feedback.

## Dataset

- **Document Sources:** 120 PDF French SQL textbooks and exercises crawled from open-access sources.
- **Filtering Results:** Excluded corrupted/copyright-locked files, retaining **102 high-quality PDFs** (~75MB of clean text after extraction), equivalent to approximately **2,520 chunks**.
- **Topic Distribution:** SQL Joins (30%), Transactions (25%), Sub-queries (20%), and other topics (25%).

## Evaluation

The system was evaluated comprehensively through:
1. **Technical Performance:** Measured FAISS retrieval time and search accuracy (Precision@5). Compared performance before and after integrating the Re-ranking model.
2. **Expert Validation:** IT instructors and SQL experts (including the authors with SQL certifications) audited question quality, SQL syntax correctness, and difficulty alignment.
3. **Classroom Usability:** Deployed the Next.js application to a small group of IT students studying SQL for real-world testing, and collected instructor surveys regarding time saved.

## Results

1. **Technical Performance:** Average retrieval time was extremely fast, reaching 0.6 seconds under normal load. The FAISS model achieved a Precision@5 of 85%. Adding the Re-ranking model with BART improved the quality of the top 5 selected chunks by 8% to 12%, effectively removing noise.
2. **Practical Usability:** Pilot tests showed stable system operation. Instructors reported that the system **reduced exam preparation time by 38%** by allowing edits on pre-generated questions instead of writing them from scratch. The generated French SQL questions had accurate syntax and aligned closely with the learning materials.

## Limitations

- **Language and Subject Limitations:** The system is currently only optimized to generate SQL exam questions in French.
- **Small Evaluation Scale:** The classroom pilot was limited to a small IT student cohort, and has not yet been validated across different courses and departments on a larger scale.
- **Lack of Automated Evaluation Framework:** The quality of the generated questions has not been verified using standard automated RAG evaluation frameworks (such as Ragas).

## Relevance to our topic

This paper is relevant to our requirements engineering focus in two ways. First, it describes an instructor review and approval workflow — edit, approve, reject — as a practical research procedure, but never formalizes it as a set of functional requirements. The absence of defined acceptance criteria, rejection handling, and quality alert conditions leaves a clear functional requirements gap that this study addresses. Second, the reported 10% schema deviation and 15% difficulty misalignment, with no specification of how the system should respond to these conditions, directly motivates the need for formally specified acceptance criteria as part of a requirements artifact for RAG-based quiz generation systems.

## Possible Improvement

- **Integrate Detailed Explanation Module:** Add a feature to automatically generate detailed feedback (explanations) for each question based on lecture slides positioned via RAG to support student self-study.
- **Multilingual and Multi-subject Expansion:** Configure prompts and the knowledge base to allow the system to generate multi-domain questions in Vietnamese/English aligned with CLOs.
