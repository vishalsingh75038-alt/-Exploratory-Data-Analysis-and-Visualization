# 🚢 Exploratory Data Analysis of Titanic Dataset

## 📌 Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** on the Titanic passenger dataset using Python. The main objective is to understand the dataset, identify important patterns and relationships, handle missing values, detect outliers, and extract meaningful insights through data visualization.

The project uses popular Python data analysis and visualization libraries including **Pandas, NumPy, Matplotlib, and Seaborn**.

---

## 🎯 Objectives

The main objectives of this project are:

* Understand the structure and characteristics of the dataset.
* Perform initial data exploration and statistical analysis.
* Identify and handle missing values.
* Analyze numerical and categorical variables.
* Create meaningful data visualizations.
* Study relationships between passenger characteristics and survival.
* Detect potential outliers and anomalies.
* Perform data transformations and aggregations.
* Extract meaningful insights from the analysis.

---

## 📊 Dataset

The project uses the **Titanic passenger dataset**, a publicly available dataset containing information about passengers who travelled on the RMS Titanic.

### Important Features

| Feature       | Description                         |
| ------------- | ----------------------------------- |
| `survived`    | Survival status (0 = No, 1 = Yes)   |
| `pclass`      | Passenger class                     |
| `sex`         | Passenger gender                    |
| `age`         | Passenger age                       |
| `sibsp`       | Number of siblings/spouses aboard   |
| `parch`       | Number of parents/children aboard   |
| `fare`        | Passenger ticket fare               |
| `embarked`    | Port of embarkation                 |
| `class`       | Passenger class category            |
| `who`         | Passenger category                  |
| `adult_male`  | Whether passenger was an adult male |
| `deck`        | Deck information                    |
| `embark_town` | Embarkation town                    |
| `alive`       | Survival represented as Yes/No      |
| `alone`       | Whether passenger travelled alone   |

---

## 🛠️ Technologies Used

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**

---

## 🔍 Exploratory Data Analysis Process

The analysis was performed through the following steps:

### 1. Data Loading

The Titanic dataset was loaded using the Seaborn library and stored in a Pandas DataFrame.

### 2. Data Understanding

The dataset was examined using:

* `head()`
* `tail()`
* `shape`
* `columns`
* `info()`
* `describe()`

This helped understand the size, structure, data types, and statistical characteristics of the dataset.

### 3. Missing Value Analysis

Missing values were identified using Pandas.

The missing values were handled using appropriate techniques:

* Median imputation for numerical `age` values.
* Mode imputation for categorical variables such as `embarked` and `embark_town`.

### 4. Duplicate Analysis

Duplicate records were checked to determine whether repeated observations were present in the dataset.

### 5. Statistical Analysis

Descriptive statistics were calculated to understand variables such as:

* Age
* Fare
* Passenger class
* Survival

---

## 📈 Data Visualizations

Several visualizations were created using Matplotlib and Seaborn.

### Visualizations included:

* Survival distribution
* Gender distribution
* Gender vs Survival
* Passenger class distribution
* Passenger class vs Survival
* Age distribution
* Fare distribution
* Age vs Survival
* Fare vs Survival
* Survival rate by gender
* Survival rate by passenger class
* Gender and class vs survival
* Correlation heatmap
* Fare outlier analysis
* Missing-value heatmap
* Survival rate by age group
* Survival rate by family size

All major charts include appropriate **titles, axis labels, and legends** wherever required.

---

## 🔄 Feature Engineering

Additional features were created to perform deeper analysis.

### Age Groups

Passengers were divided into different age categories:

* Child
* Teenager
* Young Adult
* Adult
* Senior

### Family Size

A new `family_size` feature was created using the number of siblings/spouses and parents/children travelling with each passenger.

This allowed the analysis to examine whether family size was associated with survival.

---

## 💡 Key Findings

The analysis produced several important observations:

1. A larger number of passengers did not survive compared with passengers who survived.

2. **Gender had a strong relationship with survival.** Female passengers generally had a considerably higher survival rate than male passengers.

3. **Passenger class was strongly associated with survival.** First-class passengers generally had better survival outcomes than second- and third-class passengers.

4. Passenger fares were strongly related to passenger class, with higher-class passengers generally paying higher fares.

5. The fare distribution was positively skewed because a relatively small number of passengers paid very high fares.

6. Age showed differences between survival groups, although its relationship with survival was not as strong as gender and passenger class.

7. The correlation analysis helped identify relationships among numerical variables.

8. Outlier analysis showed several unusually high fare values. These observations were retained because they may represent genuine high-fare passengers rather than data errors.

9. Feature engineering using age groups and family size provided additional perspectives for analyzing passenger survival.

---

## 📁 Project Structure

```text
Titanic-EDA/
│
├── Titanic_EDA.ipynb
│
├── README.md
│
└── report/
    └── Titanic_EDA_Report.docx
```

---

## ▶️ How to Run the Project

### Option 1 — Google Colab

1. Open Google Colab.
2. Upload `Titanic_EDA.ipynb`.
3. Run the notebook cells sequentially.
4. View the generated tables and visualizations.

### Option 2 — Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

Then open the notebook using Jupyter Notebook or JupyterLab.

---

## 📋 Project Workflow

```text
Dataset Selection
       ↓
Data Loading
       ↓
Data Understanding
       ↓
Data Cleaning
       ↓
Missing Value Analysis
       ↓
Statistical Analysis
       ↓
Univariate Analysis
       ↓
Bivariate Analysis
       ↓
Multivariate Analysis
       ↓
Correlation Analysis
       ↓
Outlier Detection
       ↓
Feature Engineering
       ↓
Key Insights
       ↓
Conclusion
```

---

## 📝 Conclusion

This project demonstrates how Exploratory Data Analysis can be used to transform raw data into meaningful insights.

By combining statistical analysis with visualization, important patterns related to passenger survival were identified. Gender and passenger class showed particularly strong associations with survival, while fare, age, and family size provided additional insights.

The project also demonstrates practical data-cleaning techniques, feature engineering, aggregation, correlation analysis, and outlier detection using Python.

Overall, this analysis provides a strong foundation for understanding the Titanic dataset before applying machine learning or predictive modeling techniques.


