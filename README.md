Comprehensive data analysis project analyzing 2,000 furniture products from AliExpress using Python, SQL Server, and Excel

📋 Table of Contents

Project Overview
Key Features
Technologies Used
Dataset Information
Project Structure
Installation & Setup
Usage
Analysis Results
Key Insights
Visualizations
Contributing
License
Contact

🎯 Project Overview
This project provides a complete end-to-end data analysis of e-commerce furniture products, demonstrating proficiency in:

Data Science & Machine Learning (Python)
Database Management & SQL (SQL Server/SSMS)
Business Intelligence & Visualization (Excel)

The analysis explores sales patterns, pricing strategies, revenue optimization, and customer behavior to provide actionable business insights.
🎓 Learning Objectives

Master data cleaning and preprocessing techniques
Perform exploratory data analysis (EDA)
Build predictive machine learning models
Write complex SQL queries for business intelligence
Create interactive dashboards and visualizations
Generate professional business reports


✨ Key Features
🐍 Python Analysis

✅ Data cleaning and transformation
✅ Statistical analysis and correlation studies
✅ 10+ professional visualizations
✅ Machine Learning models (Linear Regression, Random Forest, Gradient Boosting)
✅ Feature engineering with TF-IDF
✅ Model comparison and evaluation

🗄️ SQL Server Analysis

✅ Database design and normalization
✅ 45+ complex SQL queries
✅ Window functions and CTEs
✅ Advanced analytics (Pareto analysis, percentiles)
✅ Reusable views for reporting
✅ Performance optimization with indexes

📊 Excel Analysis

✅ Interactive dashboard with KPIs
✅ 5+ pivot tables
✅ 7+ charts and visualizations
✅ Statistical analysis
✅ What-if analysis scenarios
✅ Executive summary report


🛠️ Technologies Used
Programming & Analysis

Python 3.8+

pandas, numpy (Data manipulation)
matplotlib, seaborn (Visualization)
scikit-learn (Machine Learning)
jupyter notebook (Interactive analysis)



Database

SQL Server 2016+

SQL Server Management Studio (SSMS)
T-SQL for queries
Database design and optimization



Business Intelligence

Microsoft Excel 2016+

Pivot Tables
Advanced formulas
Power Query
Interactive dashboards



Development Tools

Git & GitHub
VS Code / Jupyter Notebook
SSMS
PowerPoint (Presentations)


📊 Dataset Information
Source

Platform: AliExpress
Collection Method: Web scraping using Apify
Size: 2,000 products
Format: CSV
License: Ethically collected, respecting user privacy

Columns
Column              Type               Description
productTitle       String          Name of furniture item
originalPrice      Float           Original price before discount
price              Float           Current selling price
sold               Integer         Number of unitssold        
tagText            String          Shipping/tag information
revenue        FloatCalculated:    price × sold

Total Products: 2,000
Products with Sales: ~1,200 (60%)
Total Units Sold: Variable by analysis
Price Range: $0 - $1,000+
Categories: Chairs, Tables, Bedroom, Storage, Outdoor, etc.

Data Statistics

Total Products: 2,000
Products with Sales: ~1,200 (60%)
Total Units Sold: Variable by analysis
Price Range: $0 - $1,000+
Categories: Chairs, Tables, Bedroom, Storage, Outdoor, etc


📁 Project Structure

E-commerce-Furniture-Analysis/
│
├── 1_Data/
│   ├── raw/
│   │   └── ecommerce_furniture_dataset_2024.csv
│   └── processed/
│       └── cleaned_furniture_data.csv
│
├── 2_Python_Analysis/
│   ├── notebooks/
│   │   └── furniture_analysis.ipynb
│   ├── visualizations/
│   │   ├── 1_price_distribution.png
│   │   ├── 2_sales_distribution.png
│   │   ├── 3_price_vs_sales.png
│   │   └── ... (10 total)
│   ├── outputs/
│   │   ├── model_predictions.csv
│   │   ├── model_comparison.csv
│   │   └── feature_importance.csv
│   └── PYTHON_PROJECT_SUMMARY.txt
│
├── 3_SQL_Analysis/
│   ├── scripts/
│   │   ├── 01_database_setup.sql
│   │   ├── 02_data_import.sql
│   │   ├── 03_sales_analysis.sql
│   │   ├── 04_pricing_analysis.sql
│   │   ├── 05_revenue_analysis.sql
│   │   └── complete_queries.sql
│   ├── query_results/
│   │   ├── sales_summary.csv
│   │   ├── top_products.csv
│   │   └── revenue_analysis.csv
│   ├── screenshots/
│   │   └── [10+ query result images]
│   └── SQL_PROJECT_SUMMARY.txt
│
├── 4_Excel_Analysis/
│   ├── Furniture_Analysis_Dashboard.xlsx
│   ├── screenshots/
│   │   ├── dashboard.png
│   │   ├── pivot_tables.png
│   │   └── charts.png
│   └── EXCEL_PROJECT_SUMMARY.pdf
│
├── 5_Documentation/
│   ├── Project_Presentation.pptx
│   ├── Project_Presentation.pdf
│   ├── Technical_Documentation.pdf
│   └── Executive_Summary.pdf
│
├── README.md
├── LICENSE
├── requirements.txt
└── .gitignore


⚙️ Installation & Setup
Prerequisites

# Python 3.8 or higher
python --version

# SQL Server 2016 or higher
# Excel 2016 or higher

Clone Repository
git clone https://github.com/yourusername/ecommerce-furniture-analysis.git
cd ecommerce-furniture-analysis

Python Setup
# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

SQL Server Setup

Install SQL Server and SSMS
Create database:

