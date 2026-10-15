# 🥛 SUMUL Dairy – Consumer Analytics & Market Intelligence Dashboard

[![Power BI](https://img.shields.io/badge/Power_BI-Desktop-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![ETL](https://img.shields.io/badge/Data_Pipeline-Power_Query-2BAE66)](#-data-pipeline--power-query-etl)
[![Model](https://img.shields.io/badge/Data_Model-Star_Schema-blue)](#-data-modeling)

An end-to-end Business Intelligence project built in Power BI to analyze customer feedback, brand perception, retail distribution, and price sensitivity for **SUMUL Dairy (The Surat District Co-operative Milk Producers’ Union Ltd.)** across Surat municipal zones[cite: 1, 3].

---

## 📌 Project Overview
- **Domain:** Dairy Cooperative & FMCG Market Intelligence[cite: 1, 3]
- **Tool Stack:** Microsoft Power BI Desktop, Power Query M-Engine[cite: 1, 4]
- **Geography:** Surat Municipal Corporation (Adajan, Vesu, Athwa, Katargam, Limbayat, etc.)[cite: 1, 3]
- **Theme:** Corporate Dairy Navy Blue (`#003882`)[cite: 1, 4]

---

## 🛠️ Data Pipeline & Power Query ETL
* Standardized conversational survey questions into clean business columns (`Milk_Type_Consumed`, `Delivery_Channel`, `Is_Satisfied_Sumul_Brand`)[cite: 1, 5].
* Performed text sanitization (`Text.Trim`, `Text.Clean`) and handled missing values[cite: 1].
* Mapped ordinal Likert scales into numeric values (1 to 4) for attribute benchmarking[cite: 1, 3].
* Engineered volumetric tiers (`Light <2L`, `Medium 2L–4L`, `Heavy >4L`) and total daily consumption columns[cite: 1].

---

## 🧩 Data Modeling
The report uses an optimized **Star Schema** with single-direction 1-to-many relationships to support high performance and clean DAX filter propagation[cite: 1]:
* **Dimensions:** `Dim_Customer`, `Dim_Date`, `Dim_Location`, `Dim_Product`[cite: 1, 3].
* **Fact Tables:** `Fact_Survey_Responses`, `Fact_Attribute_Ratings`, `Fact_Product_Price_Perception`[cite: 1, 3].

---

## 🖥️ Dashboard Pages
The interactive Power BI report is structured into 6 pages[cite: 1]:
1. **Customer Satisfaction & Executive Overview:** High-level brand CSAT, baseline category satisfaction, and primary satisfaction drivers[cite: 1].
2. **Customer Profile & Milk Consumption:** Daily milk format split (Pouch vs. Loose), consumption volume tiers, and monthly expenditure bands[cite: 1].
3. **Brand Preference & Buying Behavior:** Market share benchmark (Sumul/Amul vs. Competitors), doorstep delivery split, and pack variant contribution[cite: 1].
4. **Product Quality & Attribute Satisfaction Drivers:** Deep-dive into availability, taste, packaging, price, and promotional scheme ratings[cite: 1].
5. **Bakery & Value-Added Products:** Regular bread/curd purchase frequency and awareness of Amul Butter Bread and Probiotic Dahi[cite: 1].
6. **Marketing Strategy & Churn Opportunities:** Customer feedback sentiment breakdown, dissatisfaction drivers, and verbatim suggestions[cite: 1].

---

## 💡 Key Business Takeaways
* **Strong Overall CSAT (86.1%):** Brand loyalty is heavily driven by **Easy Availability (26.3%)** and **Product Freshness (18.8%)**[cite: 1].
* **Channel & SKU Dominance:** Pouch milk leads consumption (72.4%), with **Amul Gold** serving as the anchor product supported by high doorstep delivery penetration[cite: 1].
* **Promotional Friction:** Promotional schemes received the lowest rating (**1.86 / 4.0**), highlighting an area for retail margin optimization and loyalty offers[cite: 1].
* **Value-Added Headroom:** While regular curd consumption is high (69.5%), awareness of **Probiotic Dahi remains at 38.3%**, showing growth potential in emerging zones[cite: 1].

---
