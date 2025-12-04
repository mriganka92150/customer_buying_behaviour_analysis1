# 🛍️ Customer Shopping Behavior Analysis

An end-to-end data analytics project that explores customer purchasing patterns, identifies high-value segments, and provides actionable business recommendations using Python, SQL, and Power BI.

## 📋 Project Overview

This project analyzes transactional data from **3,900 purchases** across various product categories to uncover insights into:
- **Spending patterns** by demographic segments
- **Product performance** and customer satisfaction
- **Discount effectiveness** and subscription behavior
- **Customer segmentation** and lifetime value

The analysis aims to guide strategic business decisions in marketing, product development, and customer retention.

## 📊 Dataset Summary

- **Rows:** 3,900 purchases
- **Columns:** 18 features
- **Key Features:**
  - Customer demographics (Age, Gender, Location, Subscription Status)
  - Purchase details (Item Purchased, Category, Purchase Amount, Season, Size, Color)
  - Shopping behavior (Discount Applied, Previous Purchases, Frequency, Review Rating, Shipping Type)
- **Missing Data:** 37 values in Review Rating column (handled via imputation)

## 🛠️ Technologies Used

- **Python** (Pandas, NumPy) – Data cleaning, transformation, and analysis
- **SQL** (PostgreSQL) – Business intelligence queries and data modeling
- **Power BI** – Interactive dashboard and data visualization
- **Git** – Version control and project management

## 📁 Repository Structure

```
customer-shopping-analysis/
│
├── data/
│   ├── raw/                    # Original dataset (not included for privacy)
│   ├── processed/              # Cleaned and transformed data
│   └── sql_outputs/           # Query results and business insights
│
├── sql/
│   ├── database_setup.sql      # PostgreSQL schema and table creation
│   ├── business_queries.sql    # 11 key business questions answered
│   └── insights_summary.sql    # Aggregated insights and metrics
│
├── powerbi/
│   └── shopping_dashboard.pbix  # Interactive Power BI dashboard
│
├── docs/
│   ├── business_summary.pdf    # Executive summary and recommendations
│
├── src/
│   ├── data_cleaning.py        # Data preprocessing functions
│   ├── feature_engineering.py  # Feature creation utilities
│   └── database_connector.py   # PostgreSQL connection handler
│
├── results/
│   ├── visualizations/         # Charts and graphs (PNG)
│   └── recommendations.md     # Detailed business recommendations
│
├── README.md                   # This file
└── requirements.txt            # Python dependencies
```

## 🔍 Analysis Workflow

### 1. **Data Preparation & EDA (Python)**
- Loaded and explored dataset structure using `pandas`
- Handled missing values with median imputation per product category
- Created derived features: `age_group`, `purchase_frequency_days`
- Standardized column names and validated data consistency
- Exported cleaned data to PostgreSQL for SQL analysis

### 2. **Business Intelligence Queries (SQL)**
Performed 11 structured analyses including:
- Revenue breakdown by gender and age groups
- High-value customer identification
- Product performance and discount dependency
- Customer segmentation (New, Returning, Loyal)
- Subscription behavior analysis
- Shipping type impact on purchase amounts

### 3. **Data Visualization (Power BI)**
Built an interactive dashboard featuring:
- Revenue and customer demographic dashboards
- Product performance metrics
- Customer segmentation visualizations
- Discount effectiveness analysis
- Real-time filtering by multiple dimensions

## 📈 Key Insights

### 🎯 Customer Behavior
- **Male customers** generate nearly **2× more revenue** than female customers
- **Young adults (26.66%)** contribute the highest revenue share
- **3,476 loyal customers** drive majority of repeat purchases
- **Non-subscribers** contribute more total revenue despite smaller base

### 📦 Product Performance
- **Top-rated products:** Gloves, Sandals, Boots, Hat, T-shirts
- **Discount-dependent items:** Hat, Sneakers, Coat (47–50% discounted purchases)
- **Category leaders** vary across Accessories, Clothing, Footwear, Outerwear

### 💰 Business Metrics
- **Express shipping users** spend slightly more on average
- **Repeat buyers** generate revenue at higher rates (27.56% vs 22.41%)
- **Middle-aged + Adults** together contribute nearly **50% of total revenue**

## 🎯 Business Recommendations

Based on the analysis, three priority recommendations emerged:

1. **Prioritize Repeat Buyer Retention & Reactivation**
   - Launch loyalty/VIP programs with exclusive benefits
   - Create win-back campaigns for lapsed repeat buyers

2. **Optimize Marketing for Young Adults**
   - Tailor campaigns and product offerings to this high-value segment
   - Leverage social platforms (TikTok, Instagram) for engagement

3. **Develop Targeted Middle-Aged & Adult Strategies**
   - Create segment-specific promotions and family-oriented bundles
   - Implement targeted email marketing and retargeting campaigns

*(Five additional strategic recommendations available in detailed report)*

## 🚀 How to Run This Project

### Prerequisites
- Python 3.8+
- PostgreSQL 12+
- Power BI Desktop (for dashboard viewing)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/customer-shopping-analysis.git
   cd customer-shopping-analysis
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up PostgreSQL database**
   ```bash
   psql -U postgres -f sql/database_setup.sql
   ```

4. **Run the analysis pipeline**
   ```bash
   python src/data_cleaning.py
   python src/feature_engineering.py
   ```

5. **Execute SQL queries**
   - Connect to your PostgreSQL instance
   - Run queries from `sql/business_queries.sql`

6. **Open the Power BI dashboard**
   - Open `powerbi/shopping_dashboard.pbix` in Power BI Desktop
   - Connect to your database instance

## 📚 Skills Demonstrated

- **Data Wrangling:** Handling missing data, feature engineering, data validation
- **SQL Proficiency:** Complex joins, window functions, CTEs, performance optimization
- **Business Intelligence:** Translating data insights into actionable recommendations
- **Data Visualization:** Creating clear, impactful dashboards for stakeholders
- **End-to-End Analytics:** Complete pipeline from raw data to business insights

## 📄 License

This project is for portfolio purposes. Dataset is proprietary and not included in repository.

## 📞 8099173902

Mriganka Jyoti Bordoloi  
[[LinkedIn Profile](https://linkedin.com/in/yourprofile](https://www.linkedin.com/in/mriganka-jyoti-bordoloi-7a6690196/)) • [Email](mriganka92150@gmail.com) 

---

*Built with ❤️ using Python, SQL, and Power BI 
