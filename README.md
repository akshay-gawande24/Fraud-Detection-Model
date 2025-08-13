# Fraud Detection Model

## Project Overview  
This project focuses on developing a machine learning model to proactively detect fraudulent financial transactions. The goal is to build an effective and robust system that can identify patterns indicative of fraud within a large transactional dataset, providing an actionable tool for a financial company to prevent financial losses and protect its customers.

## Key Features and Techniques  

-  Data Cleaning & Preprocessing:   
   The project involved comprehensive data cleaning, including outlier treatment through capping to preserve valuable data points, which are often indicative of fraudulent behavior.

-  Feature Engineering:   
   New, highly predictive features were engineered from existing data, such as `balanceDiffOrig` and `balanceDiffDest`, to highlight anomalies in account balances.

-  Handling Imbalanced Data:   
   The dataset had a severe class imbalance (less than 1% fraud). This was addressed using the SMOTE (Synthetic Minority Over-sampling Technique) method to balance the training data, enabling the model to learn from the    minority class.

-  Model Selection:   
   An XGBoost Classifier was chosen for its strong performance and robustness, particularly for imbalanced datasets.

-  Model Fine-Tuning:   
   The model's decision threshold was fine-tuned to balance the trade-off between Precision (minimizing false alarms) and Recall (catching all fraud), resulting in a practical and effective solution.

## Performance and Results 

-  Recall:   
   The model achieved a high recall score, indicating its ability to successfully identify the majority of fraudulent transactions.

-  Precision:   
   The precision score was significantly improved through fine-tuning, demonstrating the model's reduced number of false positives.

-  F1-Score:   
   A high F1-score was achieved, reflecting a strong and practical balance between precision and recall, which is essential for a real-world fraud detection system.

## Technical Stack  
-  Python  
-  Pandas & NumPy  
-  Scikit-learn  
-  XGBoost  
-  Imbalanced-learn  
-  Matplotlib & Seaborn  

## How to Run the Project  
1. Clone this repository.  
2. Install the required dependencies using:
   ```bash
   pip install -r requirements.txt
3. Open and run the Jupyter Notebook Fraud Detection Model.ipynb to see the complete data analysis, model training, and evaluation pipeline.
