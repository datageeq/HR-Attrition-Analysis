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
   - To understand distributions and obtain summary statistics of the dataset  I use "print(data.describe())".
   ![Summary of Dataset](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/6aad0336-339a-4709-9bc3-cd212a3fa99a)
   ![Summary of Dataset_](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/261418c7-d9da-412d-ace9-b9ef9ae15b43)
   ![Summary of Dataset_ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/8278b2a7-22a3-4d39-8b18-f9d09f1a6670)
   ![Summary of Dataset_ _ _](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/b4d56b0b-a183-48df-8c48-ef421e714ebe)




4. **Modeling**: Train a logistic regression model to predict employee attrition.
5. **Evaluation**: Evaluate the model's performance using accuracy, confusion matrix, and classification report.

## Results
Key findings and visualizations are included in the `images` directory. The logistic regression model allows us to:
- Identify significant predictors of employee attrition.
- Understand the direction and magnitude of the relationship between predictors and attrition.

### Confusion Matrix
![confusion matrix](https://github.com/datageeq/HR-Attrition-Analysis/assets/115308270/9e81a223-73bb-469a-9c63-13171c1b9d38)



## Usage
1. Clone the repository.
2. Install the required dependencies.
3. Run the scripts in the `scripts` directory or open the Jupyter notebooks in the `notebooks` directory.

## License
This project is licensed under the MIT License.
