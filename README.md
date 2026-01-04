## 👤 Author

**[Soumyadeep Das]**  
Computer Science & Technology (AI-ML Specialization)  
Power BI | Data Analytics | Machine Learning
Computer Science & Technology (AI-ML Specialization)  
[JIS UNIVERSITY], India  
GitHub: https://github.com/Soumyadeep1012

# E-commerce-Sales-Dashboard-using-Power-BI---Regional-and-Category-Insights
📌 **Project Overview**

This project presents an interactive Power BI dashboard built on a real-world e-commerce dataset to analyze sales performance, order behavior, product categories, and regional trends.

The goal of the project is not just visualization, but to demonstrate end-to-end analytical thinking — from raw data cleaning and modeling to KPI design and storytelling.

The dashboard is structured into multiple analytical pages (Overview, Product Analysis, Regional Analysis) to support decision-making at different levels.

🗂 **Dataset Description**

Source: Olist E-commerce Dataset (Brazil)
Platform: Kaggle

The dataset represents a large-scale online marketplace with multiple relational tables, including:

Orders

Order items

Products

Customers

Payments

Geolocation

Category translations

🌍 **Why a Brazilian Dataset?**

The Olist dataset represents a real-world, production-scale e-commerce platform with complex relational data.
Its structure closely resembles that of global e-commerce companies, making it ideal for practicing industry-level BI, data modeling, and analytics skills, independent of geography.

The analytical techniques used here are globally transferable.

🔧 **Tools & Technologies Used**

Power BI Desktop (Free Version)

Power Query – data cleaning & transformation

DAX – KPI and measure creation

Star-schema-friendly data modeling

Geographical visualizations

🧠 **Data Cleaning & Transformation (Power Query)**

I performed extensive data preparation using Power Query before any visualization or modeling:

Column pruning to remove unused or redundant fields

Data type validation (dates, numeric measures, categorical fields)

Feature creation (Year, Month, Month Name)

Lookup table merging for readable product category names

Standardization of fact and dimension tables

⚠️ **Customer Modeling Decision**

In the Olist dataset, customer_id does not behave as a stable unique key for dimensional modeling.

To avoid:

Incorrect one-to-many assumptions

Aggregation errors

Ambiguous relationships

I modeled Orders as the primary analytical dimension, and used customer attributes contextually rather than forcing a traditional Customers dimension relationship.

This ensured correct aggregations, cleaner relationships, and reliable KPIs.

📐 **Star-Schema-Friendly Design**

Fact table: Order Items (sales-level granularity)

Dimensions: Orders, Products, Categories, Geography

Relationships were validated to avoid duplicate keys on the “one” side

This structured model can later be reused for:

Sales forecasting

Customer segmentation

Recommendation systems (ML use cases)

📈 **Key KPIs & DAX Measures**

The following KPIs were created using DAX:

Total Sales

Total Orders

Average Order Value (AOV)

Total Products Sold

📊 **Dashboard Structure & Pages**

📄 Page 1: Executive Overview

KPI Cards (Sales, Orders, AOV, Products Sold)

Sales trend over time (Year–Month)

Year and Month slicers

📄 Page 2: Product Analysis

Sales by product category

Category-level comparisons

Focused product insights

📄 Page 3: Regional Analysis

Sales by state (map visual)

State-wise sales comparison

Regional performance insights

🕒 **Time Intelligence Design**

Instead of using raw timestamps, I derived Year and Month during Power Query.

**Why?**

Improves readability

Simplifies slicers

Enhances performance

Avoids unnecessary timestamp complexity


🗺 **Map Visuals & Privacy Settings**

Power BI disables map visuals by default due to privacy controls.

“I explicitly enabled map visuals through Global Security settings to support geographical sales analysis.”

This allowed meaningful regional insights without compromising dashboard performance.

📂 **Measures Organization**

Why no separate Measures table?

For clarity and simplicity:

Measures were grouped under their relevant fact tables

The focus remained on correct modeling and dynamic aggregation, rather than table organization aesthetics

📁 **Repository Structure**

📁 E-Commerce-Sales-Dashboard-PowerBI

│

├── Ecommerce_Sales_Dashboard.pdf

├── README.md

└── screenshots/
    
    ├── dashboard_overview.png
   
    ├── product_analysis.png
    
    └── regional_sales_map.png

🚀 **Future Scope (AI / ML)**

The cleaned dataset and structured data model can be extended for:

Sales forecasting

Customer segmentation

Product recommendation systems

Time-series demand prediction

This makes the project highly relevant for AI-ML and Data roles.
