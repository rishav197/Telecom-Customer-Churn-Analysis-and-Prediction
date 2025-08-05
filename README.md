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
> 26.5 % of customers left the company

### 2. Distribution of features - 'tenure', 'MonthlyCharges', 'TotalCharges' :
> ![tenure distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/tenure_distribution_boxplot.png)
> ![MonthlyCharges distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/MonthlyCharges_distribution_boxplot.png)
> ![TotalCharges distribution](https://github.com/rishav197/Telecom-Customer-Churn-Analysis-and-Prediction/blob/main/plots-and-images/TotalCharges_distribution_boxplot.png)
> these feature has no outliers

## Machine Learning Model Evaluations and Predictions: 




## Conclusion :
In this project, we analyzed the Telco Customer Churn dataset to understand the factors influencing customer churn. We identified key features such as contract type, tenure, monthly charges, and services used as major contributors to churn.

Using various machine learning models, we developed a predictive model to classify churned and non-churned customers. Among the tested models, [insert best model name] performed the best with an accuracy of [insert score] and helped us identify high-risk customers.

This prediction model can assist telecom companies in targeting at-risk customers with retention strategies, ultimately reducing churn and improving customer satisfaction.

In the future, the model can be improved further by incorporating more behavioral data or deploying it in real-time systems for proactive retention efforts.


