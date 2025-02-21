# Toxic Comment Classification Using Machine Learning

## Project Overview
This project aims to **classify toxic comments** on online platforms using **machine learning models**. The dataset, sourced from **Wikipedia Talk pages**, categorizes comments into different levels of toxicity, including:

- **Toxic**
- **Severe Toxic**
- **Obscene**
- **Threat**
- **Insult**
- **Identity Hate**

By implementing **Natural Language Processing (NLP) techniques** and multiple **machine learning models**, the goal is to **moderate toxic comments effectively** and foster a safer online environment.

---

## Dataset
The dataset used for this project comes from the **[Kaggle Toxic Comment Classification Challenge](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)**. It consists of **159,571 user-generated comments**, each labeled for varying toxicity levels. 

### **Preprocessing Steps**
- **Tokenization**
- **Stopword Removal**
- **Lemmatization**
- **TF-IDF Vectorization**
- **GloVe Word Embeddings**

---

## Machine Learning Models
We experimented with the following **supervised learning models**:

### **1. Logistic Regression (Best Performing Model)**
✅ **Baseline model** with high accuracy and precision.  
✅ Uses **sigmoid function** to classify toxic vs. non-toxic comments.  
✅ Outperformed other models in recall and **F1-score**.  

### **2. K-Nearest Neighbors (KNN)**
✔ Uses majority voting from **K-nearest data points**.  
✔ Less effective for **imbalanced datasets**.  
✔ Performed moderately well but lacked precision.  

### **3. Linear Support Vector Classifier (Linear SVC)**
✔ Finds an **optimal hyperplane** for classification.  
✔ Used **OneVsRestClassifier** for multi-label classification.  
✔ Exhibited **high precision** but lower recall than logistic regression.  

---

## Results & Key Insights
📌 **Logistic Regression** emerged as the best-performing model, **balancing precision and recall**.  
📌 **Linear SVC** was highly **conservative**, leading to **fewer false positives** but **missing some toxic comments**.  
📌 **KNN struggled** with high-dimensional NLP data and **class imbalance**.  
📌 The **dataset was highly imbalanced**, requiring techniques like **class balancing** and **feature engineering**.  
📌 **Correlation analysis** revealed strong associations between **toxic, obscene, and insult labels**.  
