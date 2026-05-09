Loan Approval & Credit Risk Analysis
This project utilizes Machine Learning to predict loan eligibility and estimate maximum loan amounts for potential clients. By implementing Decision Tree Regression and Classification models, the system evaluates borrower risk based on financial and demographic attributes.

## Project Overview
The goal of this project is to automate the credit risk assessment process. It involves:

- Data Preprocessing: Handling missing values, outliers, and feature scaling using StandardScaler.

- Feature Engineering: Encoding categorical variables (e.g., Home Ownership, Loan Intent) for model compatibility.

- Modeling: Training and optimizing Decision Tree models to predict both categorical (Approval) and continuous (Loan Amount) targets.

- Inference: A dedicated pipeline to scale and predict outcomes for new, unseen client data.


## Technical Stack
- Language: Python

- Environment: Google Colab / Jupyter Notebook

- Libraries:
    - Pandas & NumPy (Data Manipulation)
    - Scikit-Learn (Machine Learning & Scaling)
    - Joblib (Model Serialization)
    - Matplotlib & Seaborn (EDA)
 

## Project Structure
- Notebook 1: Exploratory Data Analysis (EDA), Data Cleaning, and Feature Scaling.
- Notebook 2: Model Training, Hyperparameter Tuning, and Evaluation (MAE, $R^2$).
- Notebook 3: Deployment/Inference pipeline for predicting specific client cases.
- Models: Saved .joblib files for the Scaler and the trained Decision Tree models.


## Key Findings
The baseline Decision Tree (DT-1) outperformed the optimized version in this specific dataset, achieving an $R^2$ of 0.945, indicating a high level of predictive accuracy. The most influential features in determining loan amounts were Annual Income, Employment Length, and the Loan-to-Income Ratio.


## How to Use
1. Clone the repository.
2. Ensure all .joblib files and datasets are in the same directory.
3. Run the notebooks in sequence (1 through 3).
4. To predict a new client, input the raw attributes in the inference section of Notebook 3; the script will automatically handle the scaling and encoding.
