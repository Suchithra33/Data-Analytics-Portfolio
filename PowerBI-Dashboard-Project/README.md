# 🍽️ Restaurant Business Performance Analysis | Power BI

## 📊 Project Overview

This project presents an interactive **Restaurant Business Performance Dashboard** developed using **Microsoft Power BI**.

The objective of this project is to transform restaurant transaction and customer data into meaningful business insights by analyzing **sales performance, customer behavior, menu performance, order channels, payment methods, branch performance, and customer loyalty**.

The dashboard consists of two interactive pages:

1. **Executive Business Performance Dashboard**
2. **Customer Behavior & Product Performance Dashboard**

The project demonstrates the complete analytics workflow:

**Raw Data → Data Cleaning → Data Transformation → Data Modeling → DAX Calculations → Data Visualization → Business Insights**

---

## 🎯 Business Objectives

The main objectives of this analysis are to:

- Monitor overall restaurant sales performance
- Compare sales across different branches
- Identify the best-selling menu items
- Analyze sales by order channel
- Identify restaurant rush hours
- Understand customer payment preferences
- Analyze customer demographics
- Identify repeat customers
- Measure repeat customer percentage
- Analyze customer loyalty tiers
- Compare vegetarian and non-vegetarian sales
- Identify high-revenue menu items
- Understand sales contribution by menu category

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query**
- **DAX (Data Analysis Expressions)**
- **Data Cleaning & Transformation**
- **Data Modeling**
- **Interactive Data Visualization**
- **Business Intelligence**

---

## 📁 Dataset

The project uses restaurant business data containing information related to:

### Orders
- Order ID
- Order Date
- Time Key
- Branch ID
- Branch Name
- Customer ID
- Channel
- Covers
- Payment Type
- Subtotal
- Discount
- Service Charge
- VAT
- Tip
- Delivery Fee
- Net Sales

### Customer Information
- Customer ID
- Customer demographics
- Gender
- Nationality
- Loyalty Tier
- Vegetarian/Non-Vegetarian preference

### Menu Information
- Menu Item
- Category
- Price
- Vegetarian classification

### Order Items
- Order ID
- Menu Item
- Quantity
- Sales-related information

### Branch Information
- Branch ID
- Branch Name

> **Note:** The original dataset was provided for project/internship purposes. If the dataset is subject to confidentiality or redistribution restrictions, the raw dataset is intentionally not included in this public repository.

---

# 📌 Dashboard 1: Executive Business Performance

The first dashboard provides a high-level overview of restaurant business performance.

### Key Performance Indicators

| KPI | Result |
|---|---:|
| 💰 Total Sales | AED 295.88K |
| 🍽️ Total Quantity | 11K |
| 🧾 Total Orders | 4K |
| 💸 Total Discount | AED 10.20K |
| 👥 Total Customers | 962 |

---

## 📈 Sales Performance by Branch

The dashboard compares sales performance across:

- Jumeirah
- Deira
- Downtown Dubai

The analysis allows users to compare branch-level sales and identify differences in business performance between locations.

---

## 🍽️ Top 5 Best-Selling Menu Items

The dashboard identifies the top-selling menu items based on item sales.

The leading items displayed include:

- Mixed Grill
- Shawarma
- Kunafa
- Hummus
- Fresh Lime

**Mixed Grill** generated approximately **AED 66K** in item sales and was the highest-selling item displayed in the dashboard.

---

## 📦 Sales Distribution by Order Channel

Sales are analyzed across three order channels:

- Dine-In
- Delivery
- Takeaway

The dashboard shows the contribution of each channel to overall sales and helps understand how customers place their restaurant orders.

---

## ⏰ Restaurant Rush Hours

Sales are analyzed across different time periods to identify periods of higher and lower sales activity.

This analysis can help the business understand:

- Peak operating periods
- Lower-demand periods
- Potential staffing requirements
- Customer ordering patterns

---

## 💳 Orders by Payment Method

Orders are analyzed according to:

- Card
- Wallet
- Online
- Cash

This provides visibility into customer payment preferences and the distribution of transactions across payment methods.

---

## 🍴 Items Sold by Category

The dashboard compares item quantities across major menu categories, including:

- Mains
- Beverages
- Desserts
- Salad
- Starters

**Mains** represented the largest item quantity in the displayed analysis.

---

# 📌 Dashboard 2: Customer Behavior & Product Performance

The second dashboard focuses on customer characteristics, loyalty, repeat purchasing behavior, and menu performance.

### Key Performance Indicators

| KPI | Result |
|---|---:|
| 👥 Total Customers | 962 |
| 🔄 Repeat Customers | 307 |
| 📊 Repeat Customer % | 31.91% |
| 🧾 Average Order Value | 82.19 |

---

## 👥 Customer Distribution by Gender

The dashboard analyzes the customer base by gender.

The displayed data contains:

- Female customers: 498
- Male customers: 464

This provides an overview of the customer demographic distribution.

---

## ⭐ Customers by Loyalty Tier

Customers are categorized into loyalty tiers:

- Gold
- Silver
- None

The dashboard shows:

- None: 473 customers
- Silver: 287 customers
- Gold: 202 customers

This analysis helps understand customer participation in the restaurant's loyalty program.

---

## 🌍 Top 5 Customer Nationalities

The dashboard identifies the five most represented customer nationalities:

- Filipino
- Pakistani
- Emirati
- Arab Expat
- Westerner

This provides insight into the diversity of the restaurant's customer base.

---

## 🥗 Vegetarian vs Non-Vegetarian Sales

