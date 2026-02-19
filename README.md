# 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover patterns, trends, and relationships that influenced passenger survival.

The objective of this analysis is to:
- Understand the dataset structure
- Identify missing values and outliers
- Analyze feature relationships
- Extract meaningful insights using visualization and statistics

---

## 📂 Dataset Information

The dataset consists of three files:

- 📄 `train.csv` – 891 rows, 12 columns  
- 📄 `test.csv` – 418 rows, 11 columns  
- 📄 `gender_submission.csv` – 418 rows, 2 columns  

### 🔎 Important Features

- `Survived` – Survival status (0 = No, 1 = Yes)
- `Pclass` – Passenger class (1st, 2nd, 3rd)
- `Sex` – Gender
- `Age` – Age of passenger
- `Fare` – Ticket fare
- `Embarked` – Port of embarkation
- `SibSp` – Siblings/Spouses aboard
- `Parch` – Parents/Children aboard

---

## 🛠 Tools & Technologies Used

- 🐍 Python  
- 📊 Pandas  
- 🔢 NumPy  
- 📈 Matplotlib  
- 🎨 Seaborn  
- ☁ Google Colab  

---

## 🔍 Steps Performed

### 1️⃣ Data Loading
- Imported dataset using Pandas
- Verified dataset shape and structure

### 2️⃣ Data Inspection
Used:
- `.shape()`  
- `.info()`  
- `.describe()`  
- `.value_counts()`  

✔ Identified missing values in:
- Age
- Cabin
- Embarked
- Fare (test dataset)

---

### 3️⃣ Univariate Analysis

📊 Visualizations Used:
- Histograms (Age, Fare)
- Boxplots (Age, Fare)

🔎 Findings:
- Fare distribution is highly right-skewed
- Several extreme outliers in Fare
- Most passengers were between 20–40 years old
- Age shows moderate spread

---

### 4️⃣ Bivariate Analysis

📊 Survival vs Gender
- Female passengers had significantly higher survival rate
- Majority of male passengers did not survive

📊 Survival vs Passenger Class
- 1st class had highest survival rate
- 3rd class had highest death rate
- Survival decreases as class number increases

---

### 5️⃣ Correlation Analysis

📈 Heatmap Analysis

Key Observations:
- `Pclass` has negative correlation with Survival
- `Fare` has positive correlation with Survival
- Strong negative correlation between `Pclass` and `Fare`

Interpretation:
Passengers in higher classes who paid higher fares had better survival chances.

---

### 6️⃣ Multivariate Analysis

📊 Pairplot Analysis on:
- Survived
- Pclass
- Age
- Fare

Insights:
- Clear survival pattern with passenger class
- Higher fare passengers show higher survival probability
- Age alone is not a strong predictor

---

## 📌 Key Findings

- ✔ Total passengers: 891  
- ✔ Survival rate: ~38%  
- ✔ Majority passengers were male and in 3rd class  
- ✔ Gender strongly influenced survival  
- ✔ 1st class passengers had better survival probability  
- ✔ Fare positively impacts survival  
- ✔ Passenger class negatively impacts survival  
- ✔ Age shows weak independent impact  

---

## 🎯 Conclusion

Exploratory Data Analysis revealed that **Gender and Passenger Class** were the most influential factors affecting survival.

Higher-class passengers and those who paid higher fares had better survival chances. Age showed weaker influence compared to other features.

This analysis helps in understanding patterns before building predictive machine learning models.

---


⭐ If you found this project useful, feel free to explore and learn from it!
