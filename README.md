# Unilever_data_SCM_Analysis

This projecy analyze a supply chain dataset inspired by Unilever operations to evaluate Product performance, Inventory efficiency, Supplier and logistics performance, Quality issues, and Supply chain risks. The goal is to generate business insights that improve operational efficiency and decision-making. The initial dataset was deemed insufficient due to its small size (100 rows) and the absence of timestamp data. To resolve this, I utilized generative AI to augment the record count and synthesize datetime attributes, ensuring the dataset was robust enough for meaningful insight extraction.

* from 100 rows to 3,000 rows total + new Date column
* Date range covering all 24 months from 2023-01-01 to 2024-12-31
* Date display format: YYYY-MM-DD

**The analysis combines:**
* Python → data cleaning, feature engineering, and analysis
* Tableau → interactive dashboard visualization
  
## Dataset Description 
The dataset contains supply chain-related variables, including:

* Product type, SKU
* Price, Availability
* Number of products sold
* Revenue generated
* Stock levels
* Lead times (supplier & manufacturing)
* Order quantities
* Shipping times and carriers
* Manufacturing and shipping costs
* Supplier name
* Production volumes
* Inspection results
* Defect rates
* Transportation modes and routes

## Derived Variables 

Several new variables were created to better measures supply chain performance. 

* Inventory Turnover: Sales relative to stock levels (inventory efficiency)
* Revenue per Unit Sold: Average revenue per product
* Profit:	Revenue − Costs
* Profit Margin:	Profit relative to revenue
* Sales to Production Ratio:	Production efficiency
* Stock Risk:	Indicates if stock is insufficient for demand

## Tools Used 

Python, Pandas, Numpy, Matplotlib, Tableau for visualization 

## Analysis 

### 1. Product Analysis 

High-revenue products are key drivers of profitability. 

### 2. Inventory Analysis 

1,601 products are at stock risk, while 1,399 are safe, incidating imbalance between inventory and demand 

### 3. Supplier performance 

Supplier variability affects supply chain efficiency 

### 4. Logistics Analysis 

Some carriers perform significantly better in delivery time. 

### 5. Quality Analysis 

* Haircare products have the highest defect rates
* Most defect rates fall between 1.5–3.5
* High defect rates (>4) are less frequent
* Quality improvement needed in haircare production

### 6. Correlation Analysis 

A correlation heatmap was used to examine relationships between variables.

* Revenue strongly correlates with profit
* Costs negatively impact profit margin
* Inventory turnover is negatively related to stock levels
* Operational variables (lead time, defect rates) show weaker direct relationships

## Recommendations 

**Inventory Management**
* Improve demand forecasting
* Adjust reorder points
* Maintain safety stock for high-demand products

**Supplier Management**
* Monitor supplier lead times
* Prioritize reliable suppliers

**Quality Management**
* Strengthen inspection processes
* Focus on high-defect product categories

**Cost Control**
* Reduce manufacturing and shipping costs
* Improve operational efficiency

## Tableau Dashboard Images

<img width="1903" height="1032" alt="Unilever_dashboard_1" src="https://github.com/user-attachments/assets/fff71006-e9ae-49f5-ac36-fea2b3a77928" />

<img width="1904" height="1040" alt="Unilever_dashboard_2" src="https://github.com/user-attachments/assets/6718570c-5b20-4fd8-9315-ead2ae55c2e7" />

<img width="1904" height="1027" alt="Unilever_dashboard_3" src="https://github.com/user-attachments/assets/0827c236-f7e3-4af6-8043-72463583e530" />

<img width="1898" height="1036" alt="Unilever_dashboard_4" src="https://github.com/user-attachments/assets/13ac3f1a-e77f-40c4-92af-5b64aa7b92b4" />


