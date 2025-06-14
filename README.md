# Task 2: Credit Risk Prediction

## 🎯 Objective
The goal of this task is to build a machine learning model that can predict whether a loan applicant is likely to **default** on a loan (Loan_Status). The task involves data preprocessing, exploratory data analysis (EDA), model training, and evaluation.

## 📁 Dataset
- **Dataset Name**: Loan Prediction Dataset  
- **Source**: Available on Kaggle ([search for "Loan Prediction Problem"] or upload CSV manually)
- **Target Variable**: `Loan_Status` (Y = approved, N = not approved)

## 🛠️ Libraries Used
- `pandas` for data manipulation  
- `seaborn` and `matplotlib` for visualization  
- `scikit-learn` for preprocessing, modeling, and evaluation  

## 🔍 Steps Performed

### 1. Load and Inspect the Dataset
- Used `pandas.read_csv()` to load the dataset.
- Displayed basic structure using `.shape`, `.columns`, and `.head()`.

### 2. Handle Missing Values
- Imputed missing numerical columns (e.g., `LoanAmount`) with **median**.
- Imputed missing categorical columns with **mode**.

### 3. Exploratory Data Analysis (EDA)
- Plotted:
  - Histogram of `LoanAmount` and `ApplicantIncome`.
  - Count plot of `Education` vs `Loan_Status`.

### 4. Data Preprocessing
- Dropped `Loan_ID` (not relevant).
- Encoded categorical variables using `LabelEncoder`.
- Split the data into features `X` and target `y`.
- Performed a train-test split (80% train, 20% test).

### 5. Model Training
- Trained two classifiers:
  - **Logistic Regression**
  - **Decision Tree Classifier**

### 6. Model Evaluation
- Measured accuracy using `accuracy_score`.
- Evaluated using **confusion matrix** and **classification report**.


## 📊 Results

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression| ~80%     |
| Decision Tree      | ~75%     |


## 📌 Key Skills Demonstrated
- ✅ Handling missing data  
- ✅ Exploratory data analysis (EDA)  
- ✅ Binary classification modeling  
- ✅ Model evaluation with confusion matrix and accuracy

## 🧠 Future Improvements
- Try advanced models (e.g., XGBoost, Random Forest)
- Perform cross-validation
- Tune hyperparameters
- Use one-hot encoding instead of label encoding for better performance
