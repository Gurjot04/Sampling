# Sampling Techniques Assignment – Credit Card Fraud Dataset

## 📌 Objective
The objective of this assignment is to understand the importance of sampling
techniques in handling imbalanced datasets and to analyze how different
sampling strategies affect the performance of machine learning models.

The experiment applies five sampling techniques on five machine learning models
and compares their accuracies.

---

## 📊 Dataset
The dataset used is the **Creditcard_data.csv**, which contains a highly
imbalanced distribution of fraud vs non-fraud transactions.

---

## 🧪 Sampling Techniques Used
- **Sampling1** – Random Under Sampling  
- **Sampling2** – Random Over Sampling  
- **Sampling3** – Stratified Sampling  
- **Sampling4** – Bagging (Bootstrap Sampling)  
- **Sampling5** – Cluster Sampling  

---

## 🤖 Machine Learning Models (M1–M5)
- **M1** – Logistic Regression  
- **M2** – Decision Tree  
- **M3** – Random Forest  
- **M4** – Naive Bayes  
- **M5** – Support Vector Machine  

---

## 📈 Final Accuracy Table

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|-----------|-----------|-----------|-----------|-----------|
| M1 | 25.00 | 93.14 | 98.39 | **100.00** | 97.75 |
| M2 | 75.00 | **99.35** | 97.58 | **99.35** | 95.51 |
| M3 | 25.00 | **100.00** | 98.39 | **100.00** | 97.75 |
| M4 | 25.00 | 75.82 | **97.58** | 95.48 | 94.38 |
| M5 | 0.00 | 96.08 | 98.39 | **100.00** | 97.75 |

---

## 📝 Discussion

This assignment shows that sampling techniques have a major impact on model
performance when working with imbalanced datasets. Random Under Sampling
performed poorly because it removes a large portion of the majority class,
causing the model to lose important information. As a result, models trained
on Sampling1 showed very low accuracy (0–25%).

Random Over Sampling and Stratified Sampling performed much better because
they preserve or correctly balance the data distribution. Stratified Sampling
maintains the original class ratio and therefore gives stable performance,
especially for probabilistic models like Naive Bayes.

Bagging (Sampling4) gave the best overall results. Bagging creates multiple
bootstrapped datasets which reduce variance and improve generalization. This
is why models like Logistic Regression, Random Forest, and SVM achieved
accuracy close to 100%. Cluster Sampling (Sampling5) also gave good accuracy,
but slightly lower than Bagging because cluster boundaries do not always match
class boundaries.

Overall, Sampling4 (Bagging) is the most effective technique for this dataset,
and Random Forest is the top-performing model.

---

## ✅ Conclusion

- **Best Sampling Technique:** Sampling4 (Bagging)  
- **Best Overall Model:** Random Forest (M3)  
- **Worst Sampling Technique:** Sampling1 (Random Under Sampling)  
- **Key Insight:** Balanced data drastically improves ML performance.

---

## 📁 Repository Contents
- `sampling_assignment.ipynb` – Full code  
- `Creditcard_data.csv` – Dataset  
- `README.md` – Assignment explanation & discussion  

---


