# Maven Market Sales Analysis

A Power BI project that analyses sales for a retail chain using the Maven Market sample dataset (Maven Analytics). The dashboard tracks sales, quantity, returns and customer groups so that a business user can see how the stores are performing over the year.

## Business Question

- How much is the business selling, and how does it change month to month?
- Which products and brands bring in the most sales?
- Which customer groups (by education, gender and membership card tier) are we selling to?
- How many items are being returned?

## Dataset

- Source: Maven Market sample dataset by Maven Analytics [add link to the dataset page]
- Time period: [add the date range from your Calendar table]
- Tables used:
  - Transactions (two transaction tables combined into one table called All_Transactions)
  - Customers
  - Products
  - Stores
  - Regions
  - Returns
  - Calendar
- Sales is calculated as quantity multiplied by the product retail price (for example, 3 units of a product priced at 2.26 gives a sale of 6.78).

## Tools Used

- Power BI Desktop
- DAX (for the measures)
- Power Query (for cleaning and combining tables)

## Data Model

The model links the transaction table to the customers, products, stores and calendar tables. Regions connect through the stores table, and returns connect through products and stores.

![Data Model](images/data-model.png)

## Dashboard

![Dashboard](images/dashboard.png)

### KPI Cards

- Total Sales: 1.76M
- Total Quantity: 833K
- Total Returns: 8K
- Average Sales per Transaction: 6.54
- Total Transactions: 269,720

### Visuals

- Total Sales by Month (line chart)
- Total Sales by Product Brand (donut chart)
- Total Sales by Product ID (bar chart)
- Customer table by education, gender and membership card tier
- Transaction level table with product, customer and quantity

## Key Insights

- Sales stay in a fairly steady range of about 135K to 150K from January to October.
- Sales rise sharply in November and December, reaching about 177K in December. This is the year end peak.
- October is the lowest month before the jump, so promotions or stock planning before November could matter.
- Average sale per transaction is 6.54, so the business depends on a high number of small baskets and not on a few big orders.
- Customers are grouped into four membership tiers (Normal, Bronze, Silver, Golden). [add one finding here after you add sales by membership tier]

## Limitations and Next Steps

- The product ID bar chart should show product names so it is easier to read.
- The brand donut has too many brands. Showing only the top 10 would be clearer.
- Add sales by region and by store.
- Add total sales by membership card tier to compare customer groups.
- Add slicers for year, region and product category.

## How to Open the Project

1. Download `Maven-Market.pbix` from this repository.
2. Open it in Power BI Desktop.
3. Use the report pages and filters to explore the data.
