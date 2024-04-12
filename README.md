# RFM-analysis

RFM (Recency – Frequency – Monetary) is a part of Marketing Analysis and is used to analyze customer value, thereby helping businesses to segment their customer base. It enables businesses to identify different customer segments and tailor specific marketing campaigns or special care based on their behavior.

Project's context: SuperStore is a global retail company with a large customer base. On the occasion of Christmas and New Year, the Marketing department wants to run marketing campaigns to express gratitude to customers who have supported the company over time and to tap into potential customers to turn them into loyal ones. However, the Marketing department has not yet segmented customers for this year due to the large dataset, which cannot be processed manually as in previous years. Therefore, they are seeking support from the Data Analysis department to deploy a customer segmentation task to classify each customer segment and tailor marketing programs accordingly. The Marketing Director has also proposed using the RFM model. However, in the past, when the company was smaller, the team could calculate and classify using Excel. With the current large volume of data, they hope the Data department can build a deployment pipeline for segmentation evaluation through Python programming.

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
