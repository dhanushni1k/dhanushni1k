Here’s a professional and comprehensive README file for your task. You can copy and paste it directly:

---

# Credit Card Fraud Detection using Logistic Regression

## Overview
This project focuses on detecting fraudulent transactions in a credit card dataset using Logistic Regression. The dataset contains transaction details categorized as either legitimate or fraudulent. We employ a supervised learning model to achieve classification with a balanced dataset after applying under-sampling techniques.

## Files Included
- **`credit_data.csv`**: The dataset containing credit card transactions, including features such as transaction amount and a target column (`Class`) indicating legitimate (0) or fraudulent (1) transactions.
- **Python Code**: A script to preprocess the data, train a logistic regression model, and evaluate its performance.

---

## Workflow Steps

### 1. Data Loading
- The dataset is loaded into a Pandas DataFrame.
- Initial exploratory steps include checking the first and last few rows, dataset information, and the presence of missing values.

### 2. Data Exploration
- Analyze the distribution of classes in the dataset to understand the imbalance between legitimate and fraudulent transactions.
- Perform descriptive statistics on the `Amount` column for both classes.

### 3. Data Balancing (Under-Sampling)
- Create a balanced dataset by sampling legitimate transactions to match the number of fraudulent transactions (492 samples each).
- Combine the sampled legitimate transactions and fraudulent transactions into a new dataset.

### 4. Splitting Data
- Separate the features (`X`) and the target (`Y`).
- Split the balanced dataset into training (80%) and testing (20%) subsets, ensuring stratified sampling.

### 5. Model Training
- Train a **Logistic Regression** model using the training data.

### 6. Model Evaluation
- Predict outcomes on the training data.
- Evaluate the model’s performance using **accuracy score**.

---

## Code Snippets and Outputs

### Key Functions
- **`credit_card_data.info()`**: Displays information about the dataset, including column names, non-null values, and data types.
- **`credit_card_data['Class'].value_counts()`**: Shows the distribution of legitimate vs. fraudulent transactions.
- **`legit.sample(n=492)`**: Performs under-sampling to balance the dataset.

### Results
- **Training Accuracy**: Printed at the end of the script as `Accuracy on Training data`.

---

## Dependencies
Ensure you have the following Python libraries installed:
- `numpy`
- `pandas`
- `scikit-learn`

Install dependencies using pip:
```bash
pip install numpy pandas scikit-learn
```

---

## Usage Instructions
1. Place the `credit_data.csv` file in the appropriate directory.
2. Run the script to preprocess the data, train the logistic regression model, and evaluate its performance.
3. Review the accuracy score printed in the output to assess the model's effectiveness.

---

## Key Learnings
This project highlights the importance of:
1. Addressing class imbalance using under-sampling.
2. Implementing Logistic Regression for binary classification tasks.
3. Evaluating machine learning models using metrics like accuracy.

---

## Acknowledgements
This task was completed as part of the **Codetech Machine Learning Internship**, focusing on building practical skills in data preprocessing, machine learning model training, and evaluation.

---
