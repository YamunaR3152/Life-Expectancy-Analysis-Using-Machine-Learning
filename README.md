# Life-Expectancy-Analysis-Using-Machine-Learning

Built a data-driven analysis and machine learning pipeline to study the key factors influencing life expectancy across countries. The project combines data cleaning, exploratory analysis, regression, and classification techniques to derive meaningful public health and policy-related insights.

## Objective
The objective of this project is to analyze global life expectancy data and build predictive models to:
- Estimate life expectancy using socioeconomic and health-related indicators
- Classify countries into high and low life expectancy groups
- Identify the most influential factors affecting life expectancy

## Dataset Overview
- Dataset contains **2938 records** and **22 features**
- Includes demographic, economic, health, and education indicators
- Target variable: `Life expectancy`
- Data types include numerical and categorical variables
- Dataset contains missing values and outliers requiring preprocessing

## Data Cleaning & Preprocessing
- Filled missing values:
  - Numerical features → median imputation
  - Categorical features → mode imputation
- Removed duplicate records (none found)
- Converted GDP to numeric format
- Performed outlier detection using the **IQR method**
- Final dataset contains no missing values

## Exploratory Analysis
- Analyzed dataset structure, data types, and distributions
- Identified outliers across key variables such as GDP, mortality rates, and expenditure
- Examined relationships between health indicators and life expectancy

## Feature Selection
Selected predictors based on domain relevance:
- GDP
- BMI
- Schooling
- Alcohol consumption
- Adult Mortality
- Percentage expenditure
- Total health expenditure

Target variable:
- Life expectancy

## Regression Model: Life Expectancy Prediction
- Applied **Linear Regression** to predict life expectancy
- Data split: 80% training, 20% testing
- Features scaled using **StandardScaler**
- Model evaluated using:
  - R² score
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
- Model coefficients analyzed to understand feature impact

## Classification Model: High vs Low Life Expectancy
- Converted life expectancy into a binary target:
  - High (above median)
  - Low (below median)
- Used **Logistic Regression** with stratified train-test split
- Evaluated using:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix visualization

## Key Insights
- Schooling and GDP show a strong positive influence on life expectancy
- Higher adult mortality significantly reduces life expectancy
- Health expenditure and BMI contribute meaningfully to predictions
- Logistic regression effectively distinguishes high and low life expectancy groups

## Business & Policy Insights
- Investment in education and healthcare improves population longevity
- Reducing adult mortality has a direct impact on life expectancy
- Economic stability and healthcare access are critical drivers of public health
- Models can assist policymakers in prioritizing health interventions

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Skills Demonstrated
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Regression & Classification Modeling
- Feature Scaling & Selection
- Model Evaluation
- Business & Policy Analytics
