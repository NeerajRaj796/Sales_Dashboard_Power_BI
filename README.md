🛍️ Power BI Online Retail Dashboard – Stakeholder Case Study
Executive Summary

This project presents a comprehensive analysis of two years of online retail transactional data, relabelled as 2022–2023 and 2023–2024 to reflect current market scenarios. The analysis was conducted using Power BI to evaluate revenue growth, product performance, customer behaviour, and regional sales contribution.

The objective was not simply to build a dashboard, but to transform raw transactional records into strategic business insights that can inform revenue planning, product strategy, and geographic expansion decisions.

Across the two financial years, the business generated £29.04 million in total sales, supported by 16 million units sold and over 5,900 unique customers. The analysis revealed a 104% year-on-year revenue increase, indicating strong commercial momentum and market expansion.

Business Context

The retail company aims to understand what drove its rapid growth between the two years. Specifically, leadership wants clarity on whether growth is driven by higher customer acquisition, increased basket value, improved product mix, or regional expansion. Additionally, there is interest in identifying potential concentration risks — either in product dependency or geographic reliance.

The dataset used for this project originates from the Online Retail II dataset (UCI Machine Learning Repository), originally covering 2009–2011. To align findings with present-day retail contexts, the years were relabelled as 2022–2024 while preserving the dataset’s structural integrity.

Data Preparation and Modelling

The dataset consists of invoice-level transaction records, including product descriptions, quantities, unit prices, customer IDs, invoice dates, and country information.

Data cleaning involved removing duplicate transactions, handling missing customer identifiers, validating quantity and pricing consistency, and structuring the invoice date into a proper time hierarchy (Year, Quarter, Month).

A Star Schema data model was designed to ensure scalable and accurate reporting. The central Fact_Transactions table was connected to dimension tables for Date, Product, Country, and Customer. This structure enabled dynamic year-on-year comparisons and multidimensional analysis across time, geography, and product categories.

Key business metrics were calculated using DAX measures, including Total Sales, Sales Growth (£ and %), Average Order Value (AOV), Average Selling Price (ASP), and Units Sold. These measures formed the foundation for variance analysis and performance tracking.

Revenue Performance Analysis

The company recorded £9.5 million in sales during 2022–2023, which increased significantly to £19.5 million in 2023–2024, representing a 104% year-on-year growth rate. This doubling of revenue within one year suggests accelerated market demand and improved commercial performance.

Quarterly analysis revealed particularly strong performance in Q4, where revenue in 2023–2024 nearly doubled compared to the previous year. This indicates strong seasonal demand patterns, likely influenced by holiday-driven retail behaviour.

The substantial £220K+ growth contribution highlights that expansion was not incremental but structurally significant.

Product Performance and Revenue Concentration

The analysis identified over 5,100 distinct products, with revenue heavily concentrated among the top-performing SKUs. Specifically, the top five products contributed approximately 40% of total revenue, indicating a high degree of sales concentration.

This concentration presents both an opportunity and a risk. On one hand, high-performing products demonstrate strong brand alignment and demand consistency. On the other hand, over-reliance on a small subset of SKUs exposes the business to product lifecycle volatility and competitive pressures.

Product-level growth analysis showed that some SKUs experienced exponential year-on-year growth, while certain long-established products declined significantly. This pattern suggests evolving customer preferences and potential product lifecycle transitions.

Pricing and Customer Basket Behaviour

The analysis revealed an Average Selling Price (ASP) of £1.84 and an Average Order Value (AOV) of £541.42. While the individual unit price remains relatively low, the high AOV suggests that customers purchase multiple items per transaction.

This indicates that growth is primarily driven by increased basket size rather than premium pricing. The rising AOV between the two years suggests successful upselling, bundling strategies, or increased repeat purchase behaviour.

Customer analysis across 5,900+ unique customers indicates that repeat customers contribute disproportionately to revenue, demonstrating the importance of retention and loyalty initiatives.

Regional Sales Distribution

Geographic analysis identified Switzerland, Spain, and Sweden as the leading revenue-generating regions, contributing more than 80% of total sales volume. Switzerland in particular represents a significant portion of total units sold, indicating strong market penetration.

Emerging markets such as Singapore and Thailand, while smaller in contribution, show measurable growth potential. However, the heavy reliance on a limited number of markets introduces geographic concentration risk.

Strategically, this suggests the need for regional diversification while maintaining strong engagement in dominant markets.

Seasonal and Temporal Trends

Monthly and quarterly analysis revealed clear seasonal patterns. Revenue consistently peaks during Q4, aligning with typical global retail demand cycles.

The most significant year-on-year increases occurred during the final quarter, indicating that promotional strategies or seasonal purchasing behaviour strongly influence annual performance.

This insight supports targeted marketing investment in pre-Q4 periods to maximize conversion during peak seasons.

Dashboard Structure

The Power BI dashboard is structured into three interactive pages:

1. Summary Page

![Summary Page](Summary-Page.png)


Provides an executive-level overview of KPIs, quarterly trends, top-performing countries, and product mix visualization.

2. Sales Analytics Page

![Sales Analytics Page](Sales-Analytics-Page.png)


Focuses on year-on-year comparisons, monthly trends, and regional contribution analysis, including variance breakdowns.

3 Product Analysis Page

![Product Analysis Page](Product-Analysis-Page.png)


Explores SKU-level growth contribution, product performance trends, and country-level distribution.

Each page includes dynamic slicers and navigation buttons, allowing stakeholders to filter by year, country, product, and customer for deeper insight exploration.

Strategic Recommendations

Based on the analysis, several strategic actions are recommended:

Diversify revenue streams to reduce dependency on top-performing SKUs.

Strengthen investment in high-growth emerging markets while reducing geographic concentration risk.

Optimize Q4 promotional strategies to capitalize on seasonal peaks.

Expand bundling and loyalty programs to sustain rising AOV.

Monitor declining SKUs and adjust product lifecycle management accordingly.

Conclusion

This analysis demonstrates how structured data modelling and business intelligence tools can transform raw retail transactions into strategic insights.

The dashboard quantifies a 104% year-on-year revenue increase, identifies product concentration risks, highlights geographic dependency, and reveals customer basket expansion trends.

By integrating revenue, product, customer, and regional insights into a single interactive platform, this project provides a data-driven foundation for informed decision-making and long-term retail growth strategy.
