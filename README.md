# Detecting_Instagram_Accounts_Project

## Project Overview

This project focuses on detecting fake and real Instagram accounts efficiently and cost-effectively. Currently, approximately 28% of Instagram accounts are fake, and Instagram spends around $240,000 per year on detection and platform integrity.

Our goal is to build a machine learning model that maintains or improves detection accuracy at a fraction of the cost — reducing annual costs to $60,000, saving Instagram roughly $180,000 per year.

## Objectives

-Develop an ML model to classify Instagram accounts as fake or real.

-Optimize for accuracy, sensitivity, and specificity while reducing cost.

-Deploy the model using AWS for scalability and cost efficiency.

## Dataset

Source: Kaggle – Instagram Fake and Real Accounts Dataset

Key Features:

1. Bio Length

2. External URL presence

3. Full Name = Username

4. Full Name with Numbers

5. Followers / Followings count

6. Private account flag

7. Post count

8. Profile picture presence

9. Username with numbers

10. Word count for full name

11. Target Variable:

12. Fake Account (Binary: 1 = Fake, 0 = Real)


## Key Findings:

-Profile Picture: Strong negative correlation with fake accounts (r = -0.62).

-Username with Numbers: Moderate positive correlation with fake accounts (r = 0.57).

-Fake accounts are less likely to have profile pictures or external URLs.

-Fake accounts are more likely to have usernames resembling full names or containing numbers.

## Models Tested
Model	AUC	Sensitivity	Specificity	Notes
Logistic Regression (Baseline model)
K-Nearest Neighbors (KNN)	(Most cost-effective)
Random Forest	(Best Performing)

The Random Forest model demonstrated superior predictive performance and robustness.

##  Cost Comparison
Model	Deployment Cost	Net Cost	Annual Estimate
Current IG Model	—	—	$240,000
Proposed Model (AWS)	$60,000	~$43,000	$60,000 Total

## Instagram saves approximately $180,000 per year.

 ## Technical Workflow

Data Cleaning & Preprocessing

Handle missing values, feature encoding, and scaling.

Exploratory Data Analysis (EDA)

Correlation, feature visualization, and statistical insights.

Model Training

Train Random Forest, Logistic Regression, and KNN models.

Model Evaluation

Use metrics such as AUC, Sensitivity, Specificity, and Confusion Matrix.

Deployment

Deploy to AWS for scalable inference at $0.00003 per account.

##  Results & Conclusion

Best Model: Random Forest

Performance: AUC = 0.96

Savings: $180,000 annually

Outcome: Increases Instagram users’ trust and safety while maintaining platform integrity at lower cost.

##  Random Forest offers the best balance of accuracy and cost-efficiency.
