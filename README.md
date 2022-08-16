# credit_risk_analysis

## Overview
### The purpose of this analysis was to use different machine learning techniques to determine the risk of credit-card holders. 

## Results
### Deliverable 1: Using Resampling Models to Predict Credit Risk

#### - Naive Random Oversampling
<img width="473" alt="Screen Shot 2022-08-16 at 4 45 19 PM" src="https://user-images.githubusercontent.com/99444856/184990853-251c79f8-2f06-491f-8368-25f71ad28724.png">
<img width="473" alt="Screen Shot 2022-08-16 at 4 45 30 PM" src="https://user-images.githubusercontent.com/99444856/184990879-a3ac580f-1acf-4bff-8c0d-153f9dd7199b.png">
<img width="811" alt="Screen Shot 2022-08-16 at 4 46 58 PM" src="https://user-images.githubusercontent.com/99444856/184991047-25c03ab0-ba6a-4849-85c0-34eac238a9b5.png">

- Balanced accuracy score: 0.6497
- Precision:
  - High Risk: 0.01
  - Low Risk: 1.00
- Recall: 0.62/0.68


#### - SMOTE Oversampling
<img width="820" alt="Screen Shot 2022-08-16 at 4 50 55 PM" src="https://user-images.githubusercontent.com/99444856/184991619-6f988930-d7c3-44e7-a3a9-4f9fe52b8458.png">
- Balanced accuracy score: 0.6443
- Precision: 
  - High Risk: 0.01
  - Low Risk: 1.00
- Recall: 0.63/0.66



#### - Undersampling
<img width="815" alt="Screen Shot 2022-08-16 at 4 51 59 PM" src="https://user-images.githubusercontent.com/99444856/184991747-53c36f4a-c969-4dce-bf0f-fb75994dd93e.png">
- Balanced accuracy score: 0.5955
- Precision: 
  - High risk: 0.01
  - Low risk: 1.00
- Recall: 0.62/0.57 



### Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
#### - Combination (Over and Under) Sampling
<img width="717" alt="Screen Shot 2022-08-16 at 4 57 40 PM" src="https://user-images.githubusercontent.com/99444856/184992451-f3db075f-eadb-47f2-8aaa-2c7ac1e48a15.png">
Balanced accuracy score: 0.6376
- Precision: 
  - High Risk: 0.01
  - Low risk: 1.00
- Recall: 0.70/0.57



### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
#### - Balanced Random Forest Classifier
<img width="717" alt="Screen Shot 2022-08-16 at 5 03 06 PM" src="https://user-images.githubusercontent.com/99444856/184993121-af491ed0-2324-4b37-b2f3-b62a3e98cff8.png">
Balanced accuracy score: 0.7877
- Precision: 
  - High Risk: 0.04
  - Low Risk: 1.00
- Recall: 0.67/0.91 



#### - Easy Ensemble AdaBoost Classifier
<img width="717" alt="Screen Shot 2022-08-16 at 5 03 59 PM" src="https://user-images.githubusercontent.com/99444856/184993231-8db9ad27-6e6d-4d69-a81e-fadf00d5d7cb.png">
- Balanced accuracy score: 0.7877
- Precision: 
  - High Risk: 0.04
  - Low Risk: 1.00
- Recall: 0.67/0.91 


## Summary
If the purpose of assessing credit risk was to reduce defaults, then we want a more precise algorithm, especially for high risk applicants. The reasmpling methods generally had lower precision and a similar level of sensitivity compared to the ensemble classifiers. Therefore, if a choice must be made, I would recommend the ensemble classifiers to perform credit risk assessments rather than resamplers. At this point hoewver, none of the models should be used because sensitivity is so high that many low-risk credit card holders would actually be flagged as high risk. Additional data preprocessing could increase precision.


