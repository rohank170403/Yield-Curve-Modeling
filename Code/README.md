# Credit Risk Modeling Using Machine Learning

## Objective
The primary goal of this project is to develop a credit risk model that predicts the likelihood of a borrower defaulting on a loan. The project applies machine learning techniques to assess various risk factors and classify borrowers based on their creditworthiness.

## Project Steps

### 1. Data Loading and Exploration
- Two datasets (`case_study1.xlsx` and `case_study2.xlsx`) were loaded.
- Initial exploration included checking dataset structure (`.info()`), missing values, and summary statistics.
- Boxplots were used to visualize data distribution and detect outliers.

### 2. Data Preprocessing
- **Handling Missing Values:** Missing data was identified and handled using appropriate imputation techniques.
- **Encoding Categorical Variables:** Categorical features were converted into numerical representations where necessary.
- **Feature Engineering:** New features were derived to enhance model performance.

### 3. Feature Selection
- **Variance Inflation Factor (VIF):** Used to detect and remove highly correlated features.
- **Chi-square Test:** Performed to determine the statistical significance of categorical variables in relation to the target variable.

### 4. Model Building
Three classification models were built and trained:
- **Random Forest Classifier:** An ensemble learning model that constructs multiple decision trees.
- **XGBoost Classifier:** A gradient boosting algorithm optimized for speed and accuracy.
- **Decision Tree Classifier:** A simple yet interpretable model for classification tasks.

### 5. Model Evaluation
- The models were evaluated using:
  - **Accuracy Score**
  - **Precision, Recall, and F1-score** from the classification report.
- **Hyperparameter tuning** was applied to XGBoost using `GridSearchCV`, improving its performance.

## Results and Key Findings

| Model          | Accuracy |
|---------------|----------|
| Random Forest | 76.37%   |
| XGBoost       | 78.00%   |
| Decision Tree | 71.00%   |

- **XGBoost achieved the highest accuracy (78%) after hyperparameter tuning.**
- **Random Forest followed with 76.37% accuracy.**
- **Decision Tree had the lowest performance at 71%.**
- **Classification Reports:** Precision, recall, and F1-score provided further insights into each model’s ability to distinguish between defaulters and non-defaulters.
- **XGBoost’s higher recall suggests better handling of misclassified defaulters.**

## Conclusion
This credit risk modeling project successfully applied machine learning techniques to assess borrower default risk. The models demonstrated varying levels of effectiveness, with **XGBoost outperforming the others** after hyperparameter tuning. These insights can be used for improved risk assessment in financial institutions, enabling more informed lending decisions.

## Installation and Usage
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- XGBoost
