# Customer-Churn-Prediction-Model
This repository contains a machine learning project aimed at predicting customer churn (i.e., the likelihood of customers leaving the service) for American Express. The project covers data preprocessing, model building, evaluation, and interpretability using Python.

## 📁 Project Structure

```
├── American Express User Exit Pred.csv       # Input dataset
├── AmericanExpressImplementation.ipynb       # Python implementation notebook
├── README.md                                 # Project documentation
```

## 📊 Dataset

The dataset contains 9,927 records with the following features:

* **Credit Score**
* **Geography** (France, Spain, Germany)
* **Gender**
* **Age**
* **Tenure** (years as customer)
* **Balance** (account balance)
* **NumOfProducts** (number of bank products)
* **HasCrCard** (owns a credit card)
* **IsActiveMember**
* **EstimatedSalary**
* **Exited** (target label: 1 = exited, 0 = retained)

## 🧠 Models Used

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

Each model was trained and tested on an 80/20 stratified split of the dataset. Hyperparameter tuning was done using GridSearchCV.

## 🧪 Performance Metrics

| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Logistic Regression | 0.80     | 0.75      | 0.60   | 0.67     | 0.85    |
| Random Forest       | 0.86     | 0.82      | 0.70   | 0.75     | 0.92    |
| XGBoost             | 0.88     | 0.84      | 0.74   | 0.79     | 0.94    |

## 📌 Key Features Influencing Churn

* Age
* Balance-to-Salary Ratio
* Tenure
* Number of Products
* Credit Score

## 🔍 Insights & Business Implications

* Younger, single-product customers are more likely to churn.
* Customers with high balances and low salary should be targeted for retention.
* Cross-selling and loyalty offers can help improve retention.

## 🛠️ Technologies Used

* Python 3.9
* pandas, numpy
* scikit-learn
* xgboost
* matplotlib, seaborn

## 📈 Future Enhancements

* Incorporate transaction data and behavioral signals.
* Deploy as a web app with real-time prediction.
* Implement SHAP/LIME-based dashboards for model explainability.

## 📄 License

This project is for educational purposes and is licensed under the MIT License.

## 👨‍💻 Author

Jatin Goyal – Third Year CSE Student

---

> For a full walkthrough, refer to the [Churn Prediction Model File].
