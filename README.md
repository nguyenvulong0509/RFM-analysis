# RFM-analysis

RFM (Recency – Frequency – Monetary) is a part of Marketing Analysis and is used to analyze customer value, thereby helping businesses to segment their customer base. It enables businesses to identify different customer segments and tailor specific marketing campaigns or special care based on their behavior.

Project's context: SuperStore is a global retail company with a large customer base. On the occasion of Christmas and New Year, the Marketing department wants to run marketing campaigns to express gratitude to customers who have supported the company over time and to tap into potential customers to turn them into loyal ones. However, the Marketing department has not yet segmented customers for this year due to the large dataset, which cannot be processed manually as in previous years. Therefore, they are seeking support from the Data Analysis department to deploy a customer segmentation task to classify each customer segment and tailor marketing programs accordingly. The Marketing Director has also proposed using the RFM model. However, in the past, when the company was smaller, the team could calculate and classify using Excel. With the current large volume of data, they hope the Data department can build a deployment pipeline for segmentation evaluation through Python programming.

### Business questions
- The Marketing Department needs to classify the segments of each customer to deploy each marketing program suitable for each customer group.
- The Marketing Director also proposed a plan to use the RFM model in Python to segment customers, and then launch marketing campaigns to thank customers for supporting the company over the past time. As well as exploit potential customers to become loyal customers.
- Suggestions to the Marketing and Sales team with the company's retail model, which of the three indicators R, F, and M should be most interested in?

### About dataset
This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.
- **InvoiceNo**:  Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'C', it indicates a cancellation.
- **StockCode**: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
- **Description**: Product (item) name. Nominal.
- **Quantity**: The quantities of each product (item) per transaction. Numeric.
- **InvoiceDate**: Invoice Date and time. Numeric, the day and time when each transaction was generated.
- **UnitPrice**: Unit price. Numeric, Product price per unit in sterling.
- **CustomerID**: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
- **Country**: Country name. Nominal, the name of the country where each customer resides.

### Project's details
For more details about data processing and wrangling, please see the jupyter notebook attached in this repository. For now, I will demonstrate the data visualisations, insights and recommendations.

   - ![image](https://github.com/nguyenvulong0509/RFM-analysis/assets/116187817/bfd28ab4-335d-4d7c-b711-5a1ce2738799)
   - ![image](https://github.com/nguyenvulong0509/RFM-analysis/assets/116187817/74569566-2780-4b64-8d5f-6b7c8b2b3051)
   - ![image](https://github.com/nguyenvulong0509/RFM-analysis/assets/116187817/86276208-4245-4bc5-8412-9748c3c94551)
   
- Recency distribution is right-skewed, showing that the majority of customers made a purchase in the recent past. It has a long tail containing single customers who made their order long time ago. Similar pattern also appears on Frequency and Monetary distribution plots. The plots show that most customers has low frequency (small number of orders, around 10 per customer) and spend little amount of money in each transaction > Although the information is quite general (since we're using distribution plot and there might be other factors affecting the results), we've gained some insights of how customers are experiencing our services > find out the reasons why the RFM indicators are this low.

   - ![image](https://github.com/nguyenvulong0509/RFM-analysis/assets/116187817/0e7d99cc-6284-4240-84bb-0b504c6e2e70)
- Analysis of clusters based on set of rules applied to RFM scores is much more diverse. Take a closer look at the count plot above, it's good to see that 'loyal customers' and 'potential loyalists' constitute around 1/6 of all customers. What is more, there is a large group of 'champions' who are the most profitable customers. At the same time it should worry that group of 'hibernating' is so big - about 700 customers of all customers. There is an opportunity that part of this group could be reactivated with a reach out campaign. Moreover, the company should focus on the group 'at risk' and 'lost customers' to increase customer retention (for lost customers, the company can choose to ignore them if needed).

   - ![image](https://github.com/nguyenvulong0509/RFM-analysis/assets/116187817/fd7db3b3-1874-4b0d-8b4c-62c3d6c4eb7e)
Based on the previous analysis of count plot, there are six group of customers that the company need to prioritise:

- Champions
- Loyal
- Potential loyalist
- At risk
- Hibernating customers
- Lost customers
- With the treemap above, here are some recommendation for each cluster:

The champions and loyal clusters bring the majority of sales to the company (74.35% in sum). This means that they are quite satisfied with the services (to some degrees). For those groups, the company can reward them and give them early access of new products. It's also a good strategy to engage the customers by asking for reviews so that they can be brand promoters.
Despite the large number of customers, potential loyalist only spent a little amount of money (contribute 2.53% sales to company). For this group, it is necessary to Offer membership / loyalty program and Upsell higher value products.
At risk group has the same number of customer as loyal group. This type of group is known as spending big money and purchasing often long time ago (recency problems). Therefore, it is important to send them personalized emails to reconnect, offer renewals and offer special deals with the hope of bringing them back.
The last two types is hibernating and lost customers. For hibernating, the company can reactivate them by offering other relevant products and special discounts and recreating brand value. Try all the best to prevent this group from converting into lost customers group. With lost customers, it is worth trying to revive interest with reach out campaign or reach out for feedbacks (this is important to improve services). Otherwise, the company can ignore them if needed.



 

