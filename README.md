<!-- Project Title -->
# <div align="center">Telecom Customer Churn Analysis and Prediction</div>

<!-- Intro_image -->
<img src="https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/telecom-churn-intro.jpg" alt="figure0_img" width="800"/>


## Business Problem :

### **What is Customer Churn ?**

Customer churn refers to the phenomenon where customers or subscribers stop doing business with a company or discontinue using its services.

In the telecom industry, customers have access to a wide range of service providers and often switch from one to another. Due to this high level of competition, the industry experiences an annual churn rate of approximately 15–25%.

Personalized customer retention is challenging, especially for companies with large customer bases. Devoting significant time and resources to each customer is often not feasible, as the costs can outweigh the benefits. However, if a company could predict which customers are likely to churn in advance, it could strategically focus its retention efforts on these high-risk individuals. The ultimate goal is to retain customer loyalty and expand market reach. Success in this sector is fundamentally tied to understanding and serving the customer.

Churn is a key performance metric because retaining existing customers is significantly more cost-effective than acquiring new ones.

To identify early indicators of churn, organizations need to develop a comprehensive view of customer behavior across multiple touchpoints. By effectively addressing churn, telecom companies can not only protect their market share but also enhance profitability and achieve sustainable growth. The more customers a company retains, the lower the customer acquisition costs and the higher the overall return. Therefore, reducing churn and implementing a targeted retention strategy is central to long-term success.

High customer churn in the telecom industry leading to revenue loss and increased customer acquisition costs.



## Objectives :

- Identify the percentage of customers who have churned and those who continue using the service.

- Analyze the dataset to understand key features that influence customer churn.

- Develop and evaluate machine learning models to accurately classify churned and non-churned customers, and identify the most suitable model for prediction.




## Dataset :

**Telco Customer Churn Data :** [Download Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data)

**The data set includes information about :**

- Customers who left within the last month – the column is called Churn (target column)

- Services that each customer has signed up for – phone service, multiple lines, internet service, online security, online backup, device protection, tech support, and streaming services (TV and Movies)

- Customer account information such as tenure(how long they’ve been a customer), Contract type, payment method, paperless billing, monthly charges, and total charges

- Demographic info about customers such as gender, age range, and if they have partners and dependents


## Few glimpses of Exploratory Data Analysis :

<!-- PLOTS -->
### 1. Churn distribution(in %) :
> ![Churn distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/churn-dist.jpg)
> 26.5% of customers left the company


### 2. gender distribution by churn:
> ![gender dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/gender_distribution_plot.png)
> There is a negligible difference in churn rates between male and female customers. This suggests that gender does not significantly influence a customer’s decision to leave the telecom company. Both genders exhibit similar behavior when it comes to switching to a different service provider.

### 3. Customer Contract :
> ![contract dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/Contract_distribution_plot.png)
> Customers with Month-to-Month contracts show a significantly higher churn rate, with approximately 52% choosing to leave the service as compared to 11% of customers with One Year Contract and 2% with Two Year Contract. This indicates that short-term contracts are strongly associated with a higher likelihood of customers leaving, likely due to the flexibility they offer for switching providers.

### 4. Payment Methods:
> ![Payment method dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/PaymentMethod_distribution_plot.png)
> Customers who used Electronic Check as their payment method had the highest churn rate. In contrast, those who paid through Credit Card (automatic), Bank Transfer (automatic), or Mailed Check were less likely to leave the service.

### 5. Internet services:
> ![Internet services dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/InternetService_distribution_plot.png)
> A large number of customers use Fiber optic service, but it also shows a higher churn rate, which may indicate dissatisfaction with this type of internet connection. In comparison, customers with DSL service or with no internet service show a lower tendency to churn than those using Fiber optic.


### 6. Dependent distribution:
> ![Dependent dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/Dependents_distribution_plot.png)
> Customers without dependents are more likely to churn.

### 7. Online Security:
> ![Online Security dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/OnlineSecurity_distribution_plot.png)
> As shown in the plot, customers without online security are more likely to churn, suggesting that the lack of this feature may contribute to their decision to leave.

### 8. Senior Citizen:
> ![Senior dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/SeniorCitizen_distribution_plot.png)
> Although senior citizens make up a small portion of the overall customer base, they have a higher churn rate compared to other age groups.

### 9. Paperless Billing:
> ![Paperless Billing dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/PaperlessBilling_distribution_plot.png)
>Customers who use Paperless Billing are more likely to churn compared to those who don’t.

### 10. Tech support:
> ![Tech support dist](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/TechSupport_distribution_plot.png)
>As shown in the Plot, customers without Tech Support are more likely to switch to another service provider.


### 11. Distribution w.r.t Charges and Tenure:
>![MonthlyCharges distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/MonthlyCharges_by_churn.png)
>![TotalCharges distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/TotalCharges_by_churn.png)
>![tenure distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/tenure_by_churn.png)
> Customers with higher Monthly Charges are more likely to churn, particularly those who are new to the service. On the other hand, customers with higher Total Charges which typically indicates a longer relationship are less likely to churn.
This supports the finding that newer customers with low tenure tend to have a higher churn rate compared to long-term customers.


## Machine Learning Model Evaluations and Predictions: 
>![Model Performance](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/models_performance.jpg)
> XGBoost is the best overall performer, with strong F1 score, high Recall, and highest Accuracy (tied with RF).

### Predictions
>sample_input = {
    'gender': 'Male',
    'SeniorCitizen': 0,
    'Partner': 'Yes',
    'Dependents': 'Yes',
    'tenure': 72,
    'PhoneService': 'Yes',
    'MultipleLines': 'Yes',
    'InternetService': 'DSL',
    'OnlineSecurity': 'Yes',
    'OnlineBackup': 'Yes',
    'DeviceProtection': 'Yes',
    'TechSupport': 'No',
    'StreamingTV': 'No',
    'StreamingMovies': 'No',
    'Contract': 'Two year',
    'PaperlessBilling': 'No',
    'PaymentMethod': 'Credit card (automatic)',
    'MonthlyCharges': 64.45,
    'TotalCharges': 4720
}
>
>![sample_input data](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/example_input.jpg)

>sample_input2 = {
    'gender': 'Female',
    'SeniorCitizen': 0,
    'Partner': 'Yes',
    'Dependents': 'No',
    'tenure': 28,
    'PhoneService': 'Yes',
    'MultipleLines': 'Yes',
    'InternetService': 'Fiber optic',
    'OnlineSecurity': 'No',
    'OnlineBackup': 'No',
    'DeviceProtection': 'Yes',
    'TechSupport': 'Yes',
    'StreamingTV': 'Yes',
    'StreamingMovies': 'Yes',
    'Contract': 'Month-to-month',
    'PaperlessBilling': 'Yes',
    'PaymentMethod': 'Electronic check',
    'MonthlyCharges': 104.8,
    'TotalCharges': 3046.05
}
>
>![sample_input2 data](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/example_input2.jpg)


## Conclusion :
In conclusion, we analyzed the Telco Customer Churn dataset to understand the factors influencing customer churn. We identified key features such as contract type, tenure, monthly charges, and services used as major contributors to churn.
Using various machine learning models, we developed a predictive model to classify churned and non-churned customers. Among the tested models, XGBoost performed the best with an accuracy of 77% and helped us identify high-risk customers. This prediction model can assist telecom companies in targeting at-risk customers with retention strategies, ultimately reducing churn and improving customer satisfaction.
