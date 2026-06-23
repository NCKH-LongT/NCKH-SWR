# Keyword Strategy for Literature Search
**Topic:** Essential Skills for Business Analysts in the Age of AI — A Systematic Literature Review
**Group:** G01 | SE2027

---

## Part 1. Keyword List by Group

### Group 1 — Role (Subject of Study)

| Priority | Keyword | Note |
|----------|---------|------|
| High | `"business analyst"` | Core role |
| High | `"requirements engineer"` | Closest academic equivalent |
| Medium | `"systems analyst"` | Broader scope, partially overlaps |
| Medium | `"product owner"` | Agile context |

---

### Group 2 — Skills and Competency

| Priority | Keyword | Note |
|----------|---------|------|
| High | `skills` | Broad, always combine with Group 1 |
| High | `competence` | Covers competence / competency / competencies |
| High | `"AI literacy"` | Emerging skill specific to AI context |
| High | `"skill requirements"` | Useful for job-market papers |
| Medium | `"soft skills"` | Communication, adaptability, critical thinking |
| Medium | `"hard skills"` | Technical, tool-specific abilities |
| Medium | `"skill gap"` | Bridges academic and industry perspectives |
| Low | `upskilling` | Workforce development angle |

---

### Group 3 — AI Context

| Priority | Keyword | Note |
|----------|---------|------|
| High | `"artificial intelligence"` | Broadest AI term |
| High | `"generative AI"` | Post-2022 context, highly relevant |
| High | `"large language model"` | Covers LLM, LLMs |
| High | `LLM` | Short form, common in recent papers |
| Medium | `"AI-augmented"` | Describes human-AI collaboration |
| Medium | `automation` | Task-level impact on BA work |
| Low | `"prompt engineering"` | Emerging skill, niche but growing |

---

### Group 4 — Requirements Engineering Activities

| Priority | Keyword | Note |
|----------|---------|------|
| High | `"requirements engineering"` | Core domain |
| High | `"requirements elicitation"` | Key BA activity |
| Medium | `"requirements specification"` | Documentation activity |
| Medium | `"stakeholder communication"` | Soft skill domain |
| Medium | `"software development"` | Broader context anchor |

---

### Group 5 — Method and Study Type

| Priority | Keyword | Note |
|----------|---------|------|
| High | `"systematic literature review"` | Target study type (SLR) |
| High | `"systematic mapping"` | Alternative SLR format |
| Medium | `"job posting*"` | For RQ2 and RQ3 empirical data |
| Medium | `"job advertisement*"` | Synonym of job posting |
| Medium | `"literature review"` | Broader than SLR, still valid |
| Low | `survey` | Industry survey papers |

---

### Group 6 — Real-World Context (Industry and Region)


| Priority | Keyword | Note |
|----------|---------|------|
| High | `"software industry"` | General industry context |
| High | `"IT industry"` | Common label in Southeast Asia papers |
| Medium | `"Southeast Asia"` | Regional scope |
| Medium | `Vietnam` | Local market validation |
| Medium | `"digital transformation"` | Enterprise adoption context |
| Low | `"outsourcing"` | Relevant to Vietnamese IT sector |

---

## Part 2. Search Strings by Research Question

### RQ1 — What skills does the literature identify as essential for BAs in AI-augmented environments?

**Goal:** Retrieve academic papers that discuss BA or RE skill taxonomies in the context of AI.

```
("business analyst" OR "requirements engineer") 
AND (skills OR competenc*) 
AND ("artificial intelligence" OR "generative AI" OR "large language model*" OR LLM)
```

**Narrow version** (for IEEE Xplore / Scopus):
```
("business analyst" OR "requirements engineer") 
AND ("AI literacy" OR "skill requirements" OR "competency framework") 
AND ("generative AI" OR LLM OR "AI-augmented")
```

---

### RQ2 — How has AI adoption changed core BA activities (elicitation, specification, communication)?

**Goal:** Find papers that analyze the impact of AI tools specifically on requirements engineering tasks.

```
("requirements engineering" OR "requirements elicitation") 
AND ("generative AI" OR "large language model*" OR LLM) 
AND ("systematic literature review" OR "systematic mapping" OR survey)
```

**Alternative string** (broader, if results are limited):
```
("requirements elicitation" OR "requirements specification" OR "stakeholder communication") 
AND ("artificial intelligence" OR automation) 
AND ("software development")
```

> **Recommended anchor paper for RQ2:**
> Cheng et al. (2026). *Generative AI for Requirements Engineering: A Systematic Literature Review.* Software: Practice and Experience. DOI: 10.1002/spe.70029
> This SLR covers 238 papers from 2019–2025 and directly addresses GenAI applications across RE activities.

---

### RQ3 — What gap exists between skills in literature and skills demanded in job postings?

**Goal:** Retrieve papers that compare academic competency models with real-world recruitment requirements.

```
("business analyst" OR "requirements engineer" OR "systems analyst") 
AND ("job posting*" OR "job advertisement*" OR "job market") 
AND (skills OR competenc*) 
AND ("artificial intelligence" OR AI)
```

---

### Industry Context Papers (2 papers — Group 6 keywords)

**Goal:** Find papers grounding the study in real industry or regional practice, particularly the Vietnamese/Southeast Asian IT market.

```
("business analyst" OR "requirements engineer") 
AND (skills OR competenc*) 
AND ("software industry" OR "IT industry") 
AND ("Southeast Asia" OR Vietnam OR "digital transformation")
```

**Alternative** (if regional papers are limited):
```
("business analyst" OR "software engineer") 
AND "job posting*" 
AND ("Vietnam" OR "Southeast Asia" OR "developing countr*")
```


