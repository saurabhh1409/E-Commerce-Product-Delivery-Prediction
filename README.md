# E-Commerce-Product-Delivery-Prediction

## Project Overview
In the modern e-commerce industry, timely delivery is crucial to customer satisfaction and brand reputation. This project focuses on predicting whether a product will be delivered on time based on various logistical, customer, and product-related factors. Using a supervised machine learning approach, the model classifies deliveries as on-time or late, helping businesses optimize their operations and reduce delays.

## Dataset Summary
Dataset Size: 10,999 rows × 12 columns<br>
Source: Internal e-commerce operations data from Indian IT cities<br>
Objective: Predict whether a product delivery will reach the customer on time (Reached.on.Time_Y.N)<br>

## Data Dictionary

| Column Name             | Description                                                                                  |
|-------------------------|----------------------------------------------------------------------------------------------|
| **ID**                  | Unique customer ID                                                                           |
| **Warehouse_block**     | The warehouse block from where the order was dispatched (A, B, C, D, or E)                   |
| **Mode_of_Shipment**    | Mode used to ship the product (Ship, Flight, or Road)                                        |
| **Customer_care_calls** | Number of customer care calls made by the customer for order inquiries                       |
| **Customer_rating**     | Customer rating of the service (1 = Worst, 5 = Best)                                         |
| **Cost_of_the_Product** | Cost of the product in USD                                                                   |
| **Prior_purchases**     | Number of times the customer has made purchases before                                       |
| **Product_importance**  | Importance of the product (Low, Medium, or High)                                             |
| **Gender**              | Gender of the customer (Male or Female)                                                      |
| **Discount_offered**    | Discount offered on the product                                                              |
| **Weight_in_gms**       | Weight of the product in grams                                                               |
| **Reached.on.Time_Y.N** | **Target Variable**: 1 = NOT reached on time, 0 = Reached on time                            |


## Project Workflow
 1. Data Preprocessing
        - Handling missing values (if any)
        - Encoding categorical variables (e.g., Gender, Shipment Mode)
        -Feature scaling and transformation

 2. Exploratory Data Analysis (EDA)
        -Distribution of on-time vs late deliveries
        -Relationship between delays and product weight, shipment mode, etc.
        -Correlation heatmaps and boxplots

 3. Model Building
        -Logistic Regression, Decision Tree, Random Forest, XGBoost
        -Cross-validation and hyperparameter tuning
        -Evaluation metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC

## Conclusion
This project demonstrates how machine learning can effectively predict whether an e-commerce order will be delivered on time. Key factors like shipment mode, product weight, and discount offered significantly impact delivery performance. The model can help businesses reduce delays and improve logistics efficiency.

The aim of the project was to predict whether the product from an e-commerce company will reach on time or not. This project also analyzes various factors that affect the delivery of the product as well as studies the customer behavior. From the exploratory data analysis, I found that the product weight and cost has an impact on the product delivery. Where product that weighs between 2500 - 3500 grams and having cost less than 250 dollars had higher rate of being delivered on time. Most of the products were shipped from warehouse F though ship, so it is quite possible that warehouse F is close to a seaport.

The customer's behaviour also help in predicting the timely delivery of the product. The more the customer calls, higher the chances the product delivery is delayed. Interestingly, the customers who have done more prior purchases have higher count of products delivered on time and this is the reason that they are purchasing again from the company. The products that have 0-10% discount have higher count of products delivered late, whereas products that have discount more than 10% have higher count of products delivered on time.


