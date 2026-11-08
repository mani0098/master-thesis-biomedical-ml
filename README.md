# 🏥 Machine Learning for Sensor Data Processing in Biomedical Applications

### Master's Thesis | Universitat Politècnica de Catalunya (UPC) & Norwegian University of Science and Technology (NTNU) | 2020

## 📌 Overview

This master's thesis investigates the application of **machine learning to ICU mortality prediction**, focusing on the relationship between blood glucose, lactate levels, and patient outcomes.

Using the **eICU Collaborative Research Database (v2.0)**, the research develops and compares classification models to investigate whether clinical biomarkers and demographic characteristics can help predict in-hospital mortality.

The project combines large-scale clinical data processing, feature extraction, exploratory analysis, and comparative machine learning evaluation.

## 🎯 Research Objectives

- Investigate the relationship between **glucose, lactate, and ICU mortality**.
- Extract and preprocess clinical information from a large, complex relational database.
- Analyze the predictive relevance of biomarkers and demographic variables.
- Develop and compare multiple **machine learning classification algorithms**.
- Evaluate performance using statistical metrics and computational efficiency.
- Explore the potential of predictive modeling for clinical decision support.

## 🔬 Methodology

| Stage | Description |
|---|---|
| Data Exploration | Investigated the eICU-CRD structure, comprising 31 tables and over 457 million records. |
| Cohort Selection | Constructed a dataset of 59,190 patients with 11 input features and a mortality outcome. |
| Feature Engineering | Extracted glucose and lactate statistics, weight measurements, age, gender, and diabetes information. |
| Data Preprocessing | Addressed missing values, inconsistent measurements, and class imbalance using techniques including SMOTE. |
| Machine Learning | Compared seven classification algorithms using repeated cross-validation. |
| Model Evaluation | Assessed accuracy, ROC-AUC, precision, recall, F1-score, Cohen's Kappa, and computational complexity. |

## 🤖 Machine Learning Models

Seven classification algorithms were investigated:

1. Classification and Regression Tree (CART)
2. Extreme Gradient Boosting (XGBoost)
3. Support Vector Machine (SVM)
4. Logistic Regression
5. Naïve Bayes
6. Linear Discriminant Analysis (LDA)
7. K-Nearest Neighbors (KNN)

## 📊 Key Findings

**XGBoost demonstrated the strongest overall predictive performance** among the seven evaluated algorithms.

| Metric | Reported XGBoost Result |
|---|---|
| Classification Accuracy | ~90% |
| Cohen's Kappa | 0.804 |
| Best-Performing Algorithm | XGBoost |
| Final Study Cohort | 59,190 patients |

The experiments also highlighted the impact of class imbalance, resampling techniques, and computational complexity on model evaluation.

*Results reflect the retrospective experimental methodology described in the 2020 thesis. They do not establish prospective clinical performance or readiness for deployment.*

## 🛠️ Technologies & Tools

**Programming & Analysis:** Python, NumPy, scikit-learn

**Machine Learning:** XGBoost, imbalanced-learn, SMOTE

**Visualization:** Seaborn

**Computing Environment:** Anaconda Spyder, HUNT Cloud (NTNU)

**Documentation:** LaTeX

## 📂 Thesis & Resources

- 📄 [Complete Master's Thesis — Official UPC Repository](https://upcommons.upc.edu/bitstreams/7396bdb9-5e6c-4f97-929a-51fc2c5ddb6f/download)
- 💻 [Associated Machine Learning Code](https://github.com/mani0098/GlucoseLactateMortality)

## 🔒 Data Availability

The eICU Collaborative Research Database contains de-identified clinical records and requires credentialed access through PhysioNet.

Patient-level data are not redistributed in this repository.

[Access eICU-CRD v2.0](https://physionet.org/content/eicu-crd/2.0/)

## 📚 Academic Reference

Rezaeirad, M. (2020). *Machine learning for sensor data processing in biomedical applications* [Master's thesis, Universitat Politècnica de Catalunya]. UPCommons. https://hdl.handle.net/2117/340253

---

**Author:** Mani Rezaeirad  
**Degree:** Master's in Telecommunications Engineering  
**Institution:** Universitat Politècnica de Catalunya (UPC)  
**Research Collaboration:** Norwegian University of Science and Technology (NTNU)

*Exploring the intersection of machine learning, biomedical data, and clinical decision support.*
