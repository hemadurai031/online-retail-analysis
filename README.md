
# Online Retail Sales & Customer Analytics

## 📌 Project Overview

This project analyzes transactional data from a UK-based online retail company to understand *sales performance, customer purchasing behavior, product performance, country-wise sales, and sales trends over time*.

The project follows an end-to-end data analytics workflow using Python, including data cleaning, data transformation, exploratory data analysis, statistical analysis, visualization, and business recommendations.

## 🎯 Business Objectives

The main objectives of this project are:

* To analyze customer purchasing patterns and overall sales performance.
* To identify top-selling products and high-value customers.
* To analyze sales trends across different countries and time periods.
* To generate business insights that can help improve sales and marketing strategies.

## 📊 Dataset

The *Online Retail dataset* contains *541,909 transaction records* from a UK-based online retail company.

The dataset contains the following fields:

* InvoiceNo
* StockCode
* Description
* Quantity
* InvoiceDate
* UnitPrice
* CustomerID
* Country

The dataset covers transactions from *December 2010 to December 2011*.

The dataset contains approximately *25,900 unique invoices/orders*. A single invoice can contain multiple product line items, so the number of transaction rows is much higher than the number of orders.

The raw dataset is not included in this repository because of its file size.

## 🛠️ Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab
* Jupyter Notebook
* GitHub

## 🔄 Project Workflow

text
Data Collection
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Data Transformation
      ↓
Exploratory Data Analysis
      ↓
Descriptive Analysis
      ↓
Diagnostic Analysis
      ↓
Data Visualization
      ↓
Business Insights
      ↓
Prescriptive Recommendations


## 🧹 Data Cleaning

The following data-quality checks and cleaning steps were performed:

* Checked dataset dimensions and structure.
* Checked column data types.
* Checked missing values.
* Checked exact duplicate records.
* Investigated repeated InvoiceNo values.
* Investigated negative Quantity values associated with returns/cancellations.
* Checked invalid or negative UnitPrice values.
* Standardized text fields such as Description and Country.
* Converted InvoiceDate into datetime format.
* Created separate datasets for normal sales and returns/cancellations where required.
* Handled missing CustomerID specifically for customer-level analysis.

Exact duplicate rows were removed after verification.

Missing CustomerID values were not treated as a general sales-data error because those transactions can still be useful for product, country, and time-based analysis. Records without CustomerID are excluded only when performing customer-level analysis.

## 🔄 Data Transformation

The following derived fields were created for analysis:

### Total Sales Amount

text
Total Amount = Quantity × UnitPrice


### Date Features

The InvoiceDate field was used to create:

* Year
* Month
* Month Name
* Year-Month
* Day
* Hour

### Transaction Classification

Transactions were classified to identify:

* Normal sales
* Returns/cancellations

This allows normal sales performance and return activity to be analyzed separately.

## 📈 Descriptive Analysis

The analysis measures key business metrics such as:

* Total sales
* Net sales
* Total quantity sold
* Number of unique orders
* Number of unique customers
* Average order value
* Product-level sales
* Customer-level sales
* Country-level sales
* Monthly sales

## 🔍 Analysis Areas

### 1. Sales Performance

Analyze overall sales performance and order activity.

### 2. Customer Analysis

Identify:

* High-value customers
* Frequent customers
* Customer purchasing patterns
* Revenue contribution by customer

### 3. Product Analysis

Identify:

* Top-selling products by quantity
* Top-performing products by revenue
* Products contributing significantly to overall sales

### 4. Country Analysis

Analyze:

* Revenue by country
* Orders by country
* Countries contributing the highest sales

### 5. Time-Series Analysis

Analyze sales patterns across:

* Months
* Years
* Year-Month periods
* Peak and low sales periods

## 📊 Key Visualizations

The project includes visualizations such as:

* Monthly Sales Trend
* Top 10 Products by Revenue
* Top 10 Products by Quantity
* Top Countries by Revenue
* Top High-Value Customers
* Sales Distribution
* Monthly/Yearly Sales Analysis

## 💡 Business Insights

The final insights are based on the results obtained from the cleaned and transformed dataset.

The analysis aims to answer questions such as:

* Which periods generated the highest sales?
* Which products generated the highest revenue?
* Which products had the highest sales volume?
* Which customers contributed the most revenue?
* Which countries generated the highest sales?
* What purchasing patterns can be observed?

Detailed numerical findings and observations are documented in the project notebook.

## 💼 Prescriptive Recommendations

Based on the analytical findings, potential recommendations include:

* Maintain sufficient inventory for consistently high-demand products.
* Develop targeted retention strategies for high-value customers.
* Plan marketing campaigns around high-performing sales periods.
* Investigate international markets with strong sales performance.
* Review return/cancellation patterns to identify potential product or operational issues.
* Use customer purchasing behavior to support targeted marketing strategies.

The final recommendations are based on the actual findings from the analysis.

## 📁 Project Structure

online-retail-analysis/
│
├── README.md
├── Online_Retail_UK_Transactions_2010_2011.ipynb
├── requirements.txt
├── .gitignore


## 📓 Project Notebook

Online_Retail_UK_Transactions_2010_2011.ipynb

The notebook contains the complete Python-based analysis, including data cleaning, transformation, exploratory analysis, visualization, and business insights.

## 👩‍💻 Author

*Hema Durai*

Aspiring Data Analyst | Python | SQL | Excel | Power BI
