# 🌳 Ensemble Tree Classification: Heart Disease Prediction Analysis

## 🚀 Project Overview

This repository documents the completion of Task 5: Decision Trees and Random Forests. The project focuses on building, tuning, and evaluating tree-based models using the Heart Disease Dataset. The goal is to demonstrate a strong understanding of fundamental machine learning concepts—including bias-variance trade-off, information gain, and ensemble methods—in a practical classification context.

## ✨ Key Achievements & Task Fulfillment

| Objective | Description | Status |
| :--- | :--- | :--- |
| *Decision Tree Training* | Built and analyzed an unconstrained Decision Tree to demonstrate potential overfitting. | ✅ |
| *Overfitting Mitigation* | Implemented a constrained Decision Tree, controlling complexity via max_depth. | ✅ |
| *Model Visualization* | Used Graphviz to visualize the structure and decision path of the pruned tree. | 🖼️ |
| *Random Forest Ensemble* | Trained a robust Random Forest Classifier to leverage *bagging* and reduce variance. | 🌲 |
| *Feature Importance* | Calculated and plotted the relative contribution of each clinical feature to the prediction. | 💡 |
| *Robust Evaluation* | Utilized *K-Fold Cross-Validation* to secure an unbiased performance estimate. | 📊 |

## 🛠️ Technical Stack & Tools

* *Language:* Python 🐍
* *Core Libraries:* scikit-learn, pandas, numpy, matplotlib
* *Visualization Tool:* graphviz
* *Dataset:* Heart Disease Dataset (Cleveland)

## 💡 Concepts Demonstrated (Interview Prep)

The code and analysis directly address several core machine learning principles:

1.  *Gini Impurity & Entropy:* Used as criteria for optimal node splitting.
2.  *Information Gain:* The metric used to select the best split feature.
3.  *Bagging (Bootstrap Aggregation):* The foundational technique enabling the Random Forest's strength.
4.  *Bias-Variance Trade-off:* Demonstrated by comparing the high-variance (overfit) single tree to the low-variance (generalized) Random Forest.

## 📊 Results Summary

| Model Type | Primary Issue | Test Accuracy (30% Split) | Mean CV Score (5-Fold) |
| :--- | :--- | :--- | :--- |
| *Decision Tree (Unconstrained)* | High Variance (Overfitting) | ~80.0% | N/A |
| *Decision Tree (Max Depth=4)* | Controlled Complexity | ~84.5% | N/A |
| *Random Forest (n_estimators=100)* | Low Variance | *~86.9%* | *~85.5%* |

### Top 5 Predictive Features (By Importance Score)

The Random Forest model identified the following features as most crucial for determining heart disease presence:

1.  *cp* (Chest Pain Type)
2.  *thalach* (Maximum Heart Rate Achieved)
3.  *ca* (Number of Major Vessels colored by fluoroscopy)
4.  *thal* (Thalassemia)
5.  *oldpeak* (ST depression induced by exercise relative to rest)

---

## ⚙️ How to Run the Script

1.  *Clone the Repository:*
    bash
    git clone [Your Repo Link]
    
2.  *Install Dependencies:*
    bash
    pip install pandas numpy scikit-learn matplotlib graphviz
    
3.  *Data Placement:* Ensure the heart.csv file is placed in the root directory.
4.  *Execute the Script:*
    bash
    python [Your Script Name].py
    

*Note:* If you wish to view the generated tree image, ensure you have the core graphviz system tool installed (beyond the Python wrapper).
