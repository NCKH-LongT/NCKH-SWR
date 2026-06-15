# Paper 02 Summary

## Citation

- **Title:** Early Prediction of Student Dropout in Higher Education using Machine Learning Models
- **Authors:** Or Goren, Liron Cohen, Amir Rubinstein
- **Year:** 2024
- **Source:** EDM 2024 Short Papers
- **DOI/Link:** https://www.educationaldatamining.org/edm2024/proceedings/2024.EDM-short-papers.32/2024.EDM-short-papers.32.pdf

## Problem

- This paper focuses on addressing the issue of student dropout in higher education, a major challenge for the educational community. Specifically, the study addresses the following aspects of the problem:
  - High dropout rates and their consequences: In some places, such as the US, up to 30% of students drop out before the start of their second year. This has negative impacts on the students themselves, educational institutions, and the economy (especially the financial burden on taxpayers).

  - The need for early identification: Many students often show signs of dropping out as early as their first year. Therefore, early identification of "at-risk" students is crucial so that universities can implement timely interventions and support measures.

  - Building profiles of students at risk: This paper seeks to assess and explore student profiles at risk of dropping out based on various factors such as academic, socioeconomic, and psychological factors.

  - Applying machine learning for prediction: The study uses machine learning models, specifically Neural Networks and XGBoost, to make early predictions based on administrative data (registration information) and learning behavior data from a Learning Management System (LMS).

## Method

- Machine Learning Models: This research focuses on two popular models to compare their effectiveness:
  - XGBoost (Extreme Gradient Boosted Trees): A decision tree-based algorithm optimized using a GridSearch mechanism to find the best hyper-parameters to optimize AUC.

  - Neural Networks (NNs): Designed with a hidden layer of 10,000 nodes, using the SGD (Stochastic Gradient Descent) optimizer and Xavier initialization technique.

- Data Processing and Analysis Techniques: To prepare the data for the models, the research team took the following key steps:
  - Data Categorization: The data was divided into three logical groups: Pre-Entry (information before enrollment), Learning-Behavior (learning behavior on the LMS), and Achievements (end-of-term learning outcomes).

  - Temporal Division: The authors divided the data into five time points during the school year (week 4, week 8, exam period A, exam period B, and end of semester 2) to assess the ability to make early predictions.

  - Course Clustering: Using the k-means algorithm (with k=4), the courses were divided into four difficulty levels: easy, medium, hard, and very hard, based on average scores and failure rates.

  - Synthesizing the "Studentship" index: This is a new point in the paper; the authors propose combining behaviors on the LMS into two indices: Social Studentship (social interactions such as forums, login) and Cognitive Studentship (cognitive interactions such as submitting assignments, assignment scores) using a weighted summation method.

- Addressing the problem of unbalanced data: Because the number of students dropping out is small, the research team used the following techniques:
  - SMOTE: Applied to the XGBoost model to generate additional artificial data for the minority class.

  - Weighted Cross Entropy Loss: Used in a neural network to adjust the error weights for the class of students dropping out.

- Evaluation Metrics: The effectiveness of the methods is assessed through:
  - AUC (Area Under the Curve): The main metric for evaluating classification ability, particularly effective with imbalanced data.

  - Dropout Recall: A metric measuring the ability to accurately identify as many students at risk of dropping out as possible, in order to minimize the omission of students needing support.

## Context

- This paper, conducted in the field of Higher Education, focuses on the application of Machine Learning (ML) for predictive analytics to identify students at risk of dropping out early. It is a case study combining administrative and behavioral data from a Learning Management System (LMS) to evaluate the effectiveness of models such as XGBoost and Neural Networks. The study, on an institutional scale, surveyed 8,267 students at a large university to compare predictive characteristics across different disciplines. The main focus was on addressing the trade-off between early prediction and model accuracy to support timely interventions and optimize student retention rates.

## Key Findings

