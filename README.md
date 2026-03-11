# Antimicrobial Resistance (AMR) Prediction using Machine Learning

This repository contains materials related to the research paper:

**Improving Antimicrobial Resistance (AMR) Phenotype Prediction for Unseen Bacteria through Data Augmentation and Machine Learning**

Published at **ACM BCB Companion 2025**  
ACM International Conference on Bioinformatics, Computational Biology and Health Informatics  
Philadelphia, USA

Paper  
https://doi.org/10.1145/3768322.3769015

---

# Overview

Antimicrobial resistance (AMR) is a growing global health threat and a major challenge for modern medicine.  
Accurate prediction of antimicrobial resistance from genomic data is difficult due to limited labeled datasets and severe class imbalance.

This research investigates machine learning and deep learning approaches to improve AMR phenotype prediction using genomic data.

The proposed framework integrates:

- k-mer based genomic feature extraction
- tree-based ensemble models
- deep learning using a 1D Convolutional Neural Network (CNN)
- data augmentation techniques to address data scarcity

The results demonstrate that combining feature engineering, data augmentation, and deep learning significantly improves prediction performance.

---

# Research Pipeline

The experimental pipeline includes the following steps:

1. Download genomic AMR datasets from the **BV-BRC database**
2. Extract genomic features using **k-mer frequency analysis (k = 10)**
3. Select the most important features using **tree-based feature importance**
4. Construct a feature matrix for classification
5. Apply **SMOTE data augmentation** to address class imbalance
6. Train machine learning and deep learning models
7. Evaluate performance using cross-validation and test datasets

---

# Models Evaluated

### Machine Learning Models

- Random Forest (RF)
- Extra Trees (ET)
- XGBoost (XGB)

Hyperparameter tuning methods:

- Bayesian Optimization
- Randomized Search
- Grid Search

### Deep Learning Model

- **Deep 1D Convolutional Neural Network (CNN)** implemented in PyTorch

CNN models were trained using augmented datasets to improve generalization.

---

# Dataset

The dataset was obtained from the **BV-BRC (Bacterial and Viral Bioinformatics Resource Center)**.

The study evaluates multiple genome–antibiotic combinations, including:

- *Enterococcus faecium* – Vancomycin
- *Escherichia coli* – Ampicillin
- *Acinetobacter baumannii* – Amikacin
- *Salmonella enterica* – Chloramphenicol

Each task performs classification of bacterial strains as:

- Resistant
- Susceptible

---

# Key Techniques

This study combines several important techniques:

- **k-mer genomic feature extraction**
- **Feature importance based feature selection**
- **SMOTE data augmentation**
- **Hyperparameter optimization**
- **Deep learning with CNN architectures**

---

# Key Findings

The experimental results show that:

- Tree-based ensemble models perform well in **small dataset scenarios**
- CNN models significantly benefit from **data augmentation**
- Augmented CNN models achieve **higher prediction accuracy and robustness**
- The proposed approach generalizes well to **previously unseen bacteria**

The results demonstrate that combining machine learning, deep learning, and data augmentation can improve AMR prediction performance in data-limited environments.

---

# Publication

Yeojin Jung*, Namkyeong Kim*, Donghoon Kim  

**Improving Antimicrobial Resistance (AMR) Phenotype Prediction for Unseen Bacteria through Data Augmentation and Machine Learning**

ACM BCB Companion 2025

DOI  
https://doi.org/10.1145/3768322.3769015

\* Both authors contributed equally to this research.

---

# Authors

- Yeojin Jung — Arkansas State University  
- Namkyeong Kim — Arkansas State University  
- Donghoon Kim — Arkansas State University
