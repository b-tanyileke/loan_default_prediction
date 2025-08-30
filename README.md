# Loan Default Prediction

Predicting loan default using machine learning models.  
This project was developed as part of a data science challenge by [Coursera Project Network](https://www.coursera.org/projects/data-science-coding-challenge-loan-default-prediction) .

---

## 📊 Project Overview
Loan default prediction is a critical task for financial institutions, helping them minimize losses and manage risk.  
This project applies both traditional machine learning methods to predict loan defaults on a large, **highly imbalanced dataset**.

---

## 🛠️ Methods Used
- **Exploratory Data Analysis (EDA):**  
  - Distribution checks 
  - Class imbalance visualization  
  - Correlation heatmaps  

- **Data Preprocessing:**  
  - Handling missing values  
  - Encoding categorical features  
  - Standard scaling numerical features  
  - Train-test split with stratification  

- **Models Implemented:**  
  - Logistic Regression (balanced weights)  
  - Random Forest  
  - Gradient Boosting  
  - LightGBM (with scale_pos_weight)  

- **Evaluation Metrics:**  
  - ROC-AUC Score (main metric)   
  - Confusion Matrices  

---

## 📈 Results
| Model               | ROC-AUC |
|----------------------|---------|
| Logistic Regression  | 0.69    |
| Random Forest        | 0.68    |
| Decision Tree        | 0.67    |
| **LightGBMt**        | **0.76** |

- **LightGBM** achieved the best performance.  
- Handling class imbalance (via `class_weight` and `pos_weight`) significantly improved ROC-AUC.  

![LightGBM Feature Importance](data\lightGBM_gain.png)

---

## Install Dependencies

```bash
git clone https://github.com/b-tanyileke/deeplearn_pipeline_optimizer.git
pip install -r requirements.txt
```
