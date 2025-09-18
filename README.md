# 🌦️ Rainfall Prediction with Machine Learning  

## 📌 Project Overview  
This project was completed as part of my Data Analytics coursework and Kaggle challenge.  
The objective was to **predict rainfall (RainTomorrow)** using a comprehensive Australian weather dataset.  

I applied **data preprocessing, feature engineering, and multiple machine learning models** to tackle the problem, ultimately ranking **36th overall on the Kaggle leaderboard** (Top 40).  

---

## ⚙️ Dataset  
- **Source**: Weather dataset (training + unknown test set)  
- **Target Variable**: `RainTomorrow` (1 = Rain, 0 = No Rain)  
- **Features**: 21 attributes, including temperature, humidity, pressure, rainfall, sunshine, and wind data  

**Preprocessing steps included:**  
- Handling missing values (median/mode replacement)  
- Label encoding categorical features  
- Feature selection (`SelectKBest` → top 20 features)  
- Outlier handling (log transformation)  
- Normalization (StandardScaler)  

---

## 🧠 Models Implemented  
The following models were built, tuned, and compared:  
- Decision Tree  
- K-Nearest Neighbors (KNN)  
- Random Forest  
- Neural Network (MLP)  
- Support Vector Machine (SVM)  

Each model was optimized using **GridSearchCV/RandomizedSearchCV** with **cross-validation** to avoid overfitting.  

---

## 📊 Results  

| Model            | Accuracy | Precision | Recall | F1   | AUC  |  
|------------------|----------|-----------|--------|------|------|  
| Decision Tree    | 0.799    | 0.55      | 0.64   | 0.59 | 0.82 |  
| KNN              | 0.760    | 0.48      | 0.71   | 0.57 | 0.80 |  
| Random Forest    | 0.811    | 0.57      | 0.71   | 0.63 | 0.86 |  
| Neural Network   | 0.801    | 0.54      | 0.73   | 0.63 | 0.86 |  
| SVM              | 0.773    | 0.50      | 0.77   | 0.61 | 0.86 |  

🏆 **Best Model**: Neural Network (balanced performance, avoided overfitting)  

---

## 🏅 Kaggle Leaderboard  
- **Final Rank:** 36th place (Top 40)  
- **Best AUC Score:** 0.79537  



