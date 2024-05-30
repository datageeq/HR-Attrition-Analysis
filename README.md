![attr3d](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6f61fa8d-027b-4a4a-bc30-ff7a12d6e55f)


## Project Overview
This project aims to analyze employee attrition using logistic regression. The goal is to identify the key factors contributing to employee attrition and provide actionable insights to the HR department to help improve employee retention.

## Objectives
- Identify key factors contributing to employee attrition.
- Develop a logistic regression model to predict attrition.
- Evaluate the model's performance and interpret its coefficients.

## Data
The data '*ibm-hr-analytics-attrition-dataset*' used for this project is sourced from Kaggle (https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset). This is a fictional data set created by IBM data scientists. It was downloaded in a CSV format. It includes the following fields: 
- Age
- Attrition
- BusinessTravel
- DailyRate
- Department
- DistanceFromHome
- Education
- EducationField
- EmployeeCount
- EmployeeNumber
- EnvironmentSatisfaction
- Gender
- HourlyRate
- JobInvolvement
- JobLevel
- JobRole
- JobSatisfaction
- MaritalStatus
- MonthlyIncome
- MonthlyRate
- NumCompaniesWorked
- Over18
- OverTime
- PercentSalaryHike
- PerformanceRating
- RelationshipSatisfaction
- StandardHours
- StockOptionLevel
- TotalWorkingYears
- TrainingTimesLastYear
- WorkLifeBalance
- YearsAtCompany
- YearsInCurrentRole
- YearsSinceLastPromotion
- YearsWithCurrManager

## Technology Stack for Data Analysis 
For this data analysis project, I employed a comprehensive technology stack to efficiently store, manipulate, analyze, and visualize the data. These include:
- **Microsoft Excel (CSV):** This spreadsheet tool was used to download and store the dataset.
- **Python:** This is the programming language used for the analysis due to its simplicity and extensive libraries.
- **Jupyter Notebook:** This is an Integrated Development Environment (IDE) used to execute codes, analyse data and visualize data.


## Methodology
1. Data Processing
2. Exploratory Data Analysis (EDA)
3. Data Preparation
4. Modeling
5. Evaluation
6. Results
7. Interpretation


**Data Processing**
- Import the required libraries
  Using the Jupyter Notebook, I imported the necessary libraries.
![libraries](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6c8aeb4d-7862-4e8c-9fd2-8fa61f92e014)


- Load the Dataset
  Uploaded the dataset
![load only](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/56b3817b-9038-4c77-8146-2da0aa6cc859)

- Initial Data Inspection
  
  ![inspect](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/923e3cc9-6f54-4d00-8c62-bf0f2c2344d9)
  ![Summary of Dataset_](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/9098e300-fa71-4aaf-ba95-b6476189c593)
  ![Summary of Dataset_ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/3b53007d-ea0e-4aad-b489-3b020a59e278)
  ![Summary of Dataset_ _ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/bd3fb298-b84f-4ba1-8ed2-47c0e2c22343)
  ![SUmmary info](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6c64ea18-d4f1-43f9-8eaf-2e2a8af290eb)
  ![d type](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/f3523976-7eed-49cb-9120-31d7552d2bd0)




- Data Cleaning
  

- Data Quality Checks


   
**Exploratory Data Analysis (EDA)**
   - To understand distributions and obtain summary statistics of the dataset I use "print(data.describe())".
     
     ![Summary of Dataset](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6aad0336-339a-4709-9bc3-cd212a3fa99a)
     ![Summary of Dataset_](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/261418c7-d9da-412d-ace9-b9ef9ae15b43)
     ![Summary of Dataset_ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/8278b2a7-22a3-4d39-8b18-f9d09f1a6670)
     ![Summary of Dataset_ _ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/b4d56b0b-a183-48df-8c48-ef421e714ebe)


   - Visualize the distribution of attrition
     
      ![Vizualise ditribution of attrition](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/2e9f833b-7129-4a2e-a5b3-427f0dca25d2)
      ![countplot_distribution of attrition](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/2d885d39-1ae2-4538-9423-18964fcc2851)


   - Visualize the distribution of numerical features

      ![viz dist num feats](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/586742c4-d207-4aad-a6a4-800591045f9b)
         ![histogram distribution of numerical features](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/f7d3eba5-44f8-46e6-b94d-925fd0d85878)


   - Visualize the correlation matrix

        ![viz corr matrx](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/468aeee7-8d07-4247-b145-bd69732762c1)
        ![heatmap correlation matrix](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/86bd4fda-d7c2-4396-97fb-cc1ab4bdf6c2)

    
