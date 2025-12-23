## Titanic Passenger Manifest: Data Cleaning & Feature Engineering
### Project Overview
This project focuses on the rigorous cleaning, structuring, and feature engineering of the classic Titanic passenger manifest dataset. The primary goal is to transform raw, real-world survey data into a robust, analysis-ready feature set suitable for predictive modeling, specifically for predicting passenger survival.

By addressing structural untidiness and noisy data quality issues, this project demonstrates essential data wrangling skills to create a high-quality dataset where analytical patterns (e.g., the relationship between social status, family size, and survival) are easily discernible and reliable for model training.

### Business Understanding & Goals
Data Quality (Noise): Address missing values in critical features (Age, Embarked) using statistically sound imputation methods.
Data Comparability (Noise): Extract and structure packed information (e.g., social Title from Name, Family Size from SibSp and Parch) into new, useful features.
Feature Standardization (Noise): Transform highly skewed variables like Fare to improve model performance and meet statistical assumptions.
Added Value (Meta-Perspective): Engineer new features (Is_Alone, Age_Category, Family_Size_Category) to enhance predictive power.

### Data Source
Dataset: Titanic Passenger Manifest Data
File: train.csv (obtained from a public repository: [ Github,data science dojo repository](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)

### Methodology
The project followed a structured approach including data exploration, extensive cleaning, and feature engineering:

1. Data Exploration
Initial assessment of data structure, identifying variables requiring attention.
Preliminary checks for missing values, inconsistent categories, and combined features.
2. Data Cleaning & Preprocessing
Column Renaming: Standardized column names for clarity and consistency.
3. Feature Engineering
Several new features were engineered to provide more meaningful insights and improve model performance.

4. Visualizations
Key visualizations were generated to illustrate the impact of cleaning and feature engineering:

Comparison of missing values before and after cleaning.
Demonstration of memory optimization from data type conversions.
Age distribution before and after imputation.
Fare distribution before and after log transformation.
Distribution of engineered features like Title, Age_Category, and Family_Size_Category.
Survival rates analyzed by newly engineered features.
Overall data quality improvement via a radar chart.
Key Results & Achievements
Missing Values Eliminated: 100% reduction across the dataset (from 866 to 0 remaining missing values).
Memory Optimization: Achieved significant memory footprint reduction, enhancing computational efficiency.
Redundant Columns Removed: Cabin_Info column effectively handled.
New Features Created: 7 meaningful engineered features added, increasing predictive potential.
Data Type Standardization: All categorical and numerical variables correctly typed.
Fare Distribution Skewness: Reduced from 4.79 to 0.39 through log transformation.
Complete Cases: The dataset now contains 891 complete passenger records.
Analysis-Ready Features: The final dataset comprises 18 features, fully prepared for advanced modeling.
Final Dataset Snapshot
Below is a sample of the cleaned and engineered dataset:

   Passenger_ID Survival_Status Passenger_Class  Gender  Age Title  Family_Size  Is_Alone Age_Category Family_Size_Category Embarkation_Port  Ticket_Fare  Log_Fare Fare_Category
0             1               0               3    male   22    Mr            2         0        Adult                Small                S         7.25      2.11           Low
1             2               1               1  female   38   Mrs            2         0        Adult                Small                C        71.28      4.28          High
2             3               1               3  female   26  Miss            1         1        Adult                Alone                S         7.93      2.19       Mid_Low

## Project Deliverables
A well-documented, clean, analysis-ready Pandas DataFrame with newly engineered features.
Visualizations illustrating the distribution of data before and after cleansing, demonstrating added value.
A written discussion supporting all data treatment choices.
This project serves as a comprehensive example of applying robust data wrangling techniques to prepare a real-world dataset for advanced analytical tasks.
