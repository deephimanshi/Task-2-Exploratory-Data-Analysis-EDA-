# Task-2-Exploratory-Data-Analysis-EDA-
# Titanic Dataset - Exploratory Data Analysis (EDA)

This repository contains the Exploratory Data Analysis (EDA) of the Titanic dataset as part of my internship task.

## 📌 Objective
The goal of this project is to explore the Titanic dataset, understand its structure, handle missing values, detect outliers, analyze relationships between features, and engineer new features that could be useful for predictive modeling.

## 📂 Repository Structure
```
.
├─ data/
│  └─ titanic.csv          # raw dataset (not included here, download from Kaggle)
├─ notebooks/
│  └─ 01_EDA_titanic.ipynb # main EDA notebook
├─ images/                 # saved plots and visualizations
├─ requirements.txt        # dependencies
└─ README.md               # project documentation
```

## 🚀 Steps Performed
1. **Data loading & summary statistics**
   - Inspected shape, datatypes, and basic statistics.
2. **Missing values & duplicates**
   - Checked missingness, visualized with `missingno`.
   - Decided handling strategies (drop / impute).
3. **Univariate analysis**
   - Distribution of numeric variables (Age, Fare, etc.).
   - Countplots of categorical variables (Sex, Pclass, Embarked).
4. **Bivariate analysis**
   - Relationship between `Survived` and other features.
   - Boxplots, barplots, and survival percentages.
5. **Correlation & pairwise analysis**
   - Correlation heatmap and pairplots.
6. **Outlier detection**
   - IQR method and visual inspection using boxplots.
7. **Feature engineering**
   - FamilySize = SibSp + Parch + 1.
   - Extracted `Title` from Name and imputed Age accordingly.
8. **Multicollinearity check**
   - Used Variance Inflation Factor (VIF) to detect redundancy.

## 📊 Key Findings (examples)
- Female passengers had a much higher survival rate than males.
- 1st class passengers had better survival chances than 2nd and 3rd.
- Babies and very young children had higher survival rates.
- Fare distribution is highly skewed, requiring log transformation.
- Family size and Title are meaningful derived features.

## ⚠️ Limitations
- High proportion of missing values in `Cabin` column.
- Observational dataset, no causal inference can be made.

## 🛠️ Requirements
Install dependencies with:
```bash
pip install -r requirements.txt
```

Main libraries used:
- pandas, numpy
- matplotlib, seaborn, plotly
- scikit-learn, statsmodels
- missingno, jupyterlab

## ▶️ How to Run
1. Clone the repository:
```bash
git clone <your-repo-url>
cd <repo-name>
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Launch Jupyter Lab/Notebook:
```bash
jupyter lab
```
4. Open `notebooks/01_EDA_titanic.ipynb` and run all cells.

👤 Author: Himanshi Deep
