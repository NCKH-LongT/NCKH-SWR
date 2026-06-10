### 📄 PAPER 1 – Moa Chatbot: Reducing Academic Procrastination with an AI Chatbot

1. **Link:** https://doi.org/10.2196/53133

2. **Paper Title:** Development of a Mobile Intervention for Procrastination Augmented With a Semigenerative Chatbot for University Students: Pilot Randomized Controlled Trial

3. **Authors:** Seonmi Lee, Jaehyun Jeong, Myungsung Kim, Sangil Lee, Sung-Phil Kim, Dooyoung Jung

4. **Source:** JMIR mHealth and uHealth, Vol. 13, e53133, April 10, 2025. DOI: 10.2196/53133

5. **What is the real-world problem addressed in this paper?**
   Academic procrastination severely impacts university students' academic performance and mental health. Traditional time management apps (to-do lists, calendars) fail because they address only surface-level symptoms (scheduling tasks) while ignoring the underlying psychological causes such as emotional avoidance of negative feelings and lack of self-regulation.

6. **Why is this problem important?**
   Students need proactive psychological intervention, not just task reminders. Integrating a CBT-based AI chatbot enables students to develop self-awareness of their emotions, monitor procrastination triggers, and build real-time coping strategies directly on their mobile devices — without requiring direct access to a professional therapist. The pilot RCT showed statistically significant improvements in time management behavior and perceived stress in the chatbot group compared to the control group.

7. **Gap (Limitations):**
   * Small sample size (only 85 participants completed the trial), limiting statistical power.
   * Study was conducted at a single university in South Korea, limiting cultural and geographic generalizability.
   * Intervention period was only 30 days; long-term behavioral maintenance after app discontinuation was not evaluated.
   * Participants reported some unusual chatbot responses due to fine-tuning on limited data, which may affect trust and satisfaction.
   * Effectiveness is tied to the specific semigenerative architecture; how results transfer to larger generative LLMs (e.g., GPT-4, Gemini) remains untested.

---

### 📄 PAPER 2 – AI-Powered Smart Study Planner: Intelligent Personalized Scheduling

1. **Link:** https://doi.org/10.32628/IJSRSET2512320

2. **Paper Title:** AI-Powered Smart Study Planner: Enhancing Personalized Learning Through Intelligent Scheduling

3. **Authors:** Gagana Lingshetti, Sarthak Pawar, Manish Shinde, Hamja Sayyed (Department of Computer Science & Engineering, MIT ADT University, Pune, India)

4. **Source:** International Journal of Scientific Research in Science, Engineering and Technology (IJSRSET), Vol. 12, Issue 3, May 2025, pp. 148–155. DOI: 10.32628/IJSRSET2512320

5. **What is the real-world problem addressed in this paper?**
   Existing study planning tools are static and inflexible — they cannot adapt to individual learning goals, changing time availability, varying progress rates, or personal learning preferences. As a result, students quickly abandon their schedules and fail to study consistently.

6. **Why is this problem important?**
   Personalized, adaptive study planning is a key factor in improving academic outcomes. By using machine learning to automatically adjust schedules based on user behavior, quiz performance, and available time, the system optimizes study efficiency and reduces the cognitive burden of self-management — making consistent studying more sustainable for students without requiring one-on-one human tutoring.

7. **Gap (Limitations):**
   * Experimental sample was small; the system was not tested across diverse demographics, academic disciplines, or educational levels.
   * The system is heavily dependent on the accuracy and completeness of user-entered data — incorrect input leads to suboptimal schedule generation.
   * External, unpredictable disruptions (illness, family emergencies, part-time jobs) are not automatically detected or accommodated by the scheduler.
   * Long-term evaluation is absent: it remains unclear whether the system helps students build independent study habits or creates dependency on AI-generated schedules.

---

### 📄 PAPER 3 – Predicting Academic Procrastination Using Machine Learning

1. **Link:** https://doi.org/10.13021/jssr2023.3848

2. **Paper Title:** Predicting Procrastination in College Students Using Machine Learning: A Comparative Analysis of Models – A Preliminary Experiment

3. **Authors:** Arnav Mathur, Mihai Boicu

4. **Source:** Mason Publishing Journals (Journal of Student-Scientists' Research), George Mason University — ASSIP (Aspiring Scientists Summer Internship Program), 2023. DOI: 10.13021/jssr2023.3848

5. **What is the real-world problem addressed in this paper?**
   Procrastination in college students is typically detected only after it has already caused academic harm (missed deadlines, poor grades). There is a lack of early-warning systems that can predict procrastination risk from daily learning activity data before failures occur.

6. **Why is this problem important?**
   Early prediction of procrastination enables LMS systems and study apps to proactively trigger targeted interventions (such as reminders, task-splitting suggestions, or motivational nudges) before students fall into academic failure. The study demonstrates that a Random Forest model achieves R² = 0.873 when predicting a "procrastination index" derived from LMS behavioral data — a strong result suggesting practical deployability.

7. **Gap (Limitations):**
   * This is a preliminary experiment on a limited dataset; results need validation on larger, more diverse course datasets and across multiple LMS platforms.
   * The study stops at prediction — no real-time automated intervention system (e.g., smart notification trigger) was designed or tested based on the model's output.
   * Psychological and emotional variables (anxiety level, self-efficacy, intrinsic motivation) — which are root causes of procrastination — were not included as model features.
   * Results are constrained to a single course/LMS context; cross-course generalizability remains unverified.

---

### 📄 PAPER 4 – Not All Delay Is Procrastination: Behavioral Subpattern Analysis

1. **Link:** https://doi.org/10.1145/3706468.3706562

2. **Paper Title:** Not All Delay Is Procrastination: Analyzing Subpatterns of Academic Delayers in Online Learning

3. **Authors:** Jinwon Kim, Qiujie Li, Zilu Jiang, Di Xu (University of California, Irvine; paper archived in NIE Digital Repository, Singapore)

4. **Source:** Proceedings of the 15th International Learning Analytics and Knowledge Conference (LAK '25), ACM, March 2025. DOI: 10.1145/3706468.3706562

5. **What is the real-world problem addressed in this paper?**
   Learning analytics systems routinely label all late submissions as "procrastination" and apply uniform interventions (alerts, warnings) to all late submitters. This is inaccurate and counterproductive — it treats strategic learners (who submit late but perform well) the same as students who are genuinely struggling, causing notification fatigue and reducing system credibility.

6. **Why is this problem important?**
   The paper shows that late-submitting students belong to distinct behavioral subgroups with very different learning outcomes: (1) **Strategic delayers** — submit late but achieve high grades; (2) **Sporadic delayers** — occasionally late due to external factors; (3) **Dysfunctional delayers** — chronically late with poor outcomes. Correctly distinguishing these groups allows a smart reminder system to intervene only where needed, significantly improving user experience and system effectiveness.

7. **Gap (Limitations):**
   * The analysis is retrospective and static — it classifies students based on historical data, but does not provide a real-time predictive model for proactive intervention.
   * The dataset is limited to LMS clickstream and submission logs; no psychological data, off-system behavior, or qualitative context was included.
   * The paper identifies subgroups but does not propose or validate a concrete intervention design (e.g., which specific reminder strategies should be applied to each subgroup).
   * Classification results are specific to the studied online learning context; transferability to blended or fully in-person learning environments is unclear.