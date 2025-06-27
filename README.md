# Task 2: Exploratory Data Analysis on the Titanic Dataset  
**Prodigy Infotech Data Science Internship**

## Objective  
The primary goal of this task is to clean and explore the Titanic dataset to identify patterns, trends, and relationships between variables that may have influenced passenger survival during the Titanic disaster.

---

## Dataset Overview  
The dataset contains information about the passengers aboard the Titanic, including features such as:

- **Survived**: Survival (0 = No, 1 = Yes)  
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)  
- **Sex**: Gender of the passenger  
- **Age**: Age in years  
- **SibSp**: Number of siblings/spouses aboard  
- **Parch**: Number of parents/children aboard  
- **Fare**: Passenger fare  
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

---

## Workflow Followed

### 1. Data Loading  
The dataset (`train.csv`) was loaded using `pandas` for analysis and manipulation.

### 2. Data Cleaning  
- Missing values in the `Age` column were filled with the median age.  
- Missing values in the `Embarked` column were filled with the mode.  
- The `Cabin` column was not present in the dataset used.  
- Duplicates were removed if found.  
- Irrelevant columns (`PassengerId`, `Name`, `Ticket`) were dropped for focused analysis.  
- Categorical features like `Pclass` were converted to appropriate types where applicable.

### 3. Univariate Analysis  
- Count plots were used to examine the distribution of categorical variables such as `Survived`, `Sex`, `Pclass`, and `Embarked`.  
- Histograms were used to study the distribution of numerical features like `Age` and `Fare`.

### 4. Bivariate Analysis  
- Count plots with hue were used to explore survival rates across gender, class, and port of embarkation.  
- Boxplots helped visualize the distribution of age across survival outcomes.

### 5. Correlation Matrix  
- The dataset was numerically encoded and non-numeric columns were removed.  
- A correlation heatmap was generated to examine inter-variable relationships.

---

## Key Observations

- **Gender**: Females had a significantly higher survival rate compared to males.  
- **Passenger Class**: Survival rates were highest among 1st class passengers and decreased with lower classes.  
- **Age**: Children and younger passengers had relatively better survival chances.  
- **Fare**: Higher fare-paying passengers (likely 1st class) had better survival rates.  
- **Embarked**: Most passengers boarded from Southampton, but those who boarded from Cherbourg had better survival rates.

---

## Conclusion  
This analysis provided insights into the influence of demographics, ticket class, fare, and embarkation port on survival rates. These insights are critical for understanding the factors that affected passenger outcomes and lay the groundwork for further predictive modeling or statistical analysis.