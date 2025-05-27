# 📊 Task 2: Exploratory Data Analysis (EDA) – Titanic Dataset

## 📌 Objective

The goal of this task is to explore the Titanic dataset using various statistical and visualization techniques to uncover patterns, relationships, trends, and potential anomalies that may impact survival prediction.

---

## 📁 Dataset

- **Name**: Titanic Dataset
- **Source**: [Kaggle – Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- **Description**: Contains passenger information used to predict survival, including features like age, sex, fare, class, etc.

---

## 🛠 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 🔍 Steps Performed

### ✅ Step-1: Import Required Dependencies

Imported essential libraries for data analysis and visualization like `pandas`, `numpy`, `seaborn`, and `matplotlib`.

---

### ✅ Step-2: Load the Dataset

- Loaded the dataset using `pandas`.
- Also classified the Dataset into: Categorical & Numerical Columns

---

### ✅ Step-3: Generate Summary Statistics

- Examined the data structure using `df.describe()` and Computed **mean**, **standard deviation**, **min**, **max**, etc; for all numeric columns.
- Also Computed **\*median** using `dataset.median()`.
- Identified distribution characteristics of `Age`, `Fare`, `SibSp`, `Parch`, `Pclass`.

---

### ✅ Step-4: Visualize Feature Distributions

#### 🔹 Step-4.1: Histograms (with Subplots)

- Plotted histograms for numeric columns using `matplotlib` subplots and `sns.histplot()`.
- Analyzed distribution shape and skewness.

#### 🔹 Step-4.2: Boxplots

- Plotted boxplots to detect and visualize outliers for `Age`, `Fare`, `SibSp`, `Parch`.

---

### ✅ Step-5: Analyze Categorical Features

- Used **countplots** to examine survival patterns across:
  - `Sex`, `Pclass`, `Embarked`
- Used **violin plots** to study `Age` distributions with respect to `Survived` and `Sex`.

---

### ✅ Step-6: Feature Correlation & Pairplot

- Created **correlation heatmap** using `sns.heatmap()` to observe relationships between numeric features.
- Used `sns.pairplot()` for selected features to visually explore feature interactions and class separation.

---

### ✅ Step-7: Feature Engineering (Optional)

- Created new features:
  - `FamilySize = SibSp + Parch + 1`
  - `IsAlone` based on `FamilySize`
  - Extracted `Title` from `Name`
- Analyzed new features against survival outcomes using barplots.

---

## 📈 Visualizations

- **Histograms** – Distribution of numeric features
- **Boxplots** – Outlier detection
- **Countplots** – Frequency analysis by categories
- **Violin/Swarmplots** – Survival patterns
- **Heatmap** – Feature correlation
- **Pairplot** – Feature interactions
- **FacetGrid** – Multiple variable exploration

---

## 📂 Repository Contents

- `Task-2_Exploratory Data Analysis (EDA).ipynb` – Jupyter notebook with full EDA
- `Titanic-Dataset.csv` – Dataset used for analysis
- `README.md` – This file

---

## 🎯 What I Learned

- How to summarize and visualize data effectively
- Importance of exploring feature distributions
- How different features impact target variable (`Survived`)
- Identification of trends and outliers that guide model building
- Data storytelling using charts and statistical summaries

---

## 🔗 Submission

- Internship: **AI/ML Internship – Elevate Labs**
- Task: **Task 2 – Exploratory Data Analysis (EDA)**
- [Submission Form Link]

---

## 📞 Contact

If you have any questions or feedback, feel free to reach out via [LinkedIn](https://linkedin.com) or email!