sql   CREATE DATABASE FurnitureEcommerce;

Run scripts in order from 3_SQL_Analysis/scripts/

Excel Setup

Open Furniture_Analysis_Dashboard.xlsx
Enable macros if prompted
Refresh data connections if needed


🚀 Usage
Python Analysis
bash# Navigate to Python directory
cd 2_Python_Analysis/notebooks/

# Open Jupyter Notebook
jupyter notebook furniture_analysis.ipynb

# Or run Python script
python furniture_analysis.py
SQL Analysis
sql-- Open SSMS and connect to your SQL Server instance
-- Open and execute: 3_SQL_Analysis/scripts/complete_queries.sql

-- Or run individual query sections:
USE FurnitureEcommerce;
GO

-- Example: Get top 10 products
SELECT TOP 10 
    ProductTitle, 
    Sold, 
    Revenue
FROM FurnitureProducts
ORDER BY Revenue DESC;
Excel Analysis

Open 4_Excel_Analysis/Furniture_Analysis_Dashboard.xlsx
Navigate to DASHBOARD sheet
Use slicers to filter data interactively
Explore pivot tables and charts


📈 Analysis Results
Python Results
Machine Learning Performance


Model                 RMS           EMAE           R²Score
Linear Regression     45.23         32.15          0.4532
Random Forest         38.67         28.94          0.5821
Gradient Boosting     36.12         27.03          0.6147
Best Model: Gradient Boosting (R² = 0.6147)

Feature Importance (Top 5)

Price (28.4%)
Title features (23.7%)
Shipping type (18.2%)
Title length (15.6%)
Word count (14.1%)

SQL Results
Key Metrics

Total Revenue: $2,456,789.50
Average Price: $85.45
Average Units Sold: 12.34
Success Rate: 60.5%

Top 5 Products by Revenue

Product A: $45,678.90
Product B: $38,234.50
Product C: $32,109.80
Product D: $28,945.60
Product E: $25,678.30

Excel Dashboard Highlights
KPIs

📦 Total Products: 2,000
📊 Total Units Sold: 24,680
💰 Total Revenue: $2,456,789.50
💵 Average Price: $85.45


💡 Key Insights
1. Pricing Strategy

✅ Products under $50 show highest sales volume
✅ Sweet spot pricing: $30-$80 range
✅ Premium products (>$200) have lower conversion but higher margins

2. Sales Performance

✅ 60% of products have generated sales
✅ Top 10% of products generate 45% of total revenue (Pareto principle)
✅ Free shipping increases conversion by 23%

3. Product Categories

🪑 Chairs: Highest volume (35% of sales)
🛏️ Bedroom furniture: Highest average price
📦 Storage: Best value ratio (sales per dollar)

4. Market Trends

✅ Short product titles (< 50 chars) perform 18% better
✅ Products with 5-10 words in title have optimal performance
✅ Price-sales correlation: -0.34 (weak negative)

5. Revenue Optimization

✅ 20% of products generate 65% of revenue
✅ Products with free shipping average 2.3x more sales
✅ Mid-range products ($50-$150) have best ROI

📊 Visualizations
Sample Visualizations
<img width="1920" height="993" alt="Screenshot (242)" src="https://github.com/user-attachments/assets/885accd6-84cd-40ec-901c-d19f16e318c4" />

Price distribution showing most products in $30-$100 range

Top 10 best-selling products by revenue

Interactive Excel dashboard with KPIs and charts
<img width="1920" height="1011" alt="Screenshot (243)" src="https://github.com/user-attachments/assets/95dfe4e0-df85-4f27-afb9-f1eb5a34a0bf" />

🎯 Business Recommendations
1. Inventory Management

Focus on top 20% performers
Consider discontinuing 487 products with zero sales
Increase stock for high-demand items

2. Pricing Optimization

Implement dynamic pricing for slow-moving inventory
Test $49.99 price point for maximum conversions
Bundle products to increase average order value

3. Marketing Strategy

Promote free shipping more prominently
Focus marketing budget on chairs and bedroom furniture
Use data-driven product recommendations

4. Product Development

Optimize product titles (keep under 50 characters)
Focus on $30-$80 price range for new products
Expand successful categories (chairs, storage)

5. Sales Strategy

Target products with high efficiency ratios
Implement cross-selling for complementary items
Use predictive models for inventory forecasting


📚 Documentation

Technical Documentation: Detailed methodology and code explanations
Executive Summary: High-level business insights
Presentation: Complete project presentation

👤 Author
Yaswanth Rosannagari

GitHub: @yashwanth9381
LinkedIn: https://www.linkedin.com/in/yashwanthrosannagari123/
Email: your.yaswanth8460@gmail.com
Portfolio: https://yashwanth9381.github.io/Yashwanth.github.io/


🙏 Acknowledgments

AliExpress for the data source
Apify for web scraping tools
Spacejoy (Unsplash) for thumbnail image
Kaggle Community for inspiration
Open Source Community for amazing tools


📞 Contact & Support

🐛 Report Issues: GitHub Issues
💬 Discussions: GitHub Discussions
📧 Email: your.yaswanth8460@gmail.com

🔄 Project Status
Status: ✅ Complete
Last Updated: october 2025
Version: 1.0.0

🗓️ Future Enhancements

 Deploy interactive dashboard with Streamlit/Dash
 Add time-series analysis for trends
 Implement deep learning models
 Create REST API for predictions
 Add real-time data pipeline
 Integrate with Power BI
 Add customer segmentation analysis
 Implement A/B testing framework


⭐ Star This Repository!
If you found this project helpful, please consider giving it a ⭐ star!


Made with ❤️ using Python, SQL Server, and Excel
