![pyth4](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/8edb5d3b-152d-4976-a37c-73ef60aaba9e)


## Project Overview
This project aims to analyze employee attrition using logistic regression. The goal is to identify the key factors contributing to employee attrition and provide actionable insights to the HR department to help improve employee retention.

## Objectives
- Identify key factors contributing to employee attrition.
- Develop a logistic regression model to predict attrition.
- Evaluate the model's performance and interpret its coefficients.

## Data
The dataset includes the following fields:

![Load the dataset 1](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/ef5e4498-e74b-4ad2-a86a-fe2438ee13b6)

- Age, Attrition, BusinessTravel, DailyRate, Department, DistanceFromHome, Education, EducationField, EmployeeCount, EmployeeNumber, EnvironmentSatisfaction, Gender, HourlyRate, JobInvolvement, JobLevel, JobRole, JobSatisfaction, MaritalStatus, MonthlyIncome, MonthlyRate, NumCompaniesWorked, Over18, OverTime, PercentSalaryHike, PerformanceRating, RelationshipSatisfaction, StandardHours, StockOptionLevel, TotalWorkingYears, TrainingTimesLastYear, WorkLifeBalance, YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion, YearsWithCurrManager

## Methodology
1. **Data Preprocessing**: Handle missing values, encode categorical variables, and scale numerical features.
   
2. **Exploratory Data Analysis**
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

    
3. **Modeling**: Train a logistic regression model to predict employee attrition.
4. **Evaluation**: Evaluate the model's performance using accuracy, confusion matrix, and classification report.

      ![Evaluate the model](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/41538bab-0ca0-463b-ad1a-69a34950c9e3)
      ![accuracy confxn matrx](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/2eec9b10-2de2-4fce-bcb3-dfef802ad125)





## Results
Key findings from the logistic regression model are outlined in the coefficinets below: 

![image](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/cd71f33e-d84f-4e36-b6b0-7a3f7dc93869)
![image](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/722361c6-3996-40ed-a246-81f0da7f56bd)

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


## Usage
1. Clone the repository.
2. Install the required dependencies.
3. Run the scripts in the `scripts` directory or open the Jupyter notebooks in the `notebooks` directory.

## License
This project is licensed under the MIT License.
