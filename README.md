# 🏥 US Health Insurance Analysis

This project investigates how smoking status and geographic region influence healthcare charges using the **US Health Insurance Dataset**. It applies statistical techniques and data visualization to uncover patterns and relationships in medical costs, aiming to support informed policy-making and improve public health outcomes.

## 📌 Project Overview

This analysis answers two primary research questions:

1. **Does smoking status significantly affect medical charges?**
2. **Is there a regional disparity in medical charges across different parts of the US?**

## 📊 Dataset

- **Source**: [Kaggle - US Health Insurance Dataset](https://www.kaggle.com/datasets/teertha/ushealthinsurancedataset/data)
- **Size**: 1,338 rows × 7 columns
- **Features**:
  - `age` (int)
  - `sex` (male/female)
  - `bmi` (float)
  - `children` (int)
  - `smoker` (yes/no)
  - `region` (northeast/northwest/southeast/southwest)
  - `charges` (float)

## 🧪 Methodology

### 1. Data Cleaning & Transformation
- Encoded `smoker` as binary (1 for smoker, 0 for non-smoker)
- Converted `region` to numeric values (1–4)
- Removed outliers using IQR

### 2. Exploratory Data Analysis (EDA)
- Histograms and boxplots comparing charges by smoker status and region
- Descriptive statistics to observe charge distribution

### 3. Statistical Testing
- **Welch’s t-test**: To compare charges between smokers and non-smokers
- **ANOVA**: To test for significant differences across regions

### 4. Correlation & Regression
- **Pearson Correlation**: Evaluated strength of relationship between variables
- **Linear Regression**: Modeled impact of smoker status and region on medical charges

## 📈 Key Findings

### 💨 Smoking vs. Non-Smoking
- **Smokers** incur **significantly higher** medical charges (avg. ~$22,014) than **non-smokers** (~$8,362)
- Regression shows smokers pay **$13,652 more** on average
- Correlation coefficient: **0.60** (moderate positive)

### 🌍 Regional Differences
- **Southwest** region consistently shows **higher** charges compared to other regions
- Some regional charge differences are statistically significant (ANOVA p-value = 0.00153), though the correlation is weak (-0.091)

## 📚 Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy, Statsmodels

## ✅ Conclusion

- **Smoking status has a clear and significant impact** on healthcare charges.
- **Regional differences exist**, with the southwest region standing out, although the effect is less pronounced than smoking.
