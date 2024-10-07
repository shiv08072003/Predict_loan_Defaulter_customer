# Predict Loan Default Customers

**Dataset** : [source](https://www.rakamin.com/virtual-internship-experience/data-scientist-home-credit-indonesia) <br>
**Notebook** : [view](https://github.com/faizns/HCI-vix-project/blob/main/HCI_VIX.ipynb)<br>
**Presentation deck** : [view](https://www.canva.com/design/DAFsyNotg5E/RKJjuTM0nGTpKF7CuaAcWg/view?utm_content=DAFsyNotg5E&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)

<br>

**Table of Contents**
- [Business Understanding](https://github.com/faizns/HCI-vix-project/blob/main/README.md#-business-understanding)
- [Workflow](https://github.com/faizns/HCI-vix-project/blob/main/README.md#-workflow)
- [Insight](https://github.com/faizns/HCI-vix-project/blob/main/README.md#-insight)
- [Modeling and Evaluation](https://github.com/faizns/HCI-vix-project/blob/main/README.md#-modeling-and-evaluation)
- [Model Simulation using Streamlit](https://github.com/faizns/HCI-vix-project/blob/main/README.md#-model-simulation-using-streamlit)
<br>


## 📂 Business Understanding
### Problem Statement
Home Credit Indonesia is a company that provides easy, fast, and affordable credit services to the public. One of the problems that occurs in this company is that there are customers who fail to pay their credit. If many customers experience this problem, it will have a significant impact on the company.

According to an article published in the Harvard Business Review, it is stated that "*Non-payment by consumers can set off a chain reaction of bad debts, lower profits, layoffs, and even bankruptcies, ultimately affecting entire industries and even economies.*"

Therefore, identifying customers who are likely to fail to pay their credit is important to do. This can be a preventive measure for the company and ensure that customers who are able to make repayments are not rejected when applying for loans.

### Goals
- Loss Reduction, reducing the impact of losses caused by "Default Customers" who have the potential to default. - Deciding whether a loan application can be accepted or rejected
  
### Objectives
- Create predictive models to predict and classify customers who have the potential to default or not
- Identify the characteristics of customers who have the potential to default


## 📂 Workflow
<p align="center">
    <kbd> <img width="1000" alt="workflow" src="https://github.com/faizns/HCI-vix-project/assets/115857221/8d64b89f-f0d0-4276-9a51-82a1adb0c9a8.jpg"> </kbd> <br>
  Figure 1 — Model Creation Workflow
</p>
<br>

## 📂 Insight
- The default rate of customer credit from the dataset reached 9%
- The characteristics of the majority of customers who tend to experience problems in credit payments are:
- Male
- Low education group, "lower secondary"
- Age range 25 - 40 years
- Length of work 1 - 5 years
- Credit type "Cash Loan"
<br>

## 📂 Modeling and Evaluation
- Split dataset with a ratio of 80% Train : 20% Test
- Overcoming unbalanced Train data using RandomUnderSampler
- Scaling data with RobustScaler
- Experiments using several Logistic Regression, Random Forest, and XGBoost algorithms
- Best fit model obtained using Logistic Regression with hyperparameter tuning, resulting in 87% accuracy and 73% AUC

<br>
<p align="center">
    <kbd> <img width="800" alt="feats" src="https://github.com/faizns/HCI-vix-project/assets/115857221/a4daeca8-49f8-4c55-8cdd-3f3ad0486f18"> </kbd> <br>
    Figure 2 — Feature Importance
</p>
<br>


## 📂 Model Simulation using Streamlit

<p align="center">
    <kbd> > <img width="1000" alt="st1" src="https://github.com/faizns/HCI-vix-project/assets/115857221/d7a67ea8-1d82-4ccc-884f-d99e57c335b8"></kbd> <br>
    Figure 3 — Screenshot Part 1
</p>

<br>
<p align="center">
    <kbd> >  <img width="1000" alt="st2" src="https://github.com/faizns/HCI-vix-project/assets/115857221/045e4d1f-2b64-4e65-9018-8b6e8142c7cb"> </kbd> <br>
    Figure 4 — Screenshot Part 2
</p>
<br>

## 📂 Recommendations
- Mempertimbangkan untuk membuat Credit Scorecard, menggunakan Information Value dan Feature Engineering menggunakan Weight of Evidence
- Melakukan analisis kredit yang lebih mendalam 
- Meningkatkan seleksi calon peminjam dengan memperketat persyaratan dan mengumpulkan informasi yang lebih lengkap tentang calon peminjam
