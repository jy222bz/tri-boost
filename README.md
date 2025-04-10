# *TriBoost*: Cyberthreat Profiling in Networks using *Machine Learning*

## Project Overview

This project employs a data-driven experimental research methodology, utilizing the classical machine learning model *Random Forest* alongside modern models such as *TabNet* and *XGBoost* to classify network activities. The objective is to compare and analyze their performance and efficiency within **Intrusion Detection System (IDS)** applications. Additionally, the study utilizes a publicly available dataset encompassing benign and malicious patterns.

## Objectives

- Apply machine learning techniques to classify network activities.
- Optimize machine learning models through hyperparameter tuning using the *optuna* framework and evaluate their performance.

## Dataset Information

The dataset used in this project is a reasonable benchmark for network intrusion detection systems. This dataset is cited from the following sources:

- Moustafa, N., & Slay, J. (2015, November). UNSW-NB15: A comprehensive data set for network intrusion detection systems (UNSW-NB15 network data set). *2015 Military Communications and Information Systems Conference (MilCIS)*, pp. 1-6. IEEE.
- Moustafa, N., & Slay, J. (2016). The evaluation of network anomaly detection systems: Statistical analysis of the UNSW-NB15 data set and the comparison with the KDD99 data set. *Information Security Journal: A Global Perspective, 25*(1-3), 18-31.

This dataset comprises approximately **162,745 rows** and over **40 features**. The classes in the dataset are imbalanced and represent the following ten types of network activities:

1. **Analysis**  
2. **Backdoor**  
3. **DoS** 
4. **Exploits**  
5. **Fuzzers**  
6. **Generic**  
7. **Normal**  
8. **Reconnaissance**  
9. **Shellcode**  
10. **Worms**
  

## Project Workflow

### Data Preparation

1. **Data Preprocessing:**  
   The dataset is cleaned by handling missing values and converting all features to a numeric format suitable for machine learning models.

2. **Data Splitting:**  
   The data is divided into training, validation, and testing sets.

| **Dataset Split** | **Percentage** |
|-------------------|----------------|
| Training Set      | 70%            |
| Validation Set    | 15%            |
| Test Set          | 15%            |
| **Total**         | **100%**       |

---

### Model Training and Hyperparameter Tuning

The project uses **Random Forest**, **TabNet**, and **XGBoost** classification models. The models underwent a Hyperparameter Optimization Process to achieve optimal performance using the same dataset with **100 trials**, respectively. 

---

### Model Evaluation and Feature Analysis
**Performance Evaluation:**  
The models with the best parameters are tested on the validation and testing sets to assess their performance using *Accuracy*, *F1*, *Precision*, and *Recall*.

---

## Instructions for Running the Project

### Prerequisites

Ensure Python 3.8 or later is installed on the system. The project requires several Python libraries, including:

- `matplotlib`
- `numpy`
- `optuna`
- `pandas`
- `scikit-learn`
- `seaborn`
- `tabnet`
- `torch`
- `xgboost`

---

### Installing Dependencies

Run the following command to install all dependencies:

```bash
pip install -r requirements.txt

```

### For Anaconda users
Ensure Anaconda is installed on the system and then import the `environment.yaml`. If not, download and install it from the [official Anaconda website](https://www.anaconda.com/).

Clone the project repository:

```bash
git clone https://github.com/jy222bz/tri-boost.git
```


## Author

**Jacob Yousif** 