1. Predictive effectiveness increased over time, and the "golden time" for intervention was crucial: Predictive quality was directly proportional to the amount of accumulated data, reaching an AUC accuracy of over 0.9 by the end of the second semester. The study identified the B exam period as a critical time for schools to scan lists of at-risk students, as this is when the model makes a leap in its identification capabilities. This helped balance the need for early prediction with the requirement for model reliability to provide timely support.
2. The priority order of predictive data groups: Achievements are the strongest predictor and overshadow other data groups as soon as final grades are recorded. However, at the beginning of the semester, pre-entry data plays a dominant role, and if normalized by the number of features, behavioral data on the LMS actually provides higher predictive value than pre-entry data.
3. The superiority of Neural Networks in identifying students at risk of dropping out: Neural networks (NNs) demonstrate superiority in accurately identifying the group of students truly at risk of dropping out, with a Dropout Recall index of 0.92, significantly higher than XGBoost. While XGBoost requires aggregate features such as "studentship" to improve results in the early stages, NN models have better self-learning and generalization capabilities from raw data.
4. Specific differences between disciplines: Different disciplines have different graduation patterns, indicating that a one-size-fits-all model cannot be applied to all universities. For example, Psychology relies more heavily on input data than the exact sciences and experiences a decline in predictive accuracy towards the end of the year due to the uniform difficulty of the courses in the program.

## Limitations

1. Inconsistency and low reliability of LMS data: Data from Learning Management Systems (LMS) often vary greatly depending on the specifics of the academic discipline, the teaching style of each course, and even between different semesters. This makes behavioral data less reliable than traditional administrative data sources.This volatility explains why the impact of LMS data on predictive models is often inconsistent and difficult to generalize.
2. The trade-off between timing of predictions and the effectiveness of practical interventions: Although the model's accuracy peaks at the end of the semester when all achievements are available, this is also when there is very little time left to intervene and support students. Waiting for data to accumulate to achieve better predictions directly reduces the potential of measures to prevent student dropout. This is a major challenge in balancing the requirement for algorithmic reliability with practical application value in education.
3. The method of assigning weights to the "Studentship" index is subjective: The authors acknowledge that assigning weight levels (such as +5 for a large reward or -3 for a punishment) to different types of interactions on the LMS is quite arbitrary. These weights are based on the research group's personal perception of the importance of activities rather than an objective, previously proven quantitative basis. This may affect the accuracy and broad applicability of this index to other educational institutions.
4. Unexplained Phenomena in the Specific Field of Study: The study found a surprising result: the predictive accuracy of Psychology decreased sharply towards the end of the academic year, completely contrary to the trend in the exact sciences. The authors hypothesize that the cause is due to the overly even distribution of course difficulty within the field, but also acknowledge that this needs further research to verify. This suggests that the current model has not yet fully deciphered all the specific dropout patterns.
5. Difficulties in determining dropout status and data imbalances: The school's database system lacked accurate information on whether students had dropped out, forcing the research team to define it based on not enrolling in courses for two consecutive years. Furthermore, the data was severely imbalanced due to the very small percentage of students who dropped out. Even with techniques like SMOTE and error weighting, this imbalance still significantly impacted the models' ability to accurately identify dropouts.

## Relevance to our topic

- Define the input data requirements (Data Categories):
  - Pre-Entry data: Demographic, socioeconomic, and high school achievement information to give the system an overview from the moment a student enrolls.

  - Learning-Behavior data: Interactions on the LMS (number of logins, video views, forum participation) help the system track learning progress in real time.

  - Achievements data: Scores from periodic and final exams are the strongest predictors of dropout risk.

- Personalizing alerts through the "Studentship" index: Our system aims to suggest materials and support plans "appropriate to the student's status." This paper proposes classifying student status through the "Studentship" index, which consists of two components:
  - Cognitive Studentship: Based on assignment scores and submission times. If this index is low, the system may suggest additional study materials or review exercises.

  - Social Studentship: Based on forum interactions and login activity. If this index is low, the system may send alerts to instructors to facilitate connection and encouragement for students.

- Choosing the right AI model for the "Early Warning" objective: Technical requirements for the algorithm can be derived from comparing the two models in the paper:
  - Neural Networks: Achieves a very high Recall index for the dropout group (0.92). This is extremely important for early warning systems as it helps minimize the omission of students who are truly at risk.

  - XGBoost: More effective at processing tabular data and processed features (such as studentship) at the beginning of the semester.

- Disciplinary Tailoring Requirement: The paper emphasizes that "there is no one-size-fits-all model." When designing the system, the technical requirements must allow for customization of alert logic for each different department/field of study.
