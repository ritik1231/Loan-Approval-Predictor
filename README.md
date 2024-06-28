# Loan-Approval-Predictor
This notebook explores a loan approval dataset and builds predictive models to assess loan eligibility. 

## Dataset

The dataset contains information about loan applicants, including their demographics, financial status, and loan details. Features include:

* **Gender:** Male/Female
* **Married:** Yes/No
* **Dependents:** Number of dependents
* **Education:** Graduate/Not Graduate
* **Self_Employed:** Yes/No
* **ApplicantIncome:** Applicant's income
* **CoapplicantIncome:** Co-applicant's income
* **LoanAmount:** Loan amount applied for
* **Loan_Amount_Term:** Loan term in months
* **Credit_History:** Credit history (0 or 1)
* **Property_Area:** Urban/Semiurban/Rural
* **Loan_Status:** Loan approval status (Y/N) - Target variable

## Steps

1. **Data Preprocessing:**
   - Handling categorical variables using Label Encoding.
   - Addressing missing values by imputation.
   - Feature engineering by creating a 'TotalIncome' feature.

2. **Exploratory Data Analysis:**
   - Visualizing categorical variable distributions.
   - Examining correlations using a heatmap.
   - Exploring relationships between features using categorical plots.

3. **Model Training and Evaluation:**
   - Splitting the dataset into training and testing sets.
   - Training multiple classification models (KNeighborsClassifier, RandomForestClassifier, SVC, LogisticRegression).
   - Evaluating models using accuracy, precision, recall, and F1-score.

4. **Feature Scaling:**
   - Scaling features using StandardScaler.
   - Re-evaluating models after scaling.

5. **Cross-Validation:**
   - Performing 10-fold cross-validation to assess model generalization.

## Conclusion

Based on both initial and post-scaling evaluations, as well as cross-validation, **LogisticRegression** consistently demonstrates the best performance for loan approval prediction. It achieves a high accuracy, balanced precision and recall, and strong F1-score.