**3. Data Preparation**


**4. Modeling**
i. **Initialize and Train the model:** In this phase, I train a logistic regression model to predict employee attritionusing the training dataset

  ![train](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/479174c9-fa67-4497-8e1d-6f59f92d1618)

ii. **Carry out Predictions on Test Set:** Here, the trained model was used to make predictions on the test dataset.

![predictions](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/80d79d37-27ef-485d-96e6-2a18048d04de)




**5. Evaluation**
Evaluate the model's performance using accuracy, confusion matrix, and classification report.






**6. Results**
Key findings from the logistic regression model are outlined in the coefficinets below: 

![image](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/cd71f33e-d84f-4e36-b6b0-7a3f7dc93869)
![image](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/722361c6-3996-40ed-a246-81f0da7f56bd)

 ## **Interpretation:**
 **Positive coefficients** denotes a highter chances of attrition
   - **OverTime** (*1.854874*): According to the logistic regression model, this is the most significant factor for attrition which indicates that eployees who work overtime are more likely to leave the company. 
   - **YearsAtCompany** (*0.691612*): Employees who have worked for an extended number of years at the company have a higher likelihood of attrition. Possible indications for this may include burnout or lack of progression.
   - **Department** (*0.681800*): The model indictaes that certain departments have higher attrition rates. Further analysis is required to investigate which departments are driving the attrition rates and why.
   - **MaritalStatus** (*0.607765*): The positive coefficinets also indicate that marital status impacts attrition. A deeper analysis is required to uncover the statuses possibly correlating with higher attrition.
   - **YearsSinceLastPromotion** (*0.475559*): This coefficient showcases that more years since the last promotion correlates with higher attrition. This indicates a potential issue with career progression.


 **Negative cofficients** denotes a lower chance of attrition
   - **YearsInCurrentRole** (*-0.667247*): Longer tenure in the current role decreases the likelihood of attrition. Employees settled in their roles may feel more secure and satisfied.
   - **YearsWithCurrManager** (*-0.442247*): Longer relationships with the current manager reduce attrition, suggesting good managerial relationships are important for retention.
   - **JobLevel** (*-0.419056*): Higher job levels are associated with lower attrition, possibly due to higher satisfaction or better compensation.
   - **JobSatisfaction** (*-0.407041*): Higher job satisfaction reduces the likelihood of attrition, which aligns with expectations.
   - **TotalWorkingYears** (*-0.374128*): More total working years correlate with lower attrition, suggesting experienced employees are less likely to leave.


Steps for Evaluation and Further Analysis
Model Performance Metrics:
Evaluate the model using metrics such as accuracy, precision, recall, F1 score, and ROC-AUC to understand its predictive power.

Cross-Validation:
Use cross-validation to ensure the model's robustness and check if it performs consistently across different subsets of the data.

Feature Importance:
Consider the practical implications of the top features (both positive and negative) and whether they align with domain knowledge.

Investigate Departments:
If the 'Department' feature shows high positive influence on attrition, analyze specific departments to identify underlying issues.

Overtime Policy:
Since 'OverTime' has the highest positive coefficient, review overtime policies and their impact on employee well-being.

Employee Engagement:
Focus on improving job satisfaction and reducing the time since last promotion to lower attrition rates.




- Identify significant predictors of employee attrition.
- Understand the direction and magnitude of the relationship between predictors and attrition.



### Confusion Matrix
![confusion matrix](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/9e81a223-73bb-469a-9c63-13171c1b9d38)
`images`
