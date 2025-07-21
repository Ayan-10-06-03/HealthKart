# HealthKart Influencer Campaign Dashboard

## Project Overview

This project is an interactive Power BI dashboard created to analyze and visualize the performance of HealthKart's influencer marketing campaigns. The objective is to provide clear insights into campaign ROI, track influencer performance, and offer data-driven recommendations to optimize future marketing spend.

---

## Dashboard Guide

The dashboard consists of two main pages:

### Page 1: Campaign Performance Dashboard

This is the executive summary view. It provides a high-level overview of key performance indicators (KPIs).

* **KPI Cards:** At the top, you will find four key metrics: Total Revenue, Total Payout to influencers, overall Return on Ad Spend (ROAS), and Total Orders generated.
* **Filter Bar:** Below the KPIs, there is a set of four dropdown filters. You can filter the entire dashboard by **Platform**, **Influencer Category**, **Brand**, and **Product** to dynamically analyze performance.
* **Charts:**
    * **ROAS by name:** A bar chart showing the top 10 most efficient influencers based on their ROAS.
    * **Sum of revenue by product:** A donut chart breaking down which products are generating the most revenue.
    * **Sum of revenue by Month:** A line chart showing revenue trends over time.

### Page 2: Interactive Performance Analysis

This page is designed for deep-dive analysis.

* **Decomposition Tree:** This visual allows you to interactively break down the **Total Payout**. You can click the "+" icon to drill down and see how the total payout is distributed across different platforms, influencer categories, products, and individual influencers.

---

## Data Model

The dashboard is built on a data model consisting of four simulated tables:

1.  **influencers**: Contains details about each influencer (ID, name, category, gender, follower count, platform).
2.  **posts**: Contains data on individual posts made by influencers (reach, likes, comments).
3.  **tracking_data**: Contains transaction-level data linking campaigns to user actions (orders, revenue).
4.  **payouts**: Contains the financial data related to influencer payments.

---

## Key Assumptions

* **ROAS Calculation:** Return on Ad Spend (ROAS) is calculated using the formula: `ROAS = Total Revenue / Total Payout`. A true *incremental* ROAS would require baseline sales data for a control group, which was not available for this assignment.