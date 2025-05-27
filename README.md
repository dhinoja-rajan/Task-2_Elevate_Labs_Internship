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
- Also Computed **median** using `dataset.median(numerical_cols=True)`.
- Identified distribution characteristics of `Age`, `Fare`, `SibSp`, `Parch`, `Pclass`.

---

### ✅ Step-4: Correlate the Numeric Features

To understand how different numeric features are related to each other, I computed the **correlation matrix** using the `.corr()` function from pandas. This helped quantify the linear relationship between variables with values ranging from -1 to +1:

- **+1** indicates a strong positive correlation.
- **-1** indicates a strong negative correlation.
- **0** indicates no linear correlation.

#### 🔹 Correlation Heatmap

Using `sns.heatmap()`, I visualized the correlation matrix to easily spot strong positive or negative relationships between features.

##### Insights from the heatmap:

- `Fare` and `Pclass` are negatively correlated (higher class → lower Pclass number → higher fare).
- `SibSp` and `Parch` showed some positive correlation, suggesting passengers often traveled with both siblings/spouses and parents/children.
- `Survived` had notable correlations with `Sex`, `Pclass`, and `Fare`.

---

### ✅ Step-5: Different Plots

To explore feature distributions, relationships, and patterns in the dataset, I created multiple visualizations using Seaborn and Matplotlib. These plots help uncover trends, outliers, and categorical relationships essential for understanding the dataset before modeling.

---

#### 🔹 Step-5.1: Histplots / Histograms

- Used `sns.histplot()` and `df.hist()` to visualize the distribution of numeric features.
- Helped identify skewness, spread, and frequency of features like `Age`, `Fare`, `SibSp`, and `Parch`.
- Used `plt.subplots()` to display multiple histograms in a grid layout for compact viewing.

---

#### 🔹 Step-5.2: Boxplots

- Used `sns.boxplot()` to detect **outliers** and visualize feature spread and central tendency.
- Focused on numeric features like `Fare` and `Age`.
- Revealed extreme values in `Fare`, indicating highly variable ticket pricing across passengers.

---

#### 🔹 Step-5.3: Pairplots

- Used `sns.pairplot()` to plot pairwise relationships between multiple numeric features.
- Added `hue='Survived'` to see how survival status varied across feature combinations.
- Helped identify patterns like clustering and feature influence on survival.

---

#### 🔹 Step-5.4: Countplots

- Used `sns.countplot()` to visualize the count of passengers by categorical variables such as `Sex`, `Pclass`, and `Embarked`.
- Added `hue='Survived'` to compare survival counts within each category.
- Provided a clear visual breakdown of class distribution and survival trends across groups.

---

#### 🔹 Step-5.5: Violin Plots

- Used `sns.violinplot()` to visualize the distribution and density of a numeric variable across different categories.
- Compared `Age` and `Fare` distributions against `Survived` and `Sex`.
- Combined features of boxplots and KDE to provide more detailed distributional insights.

---

## 📈 Visualizations

- **Histograms** – Distribution of numeric features
- **Boxplots** – Outlier detection
- **Countplots** – Frequency analysis by categories
- **Violin/Swarmplots** – Survival patterns
- **Heatmap** – Feature correlation
- **Pairplot** – Feature interactions

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

If you have any questions or feedback, feel free to reach out via [LinkedIn](https://linkedin.com/dhinoja-rajan) or [Email](mailto:rajandhinoja03@gmail.com)!
