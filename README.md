# Bank Marketing Prediction using Decision Tree Classifier

## Project Overview
This project predicts whether a customer will purchase a product or service (e.g., a term deposit) based on their demographic and behavioral data. A **Decision Tree Classifier** is used to learn patterns from the historical dataset and make predictions for new customers.

The project also includes visualization of the decision tree and feature importance, making the model interpretable.

---

## Dataset
- The dataset used is the **Bank Marketing Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing).  
- CSV file: `bank.csv`  
- Features include demographic information (age, job, marital, education), financial information (balance, loan, housing), and campaign data (duration, previous contacts, etc.).  
- Target variable: `y` (`yes` = customer purchased, `no` = customer did not purchase)

---

## Features Used
- age
- job
- marital
- education
- default
- housing
- loan
- contact
- month
- day_of_week
- duration
- campaign
- pdays
- previous
- poutcome
- emp.var.rate
- cons.price.idx
- cons.conf.idx
- euribor3m
- nr.employed

---

## Steps in the Project
1. **Import Libraries:** Pandas, scikit-learn, matplotlib, etc.  
2. **Load Dataset:** Load CSV into a DataFrame.  
3. **Explore Data:** Check data types, null values, and target distribution.  
4. **Preprocess Data:** Encode categorical variables into numeric values.  
5. **Split Data:** Separate features (X) and target (y); split into training and testing sets.  
6. **Train Model:** Train a Decision Tree Classifier on the training data.  
7. **Predict:** Make predictions on the test set or new customer data.  
8. **Evaluate Model:** Use accuracy, confusion matrix, and classification report.  
9. **Visualize Decision Tree:** Use Matplotlib to plot the decision tree with a limited depth for readability.  
10. **Feature Importance:** Identify the most important features influencing predictions.  
11. **Predict New Data:** Upload CSV with new customers and get predictions automatically.

---

## How to Run
1. Clone the repository.
2. Install dependencies from `requirements.txt`.
3. Open the Jupyter Notebook or Google Colab file.
4. Follow the cells to:
   - Load the dataset
   - Train the Decision Tree
   - Visualize the tree
   - Upload new customer data for prediction

---

## Example: Predicting a New Customer

```python
new_customer = {
    'age': 40,
    'job': 'technician',
    'marital': 'married',
    'education': 'secondary',
    'default': 'no',
    'housing': 'yes',
    'loan': 'no',
    ...
}
# Convert to DataFrame, encode categorical features, then predict using clf.predict()
