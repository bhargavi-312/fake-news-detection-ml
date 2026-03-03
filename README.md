# 📰 Fake News Detection

This project focuses on building machine learning models to detect **fake vs. real news articles** using NLP techniques and TF-IDF vectorization.

---

## 📚 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Key Steps](#key-steps)
- [Results](#results)
- [Conclusion](#conclusion)

---

## 📘 Project Overview

This project classifies news articles as **fake (0)** or **real (1)** using several machine learning algorithms including:

- Naive Bayes  
- Logistic Regression  
- Support Vector Machine (SVM)  
- Random Forest  
- Gradient Boosting  

TF-IDF vectorization is used to transform the text into numerical features for training.

---

## 📂 Dataset

- 📁 **fakenews.csv**  
  - `text`: News article body  
  - `label`: Binary classification (0 = fake, 1 = real)

---

## 🔑 Key Steps

### 🧹 1. Data Preprocessing

- Load dataset with `pandas`
- Remove duplicates
- Clean missing/null values

### 📊 2. Exploratory Data Analysis (EDA)

- Count plot of fake vs. real labels
- Distribution of article lengths
- WordClouds for fake and real articles

### ✨ 3. Text Vectorization

- Apply **TF-IDF** to convert text into vectors

### 🧠 4. Model Training

Trained and compared the following models:

- Naive Bayes  
- Logistic Regression  
- Support Vector Machine (SVM)  
- Random Forest  
- Gradient Boosting  

---

## 📊 Results

| Model                  | Accuracy | Precision | Recall   |
|------------------------|----------|-----------|----------|
| Naive Bayes            | 76.11%   | 74.60%    | 53.71%   |
| Logistic Regression    | 76.43%   | 74.71%    | 54.86%   |
| SVM                    | 76.32%   | 70.32%    | 62.29%   |
| ✅ Random Forest        | **77.91%** | **78.54%** | **55.43%** |
| Gradient Boosting      | 75.69%   | 75.00%    | 51.43%   |

---

## 🏁 Conclusion

- ✅ **Random Forest** achieved the highest accuracy and precision, making it the best-performing model.
- Logistic Regression and Naive Bayes also performed competitively.
- SVM showed the best balance of **precision and recall**, especially for real news detection.
