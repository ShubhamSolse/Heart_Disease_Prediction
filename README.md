## Overview

Implementation of three classification algorithms using the CRISP-DM methodology on a heart disease dataset.

This project entails applying the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework to develop and implement three different classification algorithms on a heart disease dataset. CRISP-DM, a well-known and systematic approach to data mining, provides a structured process consisting of six key phases: Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment.

By following these phases, this project ensures a comprehensive and methodical analysis. Each step, from understanding the domain-specific problem of predicting heart disease to cleaning and preparing the dataset, is meticulously carried out. The classification algorithms are then selected, trained, and tuned to maximize predictive performance. The resulting models are evaluated against key performance metrics to identify the best approach for accurately predicting heart disease outcomes.

## Business Understanding

***Note : Information collected from kaggle dataset and ChatGPT***

•The aim of this project is to develop an accurate machine learning model for early detection of cardiac diseases, improving diagnostic efficiency and supporting healthcare professionals.

•	Goals include identifying key risk factors, improving existing diagnostic methods and integrating the model into clinical practice.

•	The project focuses on real-world implementation and actionable patient insights.

## Data Understanding

***Note : Information collected from kaggle dataset and ChatGPT***

Heart disease dataset has been created with the combination of two medical tests :

1. Cholesterol level (chol)
2. Fasting blood sugar (fsb)

Dataset includes 14 features which help us detemine the patient has heart disease.

1. ***age*** : Age of the patient.

2. ***sex*** : Gender of the patient (e.g., 1 = male, 0 = female).

3. ***cp*** : chest pain type:
   1. Value 0: ***typical angina*** : **Typical angina** refers to chest pain or discomfort caused by reduced blood flow to the heart, often triggered by physical exertion.

   2. Value 1: ***atypical angina*** : **Atypical angina** involves varied chest pain, may not follow typical patterns, and can be linked to multiple underlying causes.

   3. Value 2: ***non-anginal pain*** : **Non-anginal** pain is chest pain not related to heart issues, often caused by gastrointestinal, musculoskeletal, or anxiety-related factors.

   4. Value 3: ***asymptomatic*** : **Asymptomatic** chest pain refers to chest discomfort or abnormal heart conditions without noticeable symptoms, often discovered during medical evaluations.

4. ***trestbps*** : resting blood pressure (in mm Hg on admission to the hospital)

5. ***chol*** : serum cholesterol in mg/dl

6. ***fsb*** : (fasting blood sugar > 120 mg/dl, 1 = True and 0 = False)

7. ***restecg*** : resting electrocardiographic results
   1. Value 0: normal

   2. Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV) ST-T wave abnormality on ECG suggests potential heart ischemia, electrolyte imbalances, or other heart conditions requiring further evaluation.

   3. Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria (Estes' criteria for LVH uses ECG measurements to detect left ventricular thickening, often caused by hypertension or heart disease.)

8. ***thalach*** : maximum heart rate achieved

9. ***exang*** : exercise induced angina (Exercise-induced angina is chest pain triggered by physical activity, usually caused by reduced blood flow to the heart muscle.)
   1. "1 = Yes"
   2. "0 = No"

10. ***oldpeak*** : ST depression induced by exercise relative to rest

11. ***slope*** : the slope of the peak exercise ST segment
    1. Value 0: upsloping

    2. Value 1: flat

    3. Value 2: downsloping

12. ***ca*** : number of major vessels (0-4) colored by flourosopy.

13. ***thal(Thalassemia)*** : A genetic blood disorder affecting red blood cell production, which may be associated with certain cardiovascular risks.
    1. 0 = error (in the original dataset 0 maps to NaN's).

    2. 1 = Normal thallium scan (no significant coronary artery disease).

    3. 2 = Fixed defect, indicating a scar in the heart muscle (may suggest past heart attack).

    4. 3 = Reversible defect, suggesting ischemia or reduced blood flow due to coronary artery blockage, which can be treated or improved with interventions.

14. ***target*** : (0 = no disease, 1 = disease)

15. 
