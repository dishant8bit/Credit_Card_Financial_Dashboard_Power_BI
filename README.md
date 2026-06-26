# 📊 Credit Card Financial Dashboard (Power BI + PostgreSQL)

## 📌 Project Overview

This project focuses on developing an interactive **Credit Card Financial Dashboard** using **Power BI** and **PostgreSQL** to analyze customer behavior, transaction performance, revenue trends, and weekly business insights. The dashboard enables stakeholders to monitor key financial metrics, identify customer spending patterns, evaluate card performance, and make informed business decisions through dynamic visualizations and interactive reports.

The project demonstrates end-to-end **Business Intelligence (BI)** development by integrating **SQL**, **PostgreSQL**, **Power BI**, **Power Query**, and **DAX** to build a scalable and automated reporting solution. It is designed to showcase practical data analytics and dashboard development skills for **GitHub portfolios, internships, and entry-level Data Analyst or Business Intelligence roles.**

---

# 🗂 Dataset Description

The project utilizes two relational datasets stored in a PostgreSQL database.

### 1️⃣ Customer Details Table (cust_detail)

Contains customer demographic and account information.

### Key Columns

* Client Number
* Customer Age
* Gender
* Income
* Education Level
* Marital Status
* State
* Dependent Count
* Job Type
* Card Category

---

### 2️⃣ Credit Card Transaction Table (cc_detail)

Contains weekly transaction records and financial information.

### Key Columns

* Client Number
* Transaction Amount
* Transaction Count
* Interest Earned
* Annual Fees
* Activation Status
* Delinquency Status
* Week Start Date
* Card Category

---

# 🛠 Tools & Technologies Used

* Power BI Desktop
* PostgreSQL
* SQL
* Power Query
* DAX (Data Analysis Expressions)
* CSV Dataset

---

# 🗄 Database Creation & SQL Implementation

The raw customer and transaction datasets were initially available in CSV format. To create a structured and scalable data source, the datasets were imported into **PostgreSQL**.

The SQL workflow included:

* Creating relational database tables
* Defining appropriate data types
* Importing CSV files using SQL commands
* Handling date format conversions
* Cleaning inconsistent records
* Managing null values
* Verifying data integrity
* Creating relationships between customer and transaction tables using the Client Number

Using PostgreSQL provided a centralized database that supports efficient querying and seamless integration with Power BI.

---

# 🔗 Connecting PostgreSQL with Power BI

Instead of importing CSV files directly into Power BI, the dashboard connects to the PostgreSQL database.

### Connection Process

1. Created the PostgreSQL database.
2. Imported customer and transaction datasets into SQL tables.
3. Connected Power BI using the PostgreSQL Database connector.
4. Loaded the required database tables into Power BI.
5. Built relationships between tables using the Client Number.
6. Configured data refresh so that any updates made in PostgreSQL are reflected in Power BI after refreshing the report.

This approach enables a dynamic reporting workflow where the dashboard always reflects the latest data stored in the database.

---

# 🧹 Data Cleaning & Transformation

Before visualization, the data was transformed using **Power Query Editor**.

The cleaning process included:

* Removing duplicate records
* Handling missing values
* Correcting data types
* Formatting date fields
* Renaming columns
* Standardizing categorical values
* Removing unnecessary columns
* Preparing data for efficient reporting

Power Query ensured that the data model remained clean, consistent, and optimized for analysis.

---

# 📊 Data Modeling

A relational data model was created inside Power BI.

The model links:

**Customer Table** ⟷ **Transaction Table**

using the **Client Number** as the primary relationship.

This allows customer information and transaction data to interact dynamically across all dashboard visuals.

---

# 📐 DAX Calculations

Several DAX measures and calculated columns were created to generate meaningful business metrics.

### Examples

* Revenue
* Current Week Revenue
* Previous Week Revenue
* Week Number
* Age Group
* Income Group
* Week-over-Week Revenue Growth

These calculations provide dynamic KPIs that automatically update whenever new data is loaded from PostgreSQL.

---

# 📊 Dashboard Features

## 👥 Customer Dashboard

Provides detailed customer analysis through interactive visuals.

### Includes

* Revenue by Gender
* Revenue by Education Level
* Revenue by Occupation
* Revenue by Income Group
* Revenue by Card Category
* Revenue by State
* Customer Age Distribution

---

## 💳 Transaction Dashboard

Analyzes financial performance and transaction activity.

### Includes

* Total Revenue
* Total Interest Earned
* Total Transaction Amount
* Total Transaction Count
* Quarterly Revenue Trend
* Card Category Performance
* Revenue by Expenditure Type
* Revenue by Transaction Method

---

## 📈 Weekly Business Report

A PowerPoint report is included that summarizes weekly business performance and key insights derived from the dashboards.

The report contains:

* Project Objective
* Dashboard Overview
* DAX Calculations
* Week-over-Week Revenue Analysis
* Key Business Insights
* Business Recommendations

---

# 📈 Visualizations Included

* KPI Cards
* Stacked Bar Charts
* Clustered Bar Charts
* Donut Charts
* Pie Charts
* Line Charts
* Weekly Trend Analysis
* State-wise Revenue Map
* Interactive Slicers

---

# 💡 Key Business Insights

* Overall revenue exceeded **57 Million**.
* Total transaction amount reached **46 Million**.
* Interest earned exceeded **8 Million**.
* Male customers generated higher revenue than female customers.
* Blue and Silver card categories contributed approximately **93%** of all transactions.
* Texas, New York, and California generated nearly **68%** of the total revenue.
* Overall activation rate reached **57.5%**.
* Delinquency rate remained at **6.06%**.
* Week 53 recorded a **28.77% increase in revenue** compared to the previous week.

---

# 📸 Dashboard Preview

## Customer Dashboard

(Add Screenshot)

---

## Transaction Dashboard

(Add Screenshot)

---

## Weekly Business Report

(Add PowerPoint Screenshot)

---

# ▶️ How to Use

### Clone the Repository

```bash
git clone https://github.com/dishant8bit/Credit_Card_Financial_Dashboard_Power_BI.git
```

### Open the Power BI Report

Open the `.pbix` file using **Power BI Desktop**.

### Configure PostgreSQL Connection

If required:

* Open **Transform Data**
* Update the PostgreSQL server and database credentials
* Apply changes

### Refresh Data

Click **Refresh** in Power BI to retrieve the latest data from the PostgreSQL database.

Any new records inserted into PostgreSQL will automatically appear in the dashboard after refreshing.

---

# 🚀 Future Improvements

* Publish dashboard to Power BI Service
* Implement scheduled automatic refresh
* Add forecasting models
* Build customer segmentation using RFM analysis
* Integrate real-time transaction data
* Add advanced DAX measures for predictive analytics

---

# 👤 Author

Dishant Kudtarkar

Aspiring Data Analyst | Power BI | SQL | PostgreSQL | Python | Business Intelligence | Data Visualization

---

⭐ If you found this project helpful, consider giving it a **Star** on GitHub!
