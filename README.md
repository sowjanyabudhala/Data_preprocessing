## 🚢 Titanic Dataset – Data Preprocessing Project
This project demonstrates how to preprocess a real-world dataset — the famous Titanic dataset — using Python. The focus is on preparing the data for machine learning by handling missing values, encoding categorical variables, normalizing numerical features, and removing outliers.

## 📂 Dataset
The dataset used is the Titanic passenger data, which includes various features such as:

PassengerId, Name, Sex, Age

Pclass (ticket class), SibSp (siblings/spouses aboard), Parch (parents/children aboard)

Embarked (port of embarkation), Cabin, Survived (target)

## ✅ Steps Performed
1. Import Dataset and Explore
Loaded the CSV file using pandas.

Explored column data types, basic statistics, and null value counts using .info(), .describe(), and .isnull().sum().

2. Handle Missing Values
Filled missing values in Age column with mean.

Filled missing Embarked with the mode.

Filled missing Cabin values with "U" for "Unknown", then extracted the deck (first letter).

3. Convert Categorical to Numerical
Used Label Encoding for categorical columns: Sex, Embarked.

4. Normalize/Standardize Numerical Features
Applied StandardScaler to scale Age, SibSp, and Parch for uniform distribution.

5. Outlier Detection and Removal
Used boxplots for visualization.

Applied the IQR (Interquartile Range) method to filter out outliers from numerical features.

🧰 Libraries Used
pandas, numpy

seaborn, matplotlib

scikit-learn: StandardScaler, Label Encoding


