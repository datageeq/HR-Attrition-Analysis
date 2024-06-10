![a1](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/38d15c8e-4ca9-4793-a93c-e53625851b9e)
http://localhost:8888/notebooks/Untitled.ipynb



## Project Overview
This project aims to analyze employee attrition using logistic regression. The goal is to identify the key factors contributing to employee attrition and provide actionable insights to the HR department to help improve employee retention.

## Objectives
- Identify key predictors contributing to employee attrition.
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

## Tools
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


## Data Processing
1. Import the required libraries using the Jupyter Notebook, I imported the necessary libraries.
![libraries](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6c8aeb4d-7862-4e8c-9fd2-8fa61f92e014)


2. Load the Dataset
![load dataset](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/7ed811c2-0f3b-4d20-809d-13b3b85240f4)


3. Initial Data Inspection

![inspect](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/923e3cc9-6f54-4d00-8c62-bf0f2c2344d9)
  ![first rows](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/aab3c28f-27b7-471b-8f58-3a53ca7de05e)
  ![SUmmary info](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6c64ea18-d4f1-43f9-8eaf-2e2a8af290eb)

  ![d type](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/f3523976-7eed-49cb-9120-31d7552d2bd0)




4. Data Cleaning
  i. Check for Null values
   
    ![missing values](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/be78b926-eb61-4995-952b-ddd874441b3a)
   
    ![missing values JPG=](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/7ee7ee62-67b0-4bf2-b685-4b9c0ee822e1)

ii. Identify and remove duplicates
       ![remove dups](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/b8706c0c-dc29-4eee-a0ac-c0422adede3d)
      ![remove dups JPG=](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/c18316a0-d9ac-4d47-8cb7-9ddc41c00ca3)
  
iii. Check for inconsistencies
   
   ![unik](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/c5530ee0-ce17-4561-a90c-f44c1dcc3c48)
   ![unik JPG=](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/dbaf59d6-d4b7-4f6e-95b6-7a047d88ed26)


   




   
## Exploratory Data Analysis (EDA)
   - To understand distributions and obtain summary statistics of the dataset I use "print(data.describe())".
     
     ![Summary of Dataset](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6aad0336-339a-4709-9bc3-cd212a3fa99a)
     ![Summary of Dataset_](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/261418c7-d9da-412d-ace9-b9ef9ae15b43)
     ![Summary of Dataset_ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/8278b2a7-22a3-4d39-8b18-f9d09f1a6670)
     ![Summary of Dataset_ _ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/b4d56b0b-a183-48df-8c48-ef421e714ebe)


   - Visualize the distribution of attrition
     
      ![Vizualise ditribution of attrition](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/2e9f833b-7129-4a2e-a5b3-427f0dca25d2)
      ![attrition count plot](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/ae1d26a9-b799-4b56-867a-7d5ab34c30e8)



   - Visualize the distribution of numerical features

      ![viz dist num feats](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/586742c4-d207-4aad-a6a4-800591045f9b)
        ![2 Visualize the distribution of numerical features](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/a417c4d1-a2ff-443e-afa8-e01d1a1874c5)



   - Visualize the correlation matrix

        ![viz corr matrx](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/468aeee7-8d07-4247-b145-bd69732762c1)
       ![2 correlation matrix](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/27bcb1f2-54d3-42fd-a76c-ac4cb4d0026e)


    
**3. Data Preparation**
![encode](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/2bf7be61-8142-42c9-91f5-99b8d76eb841)

![scale numerical](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/29a13d36-1770-4f8b-8637-b45ae79b0430)
![scale numerical JPG=](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/ae9ed269-1915-4630-8a03-4e6ef721eac9)

![separate feats](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/2a4f5ef3-916e-49c0-abb0-939ea44686ee)
![separate feats JPG=](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/df8d23e5-f82e-4c5a-bc5b-97c7de145d04)

![split data](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/16976790-c5ea-49ca-b0e0-871f6a85ed9b)
![split data JPG=](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/7e4dab09-c760-4560-b20c-eaa9cfb88050)












**4. Modeling**

i. **Initialize and Train the model:** In this phase, I train a logistic regression model to predict employee attritionusing the training dataset

  ![train](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/479174c9-fa67-4497-8e1d-6f59f92d1618)

ii. **Carry out Predictions on Test Set:** Here, the trained model was used to make predictions on the test dataset.

![predictions](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/80d79d37-27ef-485d-96e6-2a18048d04de)




**5. Evaluation**
Evaluate the model's performance using accuracy, confusion matrix, and classification report.
![confusion matrix](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/9e81a223-73bb-469a-9c63-13171c1b9d38)





## Results
Key findings from the logistic regression model are outlined in the coefficinets below: 

![image](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/cd71f33e-d84f-4e36-b6b0-7a3f7dc93869)
![image](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/722361c6-3996-40ed-a246-81f0da7f56bd)

 ## Interpretation:
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


## Considerations for further analysis

**Overtime Policy:**
'OverTime' has the highest positive coefficient, the Human Resources department is required to review overtime policies and their impact on employee well-being.

**Investigate Departments:**
The Department feature shows positive influence on attrition, further analysis is required for specific departments to identify underlying issues.

**Employee Engagement:**
Focus on improving job satisfaction and reducing the time since last promotion to lower attrition rates.

Cross-Validation:**
Use cross-validation to ensure the model's robustness and check if it performs consistently across different subsets of the data.

Feature Importance:**
Consider the practical implications of the top features (both positive and negative) and whether they align with domain knowledge.








