

# **DEFAULT PAYMENT PREDICTION FOR CREDIT CARD CLIENTS**

## **Overview**

This project focuses on predicting the likelihood of default payment among credit card clients using customer demographic, credit, and repayment data. Accurate predictions of default probability are essential for risk management, enabling financial institutions to make informed decisions about credit approval, risk mitigation, and customer prioritization.

---

## **Project Workflow**

### **Problem Statement**
To predict whether a client will default on their credit card payment in the next month, based on historical and demographic data. This prediction can aid in improving risk management strategies and minimizing financial losses for credit institutions.

---

### **Dataset Description**

The dataset includes 23 features related to customer demographic information, past payment history, bill amounts, and payment amounts. The target variable is binary (`default payment`), indicating whether the client defaulted (`Yes = 1`) or did not default (`No = 0`).

#### **Key Features**
- **Demographic Variables**: Gender, age, marital status, and education level.
- **Credit & Payment Variables**: Credit limit, past payment history (`PAY_0` to `PAY_6`), bill amounts, and payment amounts over six months.

---

### **Preprocessing Steps**

1. **Outlier Handling**: Addressed extreme values in continuous variables using IQR-based capping.
2. **Skewness Correction**: Applied transformations to reduce skewness in numeric variables like bill amounts and payment amounts.
3. **Feature Scaling**: Standardized continuous features to ensure consistent scaling.
4. **Feature Selection**: Identified the most impactful variables using techniques such as Random Forest feature importance.

---

### **Data Balancing**
Used Synthetic Minority Oversampling Technique (SMOTE) to address any imbalance in the target variable, ensuring fair representation of both defaulted and non-defaulted cases in training data.

---

## **Model Building**

Built and evaluated multiple machine learning models to determine the best-performing one for this classification task:
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Decision Tree**
- **Random Forest**
- **Gradient Boosting**
- **Naive Bayes**
- **K-Nearest Neighbors (KNN)**

Each model was assessed using metrics like **accuracy**, **precision**, **recall**, **F1-score**, and the **confusion matrix**.

---

### **Hyperparameter Tuning**

Optimized each model using **GridSearchCV** to fine-tune hyperparameters and improve performance.

---

### **Best Model Selection**

The **Random Forest Classifier** was identified as the best model with:
- **Accuracy**: 81% on test data
- **Balanced Precision and Recall**: High scores for both defaulted and non-defaulted cases
- **F1-Score**: Indicating robust overall performance

---

## **Testing with Unseen Data**

The final model was validated on unseen data to ensure generalization, achieving consistent and reliable predictions for client default probabilities.

---

## **Key Learnings**
- **Data Preprocessing**: Proper handling of outliers and skewness significantly improves model performance.
- **Feature Engineering**: Selecting relevant features reduces complexity without sacrificing accuracy.
- **Model Optimization**: Hyperparameter tuning plays a crucial role in boosting accuracy and generalization.

---

## **Future Scope**
1. **Deploy the Model**: Integrate the trained model into financial systems for real-time credit risk analysis.
2. **Explore Advanced Models**: Experiment with ensemble methods and deep learning for further accuracy improvements.
3. **Incorporate External Data**: Use additional data, such as macroeconomic indicators, to refine predictions.
4. **Continuous Learning**: Regularly update the model with new data to maintain relevance and performance.

---

## **Conclusion**

This project successfully demonstrates the use of machine learning techniques to predict credit card default payments with high accuracy. The Random Forest Classifier emerged as the most reliable model, achieving robust performance across key metrics. This solution has the potential to enhance risk management strategies and minimize financial losses for credit institutions.

--- 

## **Acknowledgment**
This project is based on the "Default of Credit Card Clients Dataset" and serves as a foundation for further innovation in predictive modeling for financial risk management.


