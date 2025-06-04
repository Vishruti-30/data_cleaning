# 🧹 Titanic Data Cleaning with Pandas

A complete data cleaning and preprocessing workflow on the Titanic dataset using Pandas, including handling missing values, encoding, outlier detection, and feature engineering.

---

## 📁 Dataset
- **Source**: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/data)
- **File Used**: `train.csv`

---

## 🎯 Project Objectives
- Clean raw data for analysis or machine learning
- Handle missing values and inconsistent data types
- Encode categorical variables
- Engineer new features for modeling
- Detect and handle outliers
- Visualize correlations between features

---

## ✅ Steps Performed

1. **Data Loading**  
   - Read the Titanic dataset using Pandas

2. **Missing Value Treatment**  
   - Age → Filled with median  
   - Embarked → Filled with mode  
   - Cabin → Dropped (excessive missing values)

3. **Duplicate & Irrelevant Columns**  
   - Removed duplicate rows  
   - Dropped `Name` and `Ticket` columns

4. **Encoding**  
   - Converted `Sex` and `Embarked` to numerical values using mapping

5. **Feature Engineering**  
   - Added `FamilySize` = `SibSp` + `Parch` + 1  
   - Added `IsAlone` = 1 if `FamilySize` == 1 else 0

6. **Outlier Detection & Removal**  
   - Detected and optionally removed extreme outliers from `Fare`

7. **Correlation Analysis**  
   - Visualized feature correlation heatmap using Seaborn

---

## 📊 Tools & Libraries Used
- Python 3  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib

---

## 🚀 Next Steps
- Apply classification models (Logistic Regression, Random Forest, etc.)
- Perform hyperparameter tuning and cross-validation
- Build a full pipeline from raw data to prediction
