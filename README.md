**📊 Customer Segmentation using RFM Analysis**

**🔍 Overview**

This project implements an end-to-end customer segmentation framework using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering to understand customer purchasing behavior and drive data-informed marketing strategies. The goal is to identify high-value, loyal, and at-risk customer segments from large-scale transactional data.

**🎯 Business Problem**

Businesses often struggle to identify which customers contribute the most to revenue and how to tailor marketing strategies accordingly. Without segmentation, retention efforts, promotions, and resource allocation are inefficient and unfocused.

**This project addresses:**

Who are the most valuable customers?

Which customers are at risk of churn?

How can marketing strategies be customized by customer segment?

**🧾 Dataset Overview**

Transactions: ~400,000 retail transactions

Customers: 4,339 unique customers

Time Period: December 2010 – December 2011

Key Fields: Invoice Date, Quantity, Unit Price, Customer ID, Revenue

**🛠️ Methodology**

**1️⃣ Data Preprocessing**

Converted invoice timestamps to datetime format

Removed missing customer records and handled returns

Created revenue (TotalPrice) and time-based features

**2️⃣ RFM Feature Engineering**

Recency: Days since last purchase

Frequency: Number of unique purchases

Monetary: Total revenue per customer

Customers were scored using quartiles to create RFM profiles.

**3️⃣ Customer Segmentation**

Standardized RFM features using StandardScaler

Applied K-Means clustering

Selected optimal number of clusters using silhouette score

**4️⃣ Segment Profiling & Insights**

Identified a VIP segment (<1% of customers) contributing ~25% of total revenue

Profiled segments based on spending, engagement, and recency

Quantified revenue contribution and customer distribution per segment

**📈 Key Insights**

A very small group of high-frequency, high-spend customers drives a disproportionate share of revenue

Majority of customers fall into low-to-mid value segments with growth potential

Clear opportunities exist for targeted retention, upsell, and win-back campaigns

**💡 Marketing Recommendations**

VIP Customers: Loyalty programs, premium offers, early access

Loyal Customers: Cross-sell and bundle strategies to increase AOV

At-Risk Customers: Personalized win-back campaigns

New / Low-Value Customers: Onboarding offers and engagement nudges

**🧰 Tech Stack**

**Programming**: Python

**Libraries:** Pandas, NumPy, scikit-learn, Matplotlib, Seaborn

**Techniques:** RFM Analysis, K-Means Clustering, Silhouette Analysis

**🚀 Outcome**

This project demonstrates how customer segmentation can directly support marketing strategy, revenue optimization, and customer lifetime value improvement using a scalable analytics approach.
