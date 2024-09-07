# RFM Segmentation and K-Means Clustering: Optimizing Customer Insights Using Elbow Method - Marketing and Customer Analytics
---
### -  Introduction/Background
RetailCo is a medium-sized retail company specializing in consumer goods, operating through multiple channels, including in-store purchases, online sales, and direct marketing campaigns. Offering a wide range of 
products, such as groceries, electronics, fashion, and household goods, RetailCo aims to improve customer  satisfaction and increase profitability by understanding customer behavior and optimizing its marketing strategies. 
The primary objective of RetailCo is to increase customer retention and maximize customer lifetime value by leveraging data analytics to identify high-value customers who are more likely to make repeat purchases, allowing 
the company to focus on those who contribute most to revenue. Additionally, RetailCo aims to optimize marketing efforts by targeting customers based on their purchasing behavior, thereby ensuring more relevant and effective 
marketing campaigns. Improved inventory management is another key focus, as understanding product demand patterns will help align stock levels with customer needs, reducing excessive inventory costs.  

### - Dataset Description
The dataset comes from Retail Store Sales Transactions (Scanner Data) (kaggle.com). This dataset includes 64.682 transactions of 5.242 SKU's sold to 22.625 customers during one year. The dataset contains the following 
key attributes:
- Date: The data when the transaction occured.
- Customer_ID : A unique identifier for each customer.
- Transaction_ID : A unique identifier for each transaction.
- SKU_Category : The category of the product purchased (e.g., electronics, groceries)
- SKU : Stock Keeping Unit, a unique identifier for each product.
- Quantity : The quantity of each product purchased in a transaction.
- Sales_Amount : The total sales amount of the transaction. 

### - Methods
1. RFM (Recency, Frequency and Monetary) 

RFM is very valuable in predicting response and can boost a company’s profits in a short term, and it is a long-familiar method to measure the strength of customer relationship as RFM can effectively 
identify valuable customers. In this model, recency measures the interval between the most recent transaction time and the analyzing time. Frequency measures the purchase frequency within a 
specified period. Monetary measures the total monetary expenditure within a specified period. This section introduces a designated RFM model to analyze the relative profitability for each customer 
cluster from the segmentation result after purchase-based segmentation algorithm.

2. K-Means

K-means is the mostly popular and widely used algorithm for grouping data into groups to get right number of clusters. K-means is an iterative Algorithm which try to partition the data into k 
distinct groups.

### - Experiment
Step 1 : Data Collection and Preprocessing
- Collect Data
- EDA
- Data Preprocessing
  - Handle Missing Value
  - Outlier

Step 2 : RFM Analysis
- Calculate Recency, Frequency and Monetary Values
- Normalize RFM Values
- Select Features : RFM Attributes and Others

Step 3 : Determine Optimal Clusters and K-Means Clustering 
- Apply Elbow Method : Determine Optimal Number of Cluster
- Choose K-Means Algorithm
- Set Intialization and Iterations

Step 4 : Cluster Profiling and Insights 
- Profile Cluster : Analyze RFM and Additional Features
- Generate Insights for Targeted Strategies

### - Conclusion
Based on the detailed RFM segmentation analysis of **Top Tier Customers**, **Regular Customers** and **Passive Customers**, here's a strategic plan tailored to the business objectives of a retail company (RetailCo). This plan includes both short-term (0-3 months), mid-term (3-6 months) and long-term (6+ months) strategies to maximize customer lifetime value and drive overall revenue growth.

##### 1. **Top Tier Customers**
- Characteristic :
    - Highest frequency of purchases (3.48 times on average).
    - Highest monetary value per transaction (average $59.34).
    - Contributes the most to total revenue (40.70%).
    - Recency of purchases is relatively frequent.
    - Count Customers is 3,121 (17.16% of total customers).
- Short-Term Strategy (0-3 Months) :
    - Implement a VIP rewards program offering exclusive discounts, early access to new products, or personalized offers. This could be targeted at the top 10% of this group to further increase their spend.
    - Send personalized promotions every 3 months tailored to previous purchase patterns, encouraging repeat purchases.
    - Offer free premium services like expedited shipping or personal shopping assistance.
- Mid-Term Strategy (3-6 Months) :
    - Introduce subscription models for frequently purchased items to ensure engagement.
    - Encourage referrals by offering incentives to both the referrer and the new customer, expanding the high-value customer base.
- Long-Term Strategy (6+ Months) :
    - Develop a tiered loyalty program to keep them engaged and reward continued high spending
    - Regularly analyze their purchase patterns to identify early signs of disengagement and address these promptly.

##### 2. **Regular Customers**
- Characteristic :
    - Moderate frequency (1.33) and low monetary value ($17.43) per transaction.
    - Contributes 25.94% to total revenue.
    - Slightly more recent in purchases than the other segments.
    - Count Customers is 6,773 (37.25% of total customers).
- Short-Term Strategy (0-3 Months) :
    - Use email and online prompts to suggest complementary products during checkout to increase transaction value.
    - Create campaigns every 3 months targeting past buyers with special discounts to re-engage them.
- Mid-Term Strategy (3-6 Months) :
    - Offer escalating discounts based on purchase frequency within a set period to encourage more regular buying.
    - Align promotions with seasonal trends or holidays, leveraging broader marketing efforts to pull these customers back.
- Long-Term Strategy (6+ Months) :
    - Solicit feedback regularly to identify ways to enhance their shopping experience and cater to their preferences.
    - Use data to automatically retarget this segment with personalized offers across digital channels to maintain ongoing engagement.

##### 3. **Passive Customers**
- Characteristic :
    - Highest number of customers (8,290).
    - Moderate recency but lower frequency and monetary value per transaction.
    - Significant contributor to revenue (33.36%).
    - Count Customers is 8,290 (45.59% of total customers, largest segment).
- Short-Term Strategy (0-3 Months) :
    - Initiate campaigns with time-sensitive offers, such as "Buy More, Save More" or discounts on frequently purchased items.
    - Offer time-limited discounts (e.g., valid for 30 days) to encourage quicker repeat transactions.
    - Send reactivation offers every 2 months, such as discounts or free shipping on the next purchase, to stimulate purchase frequency.
- Mid-Term Strategy (3-6 Months) :
    - Promote bundles of frequently bought together items at a discounted price to increase basket size and transaction value.
    - Gather feedback to understand what additional needs.
- Long-Term Strategy (6+ Months) :
    - Provide valuable content about products, trends, or exclusive insights to keep them engaged with the brand outside of purchase occasions.