Sales are compared between:

- Vegetarian
- Non-Vegetarian

The dashboard displays approximately:

- Vegetarian: AED 142K
- Non-Vegetarian: AED 133K

This comparison helps understand the contribution of different customer/menu preferences to overall sales.

---

## 🍰 Sales Contribution by Menu Category

The dashboard uses a **treemap visualization** to show the contribution of different menu categories to sales.

Categories include:

- Mains
- Desserts
- Salad
- Beverages
- Starters

**Mains** contributed the largest share of category sales in the displayed analysis.

---

## 🏆 Top 10 Revenue-Generating Menu Items

The dashboard identifies the menu items generating the highest sales.

The leading items displayed include:

- Mixed Grill
- Chicken Biryani
- Shawarma
- Fattoush Salad
- Falafel Plate
- Kunafa
- Hummus with ...
- Fresh Lime ...

This analysis can help identify high-performing products and support menu and promotional decisions.

---

# 🔄 Data Preparation

The data was prepared using **Power Query** before visualization.

The preparation workflow included:

- Reviewing the structure of the source tables
- Checking data types
- Cleaning and transforming fields
- Preparing date and time information
- Reviewing customer and transaction data
- Creating relationships between tables
- Preparing data for DAX calculations
- Validating the transformed data before dashboard creation

The Power BI data preparation process makes the analysis more **repeatable and refreshable**.


# 🧮 DAX & Calculated Metrics

DAX was used to create analytical measures and KPIs for the dashboard.

Examples of calculated metrics include:

### Total Sales

```DAX
Total Sales = SUM(Orders[NetSalesAED])
Total Orders = DISTINCTCOUNT(Orders[OrderID])
Total Customers = DISTINCTCOUNT(Orders[CustomerID])
Repeat Customer % =
Repeat Customers / Total Customers × 100
Average Order Value =
Total Sales / Total Orders

```
## 📌 Key Performance Indicators

The dashboard provides an overview of restaurant performance through the following KPIs:

- **Total Sales:** AED 295.88K
- **Total Orders:** 4K
- **Total Quantity:** 11K
- **Total Discount:** AED 10.20K
- **Total Customers:** 962
- **Average Order Value:** 82.19
- **Repeat Customers:** 307
- **Repeat Customer %:** 31.91%

---

## 📊 Key Analysis

### 🏪 Branch Performance
Sales performance was analyzed across the restaurant branches, including Jumeirah, Deira, and Downtown Dubai.

### 🍽️ Menu Performance
The dashboard identifies the best-performing menu items and categories based on sales and quantity.

**Mixed Grill** was the highest-selling menu item displayed in the analysis, generating approximately AED 66K in item sales.

### 📦 Order Channel Analysis
Sales were analyzed across:
- Dine-In
- Delivery
- Takeaway

This helps understand customer ordering preferences.

### 💳 Payment Method Analysis
Orders were analyzed by:
- Card
- Wallet
- Online
- Cash

### ⏰ Rush Hour Analysis
Sales and order activity were analyzed across different time periods to identify high-demand operating hours.

### 👥 Customer Analysis
Customer behavior was analyzed based on:
- Gender
- Nationality
- Loyalty Tier
- Repeat Purchase Behavior

### 🔄 Repeat Customer Analysis
The dashboard identified **307 repeat customers**, representing approximately **31.91%** of the total customer base.

### 🥗 Vegetarian vs Non-Vegetarian Sales
The dashboard compares sales generated from vegetarian and non-vegetarian offerings.

### 🏆 Top Revenue-Generating Products
The dashboard highlights the top-performing menu items based on revenue, helping identify products that contribute significantly to restaurant sales.

---

## 🧹 Data Cleaning & Transformation

Power Query was used to prepare the data for analysis.

Key steps included:

- Data type validation
- Handling missing values
- Removing/reviewing duplicate records
- Standardizing data fields
- Transforming columns
- Preparing data for analysis
- Creating relationships between tables

---

## 🧮 DAX Measures

DAX was used to create the required KPIs and analytical measures, including:

- Total Sales
- Total Orders
- Total Customers
- Total Quantity
- Total Discount
- Average Order Value
- Repeat Customers
- Repeat Customer %
- Vegetarian Sales
- Non-Vegetarian Sales

---

## 🎛️ Interactive Dashboard

The dashboard includes interactive slicers and visualizations that allow users to explore restaurant performance dynamically.

Users can filter the analysis based on relevant business dimensions such as:

- Branch
- Order Channel
- Payment Type
- Customer Gender
- Loyalty Tier
- Menu Category
- Vegetarian / Non-Vegetarian

---

## 💡 Key Insights

The analysis provided the following observations:

- Total sales reached approximately **AED 295.88K**.
- The dashboard recorded approximately **4K orders**.
- The restaurant had **962 customers**.
- **307 customers** were identified as repeat customers.
- Repeat customers represented approximately **31.91%** of the customer base.
- **Mixed Grill** was the highest-selling menu item displayed.
- **Mains** represented the largest category by item quantity.
- Sales performance varied across the different restaurant branches.
- Customer orders were distributed across Dine-In, Delivery, and Takeaway channels.
- Payment preferences varied across Card, Wallet, Online, and Cash.

---

## 🎯 Project Outcome

This project helped me develop practical experience in transforming raw business data into an interactive Power BI dashboard.

### Skills Demonstrated

**Power BI | Power Query | DAX | Data Cleaning | Data Modeling | Data Visualization | Business Intelligence | Customer Analytics | Sales Analysis**

---


