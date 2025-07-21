# Loan_status_prediction_ML
A loan approval prediction model using Support Vector Machine on a real-world dataset.


##  Loan Approval Prediction using SVM

This project uses **Support Vector Machine (SVM)** to predict whether a loan should be approved or not based on applicant details such as gender, income, education, credit history, and property area. The dataset used comes from a real-world loan application scenario.

---

###  Dataset

The dataset used in this project is from <a herf="https://github.com/Akshitachoudhary/Loan_status_prediction_ML/blob/main/loan_training_data.csv">/Dataset</a>

###  Project Workflow

1. **Data Loading**
   Read CSV data using `pandas`.

2. **Data Cleaning**

   * Handle missing values
   * Encode categorical features
   * Replace `'3+'` in 'Dependents' with `4`
   * Encode target column `'Loan_Status'` to binary (0/1)

3. **Exploratory Data Analysis (EDA)**
   Used Seaborn to visualize the relation between:

   * Education and Loan Status
   * Marital Status and Loan Status
   * Gender and Loan Status

4. **Feature Engineering**

   * Dropped unnecessary columns (`Loan_ID`, `Loan_Status` from features)
   * Converted categorical features into numerical

5. **Model Building**

   * Split data into training and testing sets using `train_test_split`
   * Built a Support Vector Classifier with linear kernel
   * Evaluated accuracy on both training and testing datasets

6. **Prediction**

   * Made a sample prediction and compared it with actual label


###  Model Performance

* **Training Accuracy:** 0.7986111111111112
* **Testing Accuracy:** 0.8333333333333334


###  Dependencies

```bash
pip install numpy pandas seaborn scikit-learn
```


###  How to Run

1. Clone the repo or download the `.ipynb` file
2. Run it in **Jupyter Notebook** or any Python environment
3. Make sure the CSV file path is correct for your system


### Sample Output

```python
prediction = classifier.predict(X_new)
print(prediction)

# Output
[1]
Loan can be Given
Actual: 1
```


