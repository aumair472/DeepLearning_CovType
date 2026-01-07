# Deep Learning on Forest CoverType Dataset

This repository contains my Deep Learning Module Project for AtomCamp, where I applied neural networks and ensemble learning techniques to the UCI Forest CoverType dataset and analyzed their performance.

---

## 📌 Project Objective

The goal of this project was to:
- Build a baseline Multi-Layer Perceptron (MLP)
- Improve it using deeper architectures, regularization, and learning rate strategies
- Evaluate the model using accuracy, precision, recall, F1-score, and confusion matrix
- Compare neural networks with ensemble methods (Random Forest and XGBoost)
- Analyze why tree-based models outperform deep learning on structured/tabular data

---

## 📊 Dataset

- **Name:** Forest CoverType Dataset (UCI)
- **Samples:** 581,012
- **Features:** 54 numerical and binary attributes
- **Target Classes:** 7 forest cover types
- **Type:** Structured / Tabular Data

---

## ⚙️ Models Implemented

### 1️⃣ Baseline MLP
- Simple feedforward neural network
- Accuracy: **~86%**

### 2️⃣ Tuned MLP
- Added Batch Normalization, Dropout, L2 Regularization
- Learning Rate Scheduling and Early Stopping
- Accuracy: **~88%**

### 3️⃣ Random Forest
- Tuned hyperparameters
- Accuracy: **93%**
- Optimized version: **95.6%**

### 4️⃣ XGBoost (Best Model)
- Boosted decision trees with regularization and learning rate tuning
- Accuracy: **96.7%**

---

## 📈 Model Comparison

| Model | Accuracy |
|------|----------|
Baseline MLP | 86% |
Tuned MLP | 88% |
Random Forest | 93% |
Optimized Random Forest | **95.6%** |
XGBoost | **96.7%** |

---

## 🧠 Key Findings

- Neural Networks (MLP) struggle with structured/tabular data due to limited ability to model feature interactions.
- Ensemble tree-based models (Random Forest, XGBoost) significantly outperform MLP.
- XGBoost achieved the highest performance by focusing on misclassified samples through boosting.

---

## 📝 Conclusion

Despite extensive tuning, the MLP saturated near 88% accuracy, showing a performance ceiling on tabular data. In contrast, ensemble models achieved superior results, with XGBoost reaching 96.7%. This confirms that tree-based ensemble methods are better suited for structured datasets than standard neural networks.

---

## 🛠️ Tools & Libraries

- Python
- TensorFlow / Keras
- Scikit-learn
- XGBoost
- NumPy, Pandas, Matplotlib, Seaborn

---

## 📂 How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/DeepLearning_CovType.git
