# 💰 Pricing Clash Analysis
**Identifying price conflicts across pricing hierarchy levels using Qlik**

## 📌 Project Overview
This project analyses **price inconsistencies across different pricing hierarchy levels**, including **Customer, Head Office, and Term Code price levels**.

The objective is to detect **pricing conflicts (price clashes)** and provide visibility into which pricing level overrides another. The analysis extracts and transforms pricing data from the **Pronto ERP system using Qlik Script**, enabling the business to understand how prices and discounts are applied across different pricing structures.

This project helps improve **pricing governance, pricing transparency, and discount control**.

## 🛠️ Tools & Technologies
- **Qlik Sense** – data modelling and analytics dashboard
- **Qlik Script** – data extraction, transformation, and price clash logic
- **Pronto ERP** – source system for pricing data
- **Data Modelling** – hierarchy comparison and price validation logic

## 📊 Key Insights

- **Most items experience a single price clash**  
  The analysis shows that the majority of items have **only one pricing conflict across hierarchy levels**, while only a small portion of items experience **multiple clashes (2–3 levels)**. This indicates that pricing inconsistencies are generally isolated rather than widespread across all pricing levels.

- **Clear pricing hierarchy determines price overrides**  
  The pricing structure follows a strict hierarchy:  
  **Customer Price → Head Office Price → Term Code Price**.  
  Customer-level prices override both Head Office and Term Code prices, while Head Office prices override Term Code prices. This hierarchy explains why certain pricing conflicts occur when multiple price rules are applied to the same item.

- **High discount levels observed across pricing tiers**  
  Many discounts are configured at **relatively high levels (above 40%)**, which may significantly impact margin performance and pricing control. This insight highlights the need for stronger **pricing governance and discount monitoring**.

## 📌 Key Metrics
- **No. of PD (Price Difference)**  
  Indicates whether a price difference exists for each item across the pricing hierarchy levels.

- **Price Difference**  
  Logic-based condition used to determine whether a **real pricing clash** exists between levels.

- **P or D (Price or Discount)**  
  Identifies whether the difference is driven by a **price change or discount application**.

## 📌 Visualisations
- 📊 **Price Clash Summary** – Number of items with price differences across hierarchy levels  
- 📈 **Pricing Level Comparison** – Customer vs Head Office vs Term Code price comparison  
- 🔎 **Item-level Pricing Analysis** – Identifying items with conflicting price rules  
- 📉 **Discount Impact Analysis** – Detecting discount influence across pricing levels  

## 📂 Files in Repository
- `Pricing Clash Analysis.xlsx` – Extracted final pricing clash report
- `Pricing Clash Analysis.txt` – Qlik Script for price extraction and transformation

## 🚀 Business Impact
This analysis helps the business:

- detect **pricing conflicts across hierarchy levels**
- improve **pricing governance and consistency**
- identify **unexpected discount overrides**
- gain clearer visibility into **pricing rule application**

The project enables **data-driven pricing management and improved margin control**.
