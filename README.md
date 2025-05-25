### Product Recommender for Business Customer in B2B

Product Recommender for Customers
Understanding the customer attrition and market demand is crucial for a business. This project explores the machine learning methodologies to process transactioanl records efficiently by focusing on the differences between customers, product families, products across all the regions and purchasing types.

**Author** Divya Pottakkal Divakaran

#### Executive summary

The organization XXX, with a global footprint in a specific range of products, anticipates challenges in achieving its projected revenue targets in the coming years due to increasing competition within the product market segments. To regain and retain business and customers, the organization aims to leverage AI/ML to uncover product associations and relationships, in  identifying opportunities for revenue growth.
Recommended Solution:
The data team put forth the idea of a part recommender logic (ML model) for the customers, by analyzing the sales data to increase sales by implementing it in an ecommerce platform as well as to train the sale representative who accepts customer call. 
The ML model will analyze the organization sale history to trace the high revenue customers, as well as the products purchased together at their different customer sites. These products will be grouped and will be analyzed in detail to trace if any of the products from the grouping are in decline in recent sales. The decline in the product or the product family is an indication that the competitor is already in the take the market share.

#### Rationale
Need to build a part recommender logic(ML model) for the customers to increase sale by implementing it in ecommerce platform as well as to train the sale representative who accepts customer call. 
Detailed description:  XXX company sells various products around the globe. Customers purchases these products for their homes and for offices. XXX company notices there are certain products purchased together by the customer in most of their orders. So XXX company wants to build a part recommender model to implement in their e commerce as well as educate the sale representatives to encourage customers to buy these recommended parts together.
So if one customer purchased product A and B together in past orders, next time any customer adds product A to their shopping cart, product B will be listed at the bottom as recommended product  to buy along with a small discount to increase the sale.


#### Research Question
Analyse the historic transactional data of all the customers and the products they purchase in the last 4 years to build a Product recommender to enhance the business.
The raw data is clustered based on the revenue of the products. The Customer - Product Family is analysed to select the data block with Highest sales order value transactions is selected for the analysis to builkd the product recommender. Aggregated Order Values for Customer/Part Family pairs. 

#### Data Sources
The Data is an encripted data from a Business Organizations. The data is pre-precessing includes data cleaning and data selection process. Data filtered to remove anomalous values and low frequency entries. Negative sale quantities, non integers and negative order values are removed.

#### Methodology
Block Clustering , Moving averges and Change Points are used for Data analysis Rare customers and Products are removed.

#### Results
Data selection process filters 30% of the data which filters the raws with higher order value based on hierarchical block clustering on matrix of aggregated Order Value, where rows represent Customer - and column represent Product Family.

#### Next steps
Next Steps after Data Selection
1. Product Trends Analysis
2. Sales Decline Analysis
3. Customer Similarity Analysis
4. Total purchase Analysis

Sales Decline Analysis + Customer Similarity Analysis + Total Purchase Analysis = > Leads to the Product Recommender.

**Product Trends Analysis **
   a) Products with simlar purchasing trends
   b) Products with declining trends

   Methodoloigies:
   a) K-Shape Clustering 
   b) Shape Based Distance(SBD)

  ** Sales Decline Analysis**
    a) Moving average for Sales declined Detection
Pivoted Data for each customer - > Moving average, Guassian smoothing, Exponential Smoothing - > Slope Calculation for each Smoothed series 

Find Highest Decline (Most negative slope)
Normailize = Change vs historical mean
   
**Customer Similarity Analysis**
a) Customer Sililarity - Chi squared distance
b) Emperical Modeling wiht log Chi Squared Distance

**Total purchase Analysis**
a) Marcov Chain -m Stochastic Process describign the events

#### Outline of project

Here is the code used for initial analysis and fine Tuning the data to select the right cluster of transactions to be used to build the Product recommender system for Customers.

Capstone_EDA.ipynb


##### Contact and Further Information
