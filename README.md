# Lending Club Loan Prediction

This project aims to predict the likelihood of a borrower defaulting on their loan using machine learning techniques. The dataset contains information about customers' loan applications from Lending Club, and we use this data to build a model that predicts whether a borrower will repay or default on their loan.

## Steps Involved

1. **Data Preprocessing**:
    - Data cleaning was performed to handle missing values and encode categorical variables.
    - Feature scaling was applied using `StandardScaler` to standardize the features, ensuring better model performance.

2. **Handling Imbalanced Data**:
    - The dataset exhibited a significant class imbalance (more loans are repaid than defaulted). To address this, **Random UnderSampling** was used to balance the data, ensuring that the model could effectively learn both classes without being biased toward the majority class.

3. **Model Building**:
    - A **Logistic Regression** model was selected to predict loan defaults. The model was trained on the processed dataset and evaluated using multiple metrics.

4. **Model Evaluation**:
    - The model's performance was evaluated using **Accuracy**, **Precision**, **Recall**, **F1 Score**, and the **Confusion Matrix**.
    - The **ROC Curve** and **AUC Score** were also computed to assess the model's ability to distinguish between defaulters and non-defaulters.

5. **Threshold Tuning**:
    - The optimal decision threshold was chosen to maximize the **F1 Score**, which balances Precision and Recall. Several thresholds between 0.1 and 0.9 were tested to find the best-performing threshold.

## Key Insights

- The model provides insights that help financial institutions assess loan default risk, allowing them to better manage their lending practices.
- The **0.5 threshold** provided a good balance between **Precision** and **Recall**, ensuring that the model was able to detect defaulters while minimizing false positives.

## Conclusion

This project demonstrates the application of machine learning techniques to predict loan defaults. It highlights the importance of handling imbalanced data and tuning the decision threshold for better model performance. The results can assist banks and financial institutions in reducing the risk of loan defaults.
