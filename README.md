# 🚢 Titanic Dataset – Exploratory Data Analysis (EDA)

Welcome to the **Titanic EDA project**, part of the AI & ML Internship task. This analysis dives into the legendary Titanic passenger data to uncover insights, trends, and relationships that influenced survival.

---

## 🎯 Objective

Perform Exploratory Data Analysis (EDA) on the Titanic dataset using **Python**, **Pandas**, **Seaborn**, and **Plotly** to:
- Understand data distributions
- Identify patterns and trends
- Visualize relationships between variables
- Handle missing values and outliers
- Perform basic feature engineering

---

## 🧰 Tools & Libraries Used

- `Python 3.x`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `plotly`

> 📌 All required packages are listed in [`requirements.txt`](./requirements.txt)

---

## 🗂️ Dataset Description

Dataset used: [`Titanic-Dataset.csv`](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

Key Columns:
- `Survived`: Target variable (0 = No, 1 = Yes)
- `Pclass`: Passenger class
- `Name`, `Sex`, `Age`, `Fare`, `Embarked`: Personal and travel info
- `SibSp`, `Parch`: Family aboard

---

## 🔍 Key Steps in EDA

### 1. 🧾 Data Understanding
- Overview using `.info()`, `.describe()`
- Missing value inspection

### 2. 📊 Visualizations
- Histograms for distributions
- Boxplots for outliers
- KDE plots for age survival
- Countplots for categorical insights

### 3. 🧹 Data Cleaning
- Filled missing `Age` with median
- Filled `Embarked` with mode
- Dropped sparse `Cabin` column
- Removed `Fare` outliers beyond 99th percentile

### 4. 🔎 Pattern Recognition
- Higher survival rate in females and 1st class
- Age impacts survival (children had better odds)
- Strong correlation between `Fare` and survival

### 5. 📈 Correlation Analysis
- Created correlation matrix and pairplots
- Used only numeric columns to avoid conversion errors


### 6. 🎨 Interactive Visuals (Bonus!)
- Used Plotly for interactive scatter plots of `Age` vs `Fare` colored by survival

### 7. 🧠 Feature Engineering
- Extracted `Title` from names
- Grouped rare titles for better insights


---

## 📌 Observations

- 💡 **Women and children** had better survival chances.
- 💡 **Higher-class** passengers (Pclass = 1) survived more.
- 💡 Age and Fare are useful predictors.
- 💡 Extracted titles (Mr, Miss, etc.) add valuable signal.

---

## 💾 Files Included

- `requirements.txt` – Problem Statement
- `Titanic-Dataset.csv` – Original dataset
- `Titanic_EDA.ipynb` – Full analysis notebook
- `Cleaned_Titanic_Dataset.csv` – Cleaned data after processing
- `README.md` – Project overview
- `requirements.txt` – List of dependencies

---

## ▶️ How to Run

1. Clone this repo or download the files
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
