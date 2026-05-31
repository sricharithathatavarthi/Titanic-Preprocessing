# Titanic Dataset Preprocessing 🚢

This repository contains step-by-step preprocessing tasks performed on the Titanic dataset using **Google Colab**.  
The goal is to clean, transform, and prepare the dataset for machine learning models that predict passenger survival.

---

## 📂 Contents
- `Titanic-Dataset.csv` → Original dataset
- `Titanic-Preprocessing.ipynb` → Colab notebook with all preprocessing steps
- `README.md` → This guide

---

## 🪜 Preprocessing Steps
1. **Import & Explore**  
   - Load dataset with pandas  
   - Check null values, data types, and summary statistics  

2. **Handle Missing Values**  
   - Fill `Age` with median  
   - Fill `Embarked` with mode  
   - Drop `Cabin` (too many missing values)  

3. **Encode Categorical Features**  
   - Convert `Sex` into numeric (male=0, female=1)  
   - One-hot encode `Embarked` (S, C, Q)  

4. **Normalize Numerical Features**  
   - Standardize `Age`, `Fare`, `SibSp`, `Parch` using `StandardScaler`  

5. **Visualize & Remove Outliers**  
   - Use boxplots to detect outliers  
   - Apply IQR rule to remove extreme values in `Age` and `Fare`  

---

## ⚙️ How to Run
1. Open [Google Colab](https://colab.research.google.com/)  
2. Upload the dataset (`Titanic-Dataset.csv`)  
3. Run the notebook `Titanic-Preprocessing.ipynb` step by step  
4. The cleaned dataset will be ready for ML modeling  

---

## 🎯 Next Steps
- Split dataset into train/test sets  
- Build a simple model (Logistic Regression, Decision Tree, etc.)  
- Evaluate survival prediction accuracy  

---

## 👩‍💻 Author
Created by **Charitha** — learning ML & AI step by step 🚀
