# Titanic Dataset - EDA Summary
- Objective:
  -  Explore the Titanic dataset to uncover patterns and insights related to passenger survival.

- Dataset Overview:
  -  Total Records: 891 passengers
  -  Key Columns: Survived, Pclass, Sex, Age, SibSp, Parch, Fare, Embarked
  -  Target Variable: Survived (0 = No, 1 = Yes)

- Data Cleaning:
  - Missing Values:
    -  Age: 177 missing → filled with median age
    -  Embarked: 2 missing → filled with mode ('S')
    -  Cabin: 687 missing → dropped column
  - New Feature:
    -  FamilySize = SibSp + Parch + 1

- Key Insights:
  - Univariate Analysis:
    -  Survival: ~38% survived, with females having a higher survival rate than males.
    -  Passenger Class: Most passengers were in 3rd class. 1st class had the best survival rate.
    -  Fare Distribution: Majority of fares were under 100, with some high-fare outliers.
    -  Age Distribution: Most passengers were between 20-40 years old, with a median age of ~28.
  - Bivariate Analysis:
    -  Survival vs. Sex: ~75% of females survived vs. ~19% of males.
    -  Survival vs. Pclass: 1st class passengers had the highest survival rate, and 3rd class had the lowest.
    -  Fare vs. Pclass: 1st class had the highest median fare.
    -  Survival vs. Family Size: Medium family sizes (2-4) had better survival chances; solo travelers and large families had lower survival rates.
    -  Age vs. Survival: Children had better survival, while elderly passengers had lower survival rates.
  - Correlation Insights:
    -  Fare ↔ Pclass: Strong negative correlation (higher class, higher fare).
    -  Weak correlations between survival and other features like Age, Fare, Pclass, and Sex.
  - Key Takeaways:
    -  Gender and Class were the strongest predictors of survival.
    -  Higher fares were generally associated with better survival chances.
    -  Family size influenced survival outcomes, with moderate family sizes faring better.
    -  Handling missing values and adding new features like FamilySize enhanced the analysis.
