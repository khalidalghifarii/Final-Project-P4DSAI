# Enhanced Credit Card Default Prediction Using SMOTE, LSTM, and Stacked Ensemble Methods

This repository contains the complete implementation and documentation of a machine learning project focused on improving credit card default prediction under class imbalance conditions. The project systematically compares traditional statistical models, modern machine learning approaches, and advanced hybrid techniques to enhance default detection performance, with a primary emphasis on recall.

The project was conducted as part of a Programming for Data Science and Artificial Intelligence coursework and follows a full research lifecycle, including proposal formulation, progress reporting, experimental validation, and final reporting.

---

## Project Overview

Credit card default prediction is a critical problem in financial risk management, where failing to identify high-risk customers can result in substantial financial losses. Real-world credit datasets are inherently imbalanced, leading many models to achieve high accuracy while exhibiting poor recall for default cases.

This project addresses these challenges by:
- Handling class imbalance using Synthetic Minority Over-sampling Technique (SMOTE),
- Modeling temporal payment behavior with Long Short-Term Memory (LSTM) networks,
- Leveraging model diversity through stacked ensemble learning.

All experiments are conducted using the UCI Credit Card Default dataset, which contains 30,000 customer records from Taiwan with demographic, billing, and payment history features.

---

## Key Contributions

- Replication and validation of six baseline models reported in prior literature.
- Quantitative analysis of class imbalance effects on credit default prediction.
- Demonstration that SMOTE improves recall by approximately 30% for tree-based models.
- Development of an LSTM-based hybrid model to capture sequential payment behavior.
- Construction of a stacked ensemble model achieving the highest recall (50.41%).
- Business-oriented evaluation emphasizing recall over accuracy and estimating financial impact.


---

## Reports

This repository includes three formal academic reports documenting the evolution of the project:

- **Project Proposal**  
  Defines the research motivation, related work, problem formulation, and intended methodology.

- **Progress Report**  
  Documents completed preprocessing, feature engineering, baseline model implementation, and preliminary results.

- **Final Report**  
  Presents full experimental results, advanced model evaluation, discussion, limitations, and conclusions in IEEE conference format.

All reports are written in English and formatted according to academic standards.

---

## Dataset

- **Name:** Default of Credit Card Clients  
- **Source:** UCI Machine Learning Repository  
- **Size:** 30,000 samples  
- **Features:** 23 original features + engineered features  
- **Class Distribution:**  
  - Non-default: 77.88%  
  - Default: 22.12%

Due to licensing, the dataset is not included in this repository. It can be downloaded from:
https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients

---

## Methodology Summary

### Baseline Models
- Linear Discriminant Analysis (LDA)
- Logistic Regression (LR)
- Support Vector Machine (SVM)
- Random Forest (RF)
- XGBoost
- Deep Neural Network (DNN)

### Advanced Approaches
- **SMOTE-enhanced XGBoost**
- **LSTM Hybrid Model**
- **Stacked Ensemble**
  - Base learners: XGBoost, Random Forest, Logistic Regression
  - Meta-learner: Logistic Regression

### Evaluation Metrics
- Accuracy
- Precision
- Recall (primary metric)
- F1-score
- G-Mean
- AUC-ROC

---

## Experimental Environment

- Python 3.12
- scikit-learn 1.3
- XGBoost 2.0
- TensorFlow 2.15
- imbalanced-learn
- Google Colab (CPU runtime)

All experiments are fully reproducible using the provided Jupyter Notebook.

---

## Results Summary

- Baseline models achieve high accuracy (~81%) but low recall (23–39%).
- SMOTE improves recall by up to 30.8% with minimal accuracy loss.
- LSTM captures temporal behavior but requires class balancing for optimal recall.
- The stacked ensemble achieves the best overall recall (50.41%), detecting 154 additional default cases per 6,000 customers compared to the baseline DNN.

---

## Authors

- **Muhammad Khalid Al Ghifari**  
  Department of Informatics  
  Syiah Kuala University, Banda Aceh, Indonesia  
  Email: khalid.22@mhs.usk.ac.id  

- **Andrie Fadhlullah Wahby**  
  Department of Informatics  
  Syiah Kuala University, Banda Aceh, Indonesia  
  Email: andri33@mhs.usk.ac.id  

---

## License

This project is intended for academic and educational purposes only.  
Please cite appropriately if you reuse any part of this work.

---

## Acknowledgment

The authors acknowledge Syiah Kuala University for providing computational resources and academic support throughout this project.
