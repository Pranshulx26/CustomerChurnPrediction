# Telco Customer Churn Prediction

**Problem Statement:**

In the competitive telecom industry, customer retention is paramount. With increasing competition and the ease of switching providers, understanding and predicting customer churn is crucial. Churn, the rate at which customers discontinue their services, directly impacts a company's revenue. By analyzing various factors such as demographics, service usage, and contract terms, we can build predictive models to identify customers at risk of churning.

**Aim:**

To classify customers as potential churners based on given numerical and categorical features. This is a binary classification problem for an imbalanced dataset.

**About the Dataset:**

**A fictional telco company that provided home phone and Internet services to 7043 customers in California in Q3.**

**Customer Information:**

* **CustomerID:** A unique ID that identifies each customer.
* **Count:** A value used in reporting/dashboarding to sum up the number of customers in a filtered set.
* **Country:** The country of the customer’s primary residence.
* **State:** The state of the customer’s primary residence.
* **City:** The city of the customer’s primary residence.
* **Zip Code:** The zip code of the customer’s primary residence.
* **Lat Long:** The combined latitude and longitude of the customer’s primary residence.
* **Latitude:** The latitude of the customer’s primary residence.
* **Longitude:** The longitude of the customer’s primary residence.

**Customer Demographics:**

* **Gender:** The customer’s gender: Male, Female
* **Senior Citizen:** Indicates if the customer is 65 or older: Yes, No
* **Partner:** Indicate if the customer has a partner: Yes, No
* **Dependents:** Indicates if the customer lives with any dependents: Yes, No. Dependents could be children, parents, grandparents, etc.

**Customer Services:**

* **Tenure Months:** Indicates the total amount of months that the customer has been with the company by the end of the quarter specified above.
* **Phone Service:** Indicates if the customer subscribes to home phone service with the company: Yes, No
* **Multiple Lines:** Indicates if the customer subscribes to multiple telephone lines with the company: Yes, No
* **Internet Service:** Indicates if the customer subscribes to Internet service with the company: No, DSL, Fiber Optic, Cable.
* **Online Security:** Indicates if the customer subscribes to an additional online security service provided by the company: Yes, No
* **Online Backup:** Indicates if the customer subscribes to an additional online backup service provided by the company: Yes, No
* **Device Protection:** Indicates if the customer subscribes to an additional device protection plan for their Internet equipment provided by the company: Yes, No
* **Tech Support:** Indicates if the customer subscribes to an additional technical support plan from the company with reduced wait times: Yes, No
* **Streaming TV:** Indicates if the customer uses their Internet service to stream television programing from a third party provider: Yes, No. The company does not charge an additional fee for this service.
* **Streaming Movies:** Indicates if the customer uses their Internet service to stream movies from a third party provider: Yes, No. The company does not charge an additional fee for this service.

**Customer Account Information:**

* **Contract:** Indicates the customer’s current contract type: Month-to-Month, One Year, Two Year.
* **Paperless Billing:** Indicates if the customer has chosen paperless billing: Yes, No
* **Payment Method:** Indicates how the customer pays their bill: Bank Withdrawal, Credit Card, Mailed Check
* **Monthly Charge:** Indicates the customer’s current total monthly charge for all their services from the company.
* **Total Charges:** Indicates the customer’s total charges, calculated to the end of the quarter specified above.

**Customer Churn Information:**

* **Churn Label:** Yes = the customer left the company this quarter. No = the customer remained with the company. Directly related to Churn Value.
* **Churn Value:** 1 = the customer left the company this quarter. 0 = the customer remained with the company. Directly related to Churn Label.
* **Churn Score:** A value from 0-100 that is calculated using the predictive tool IBM SPSS Modeler. The model incorporates multiple factors known to cause churn. The higher the score, the more likely the customer will churn.
* **CLTV:** Customer Lifetime Value. A predicted CLTV is calculated using corporate formulas and existing data. The higher the value, the more valuable the customer. High value customers should be monitored for churn.
* **Churn Reason:** A customer’s specific reason for leaving the company. Directly related to Churn Category.

## **Exploratory Data Analysis (EDA)**

[Include detailed insights from the EDA, including visualizations and key findings]

## **Data Preprocessing**

* **Handling Missing Values:** Impute missing values using appropriate techniques.
* **Feature Engineering:** Create new features from existing ones to capture additional insights.
* **Data Scaling:** Normalize numerical features to a common scale.
* **Data Balancing:** Address class imbalance using oversampling techniques.

## **Model Development**

**Model Selection:**

* **XGBoost**
* **LightGBM**
* **Random Forest**
* **Decision Tree**

**Model Training and Evaluation:**

* Train and evaluate models using appropriate metrics like accuracy, precision, recall, F1-score, and ROC-AUC.
* Perform hyperparameter tuning to optimize model performance.

**Model Stacking:**

* Combine multiple models to create a more powerful ensemble model.
* Train a meta-model on the predictions of the base models to make the final prediction.

## **Results**

**Model Performance:**

* **XGBoost:** Cross-Validation Score: 90.86%, ROC-AUC Score: 90.36%
* **LightGBM:** Cross-Validation Score: 91.04%, ROC-AUC Score: 90.62%
* **Random Forest:** Cross-Validation Score: 87.01%, ROC-AUC Score: 85.98%
* **Decision Tree:** Cross-Validation Score: 85.28%, ROC-AUC Score: 84.30%
* **Stacking Model:** Cross-Validation Score: 91.59%, ROC-AUC Score: 91.36%

## **Conclusion**

By leveraging data-driven insights and advanced machine learning techniques, we have developed a robust model to predict customer churn. This model can be used to identify customers at risk of churning and implement targeted retention strategies.

**Key Insights and Recommendations:**

* **Customer Segmentation and Personalized Marketing:**
  * Segment customers based on demographics, service usage, and churn risk to tailor marketing efforts.
  * Implement a loyalty program to reward loyal customers.
  * Offer flexible contract options to cater to diverse customer needs.
* **Service Quality and Customer Support:**
  * Prioritize customer satisfaction by investing in robust customer support channels.
  * Implement proactive customer service to anticipate and address issues.
  * Monitor service quality to identify areas for improvement.
* **Pricing and Bundling Strategies:**
  * Offer competitive pricing and explore bundling opportunities.
  * Consider tiered pricing to meet diverse customer needs.
* **Data-Driven Decision Making:**
  * Leverage data analytics to gain insights into customer behavior and preferences.
  * Implement a data governance framework to ensure data quality and security.
  * Utilize predictive analytics to forecast churn and proactively address customer needs.
* **Continuous Improvement:**
  * Regularly review and refine strategies to stay updated on industry trends.
  * Conduct customer surveys and feedback analysis to improve products and services.
  * Embrace innovation to enhance customer experience.

By implementing these strategies, the Telco company can effectively address customer concerns, improve customer satisfaction, and reduce churn.
