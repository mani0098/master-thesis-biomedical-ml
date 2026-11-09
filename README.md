# 🏥 Machine Learning for Sensor Data Processing in Biomedical Applications

### Master's Thesis | Universitat Politècnica de Catalunya (UPC) & Norwegian University of Science and Technology (NTNU) | 2020

**📄 [Read the Complete Thesis — Official UPC PDF](https://upcommons.upc.edu/bitstreams/7396bdb9-5e6c-4f97-929a-51fc2c5ddb6f/download)** · [UPC publication record](https://upcommons.upc.edu/entities/publication/b424e102-8063-4b25-a467-633a4358bc51)

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

![Cohort selection process](fig/chapter3/Cohort%20Selection%20Process.jpg)

*Figure: Patient cohort selection from the eICU-CRD dataset (original thesis).*

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

![Algorithm comparison using SMOTE and repeated stratified cross-validation](fig/chapter5/Algorithm%20Comparison%20%28SMOTE%2C%20RSKFold%29.png)

*Figure: Comparison of classification algorithms after applying SMOTE, as reported in the thesis.*

*Results reflect the retrospective experimental methodology described in the 2020 thesis. They do not establish prospective clinical performance or readiness for deployment.*

## 🛠️ Technologies & Tools

**Programming & Analysis:** Python, NumPy, scikit-learn

**Machine Learning:** XGBoost, imbalanced-learn, SMOTE

**Visualization:** Seaborn

**Computing Environment:** Anaconda Spyder, HUNT Cloud (NTNU)

**Documentation:** LaTeX

## 📁 Repository Structure

This repository preserves the **editable LaTeX thesis source** and its original figures:

| File / Directory | Description |
|---|---|
| [`main.tex`](main.tex) | Main document that assembles the thesis chapters |
| [`TexFiles/`](TexFiles/) | Abstract, chapters, conclusions, glossary, and supporting LaTeX files |
| [`TexFiles/mylib.bib`](TexFiles/mylib.bib) | Bibliographic references |
| [`TexFiles/sty.sty`](TexFiles/sty.sty) | Document formatting and LaTeX packages |
| [`fig/`](fig/) | Figures, diagrams, and evaluation plots |
| [`TitlePage.pdf`](TitlePage.pdf) | Title page only, **not** the full thesis |

Start with [`main.tex`](main.tex) to inspect or edit the document. Keep the relative structure of `TexFiles/` and `fig/` intact so the LaTeX references continue to work. The **official UPC PDF linked at the top** is the published, complete thesis.

## 📂 Thesis & Resources

- 📄 [Complete Master's Thesis — Official UPC Repository](https://upcommons.upc.edu/bitstreams/7396bdb9-5e6c-4f97-929a-51fc2c5ddb6f/download)
- 💻 [Associated Machine Learning Code](https://github.com/mani0098/GlucoseLactateMortality)

## 🔗 Related Work — IT Academy Final Project (2026)

Six years later, I revisited **eICU-CRD v2.0** for a different clinical prediction task: identifying lung cancer patients at risk of a **prolonged ICU stay (>5 days)** using data available during the **first 24 hours** of admission.

[Explore the 2026 project: Early Prediction of Prolonged ICU Stay in Lung Cancer Patients](https://github.com/mani0098/ITA_Data_Analytics/tree/main/Sprint%2013.%20Final%20project)

The two projects illustrate a progression from biomarker-based mortality prediction to early risk stratification for ICU length of stay.

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
