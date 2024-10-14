# **OnlineRetail-CustomerSegmentation**

## **Introduction**

This repository presents an analysis of an online retail dataset covering **2009 to 2011**, consisting of over **1.5 million transactions**. It offers insights into customer behavior through key variables such as customer ID, invoice date, invoice number, product description, quantity, price, and country.

The main goal of this analysis is to conduct **customer segmentation** to identify distinct groups based on purchasing patterns, alongside **churn analysis** to detect customers at risk of discontinuation. By achieving these objectives, this project provides stakeholders with actionable insights that can enhance targeted marketing efforts and improve customer retention strategies.

- [Power BI Dashboard Link](https://github.com/NishaChandila/OnlineRetail-Customer-Segmentation/blob/main/Customer-Segmentation-Dashboard.pdf)  
- [Data Cleaning & EDA File](https://github.com/NishaChandila/OnlineRetail-Customer-Segmentation/blob/main/OnlineRetail-DC.ipynb)

You can access the dataset from these links:
- [2009-2010 Dataset](https://www.kaggle.com/datasets/sanlian/online-retail-dataset/data)
- [2010-2011 Dataset](https://www.kaggle.com/datasets/sanlian/online-retail-dataset/data)
---

## **Data Structure**

The dataset used for this analysis was sourced from Kaggle and contains transactional data from an online retail store. It spans two fiscal years: 2009-2010 and 2010-2011.

### **Dataset Preview:**
![Dataset Preview](https://github.com/NishaChandila/project-assets/blob/main/onlineretail-dataset.jpg?raw=true)  

### **Data Columns:**
The dataset includes the following columns, each representing key attributes related to customer transactions:

- **Invoice**: A unique identifier for each transaction or order.
- **StockCode**: An identifier for each product sold. It may represent various items in the inventory.
- **Description**: A textual description of the product corresponding to the StockCode.
- **Quantity**: The number of units sold in each transaction. This can be positive for sales and negative for returns.
- **InvoiceDate**: The date and time when the transaction occurred, providing temporal context for each sale.
- **Price**: The price per unit of the product at the time of purchase. It reflects the monetary value of each item sold.
- **CustomerID**: A unique identifier assigned to each customer. This helps in tracking individual purchasing behavior.
- **Country**: The country where the customer is located, allowing for geographical analysis of sales.

You can access the dataset from these links:
- [2009-2010 Dataset](https://www.kaggle.com/datasets/sanlian/online-retail-dataset/data)
- [2010-2011 Dataset](https://www.kaggle.com/datasets/sanlian/online-retail-dataset/data)

---

## **Executive Summary**

This report presents an analysis of an online retail dataset collected from 2009 to 2011, containing over 1 million transactions. The dataset includes key details such as customer ID, invoice date, invoice number, product description, quantity, price, and country of transaction. Our primary objective was to segment customers based on their purchasing behavior and analyze churn rates to support business decisions aimed at improving customer retention and revenue growth.

![Power BI Dashboard](https://github.com/NishaChandila/project-assets/blob/main/onlineretail1.PNG)

### **Customer Segmentation**

Customer segmentation was carried out to classify customers into different groups based on their purchasing behaviors using the RFM model. The analysis identified regular customers, high-value VIP customers, and churned customers, among others.

Key highlights from the segmentation include:

- **Customer Count by Segment**: The analysis shows that there are approximately 884K total customers, with 346K regular customers and 213K VIP customers.
- **Churn Analysis**: The churn status indicates that 782K customers did not churn, while 101K customers were identified as churned.
- **Revenue Insights**: The majority of the revenue came from the UK, showing the importance of this region for the business, while the total revenue for the period amounted to approximately $9.40M.
- **RFM Score**: The average RFM score across all customers is 11.434, indicating a strong base of frequent, high-value customers.

This segmentation provides actionable insights into customer behavior, allowing for more targeted marketing strategies, personalized offers, and a focus on high-value customer retention.

![Customer Segmentation Visualization](https://github.com/NishaChandila/project-assets/blob/main/onlineretail2.PNG)  

---

## **Data Cleaning and RFM Analysis Summary**

To prepare for customer segmentation analysis, we conducted critical data cleaning and analysis steps:

1. **Missing Values Handling**:
   - **Description**: We addressed 4,382 missing values (0.41%) in the Description column by replacing them with 'Unknown', preserving the context for our analysis.
   - **Customer ID**: For the 243,007 missing CustomerID values (22.76%), we created a new column called CustomerType and labeled these as 'Guest' to represent unregistered transactions.

2. **Outlier Detection**:
   - We identified and removed extreme outliers in the Price and Quantity columns using box plots and the Interquartile Range (IQR) method to ensure that our analysis reflects typical customer behavior without distortion from outliers.

3. **RFM Analysis**:
   - **Recency**: Calculated the number of days since each customer's last purchase.
   - **Frequency**: Counted the total number of purchases made by each customer.
   - **Monetary**: Summed the total amount spent by each customer.
   - **RFM Score**: Combined the scores for recency, frequency, and monetary value to create a composite RFM Score, allowing us to rank customers based on their engagement.
   - **Segmentation**: Categorized customers into segments such as Champions, Loyal Customers, At Risk, Hibernating, and Lost Customers based on their RFM Score, facilitating targeted marketing and engagement strategies.

- [Data Cleaning & EDA File](https://github.com/NishaChandila/OnlineRetail-Customer-Segmentation/blob/main/OnlineRetail-DC.ipynb)

---

## **Recommendations**

Based on the customer segmentation and churn analysis, it is recommended to implement targeted marketing campaigns for high-value and at-risk customers to enhance engagement and retention. Focus on improving customer experience through feedback, and consider product bundling to increase order value. Regularly monitor RFM scores to track customer behavior shifts, and tailor communication based on customer segments. Prioritize the UK market while exploring underperforming regions, and continuously update visualizations to keep stakeholders informed. Finally, use churn analysis insights to address reasons for customer loss and adjust pricing or promotional strategies accordingly.

---

- [Power BI Dashboard Link](https://github.com/NishaChandila/OnlineRetail-Customer-Segmentation/blob/main/Customer-Segmentation-Dashboard.pdf)  
- [Data Cleaning & EDA File](https://github.com/NishaChandila/OnlineRetail-Customer-Segmentation/blob/main/OnlineRetail-DC.ipynb)

You can access the dataset from these links:
- [2009-2010 Dataset](https://www.kaggle.com/datasets/sanlian/online-retail-dataset/data)
- [2010-2011 Dataset](https://www.kaggle.com/datasets/sanlian/online-retail-dataset/data)
