# 🧠 Customer Segmentation & Retention Analysis (RFM Model)

### 📊 Project Overview
This project applies **RFM (Recency, Frequency, Monetary)** analysis to identify key customer segments, derive actionable business insights, and develop a foundation for data-driven decision-making.

---

## 🎯 Goals
- Segment customers based on purchasing behavior.
- Identify high-value and at-risk segments.
- Provide actionable recommendations for retention and engagement.
- Prepare foundation for visual reporting and decision dashboards.

---

## 📂 Repository Structure

---

## 🧩 01_Data_ingest_and_cleaning.ipynb
**Goal:** Prepare and clean the Online Retail dataset for RFM modeling.

**Main Steps:**
- Loaded and inspected data (`online_retail.csv`)
- Cleaned missing `CustomerID` entries
- Removed negative/cancelled transactions
- Created `TotalPrice = Quantity * UnitPrice`
- Converted date and numeric fields
- Saved cleaned dataset → `data/interim/online_retail_interim.csv`

---

## 🧩 02_RFM_Feature_Engineering.ipynb
**Goal:** Generate customer-level RFM metrics and scores.

**Key Steps:**
- Computed Recency, Frequency, and Monetary per customer.
- Used quantile-based scoring (1–5 scale).
- Created `RFM_score = R + F + M`.
- Exported `customer_rfm.csv`.

---

## 🧩 03_Segmentation_Mapping_and_Labels.ipynb
**Goal:** Assign customer segments and summarize business patterns.

**Segment Rules:**
| Segment | Description |
|----------|--------------|
| Champions | Recent, frequent, high spenders |
| Loyal Customers | Repeat buyers with consistent engagement |
| At Risk | Declining engagement, but still valuable |
| Lost Customers | Long inactive, low spend |
| Recent Buyers | New or one-time buyers |
| Others | Average or mixed profiles |

---

## 📈 Key Metrics
| Metric | Value |
|--------|--------|
| Total Customers | ≈ 4K |
| Total Revenue | ≈ 4.30M |
| Avg Revenue per Customer | 1.03K |
| Avg Frequency | 4.01 |
| Avg Recency | 92 days |

---

## 💡 Insights
- **Champions (22%)** → drive **61% of total revenue**
- **Loyal Customers (23%)** → contribute **18%**
- **Lost + At Risk (31%)** → together only **12% of revenue**
- Focused loyalty programs can **retain 79% of revenue** from top 45% of customers.

---

## 🧠 Tactical Action Plan
| Segment | Goal | Recommended Actions |
|----------|------|----------------------|
| Champions | Retain loyalty | Early access, VIP rewards |
| Loyal Customers | Increase repeat buys | Tiered points, personalized offers |
| At Risk | Reactivate | Limited-time offers |
| Lost Customers | Win-back | Feedback campaigns |
| Recent Buyers | Encourage repeat | Bundle discounts |
| Others | Upsell | Showcase trending items |

---

## 🪄 Dashboard Overview (Power BI)
**File:** `RFM Segmentation Dashboard.pdf`

**Key Visuals:**
- KPI Cards (Total Revenue, Avg Recency, etc.)
- Customer Segment Distribution
- Revenue Contribution by Segment
- Top 10 High-Value Customers
- RFM & Monetary Range Slicers

---

## 📚 Tools & Technologies
- **Python** (Pandas, NumPy, Matplotlib)
- **Power BI** for interactive dashboarding
- **Excel** for initial data validation

---

## 🧾 Deliverables
| File | Description |
|------|--------------|
| `01_Data_ingest_and_cleaning.ipynb` | Data preparation |
| `02_RFM_Feature_Engineering.ipynb` | Feature creation |
| `03_Segmentation_Mapping_and_Labels.ipynb` | Segmentation & summary |
| `RFM Segmentation Dashboard.pdf` | Power BI dashboard |
| `Report.pdf` | Business insight summary |

---

## ✨ Summary
- RFM Segmentation effectively reveals customer value patterns.
- Champions & Loyal customers represent **45% of base but 79% of revenue**.
- Strong potential exists for **reactivation and loyalty campaigns**.
- Insights can guide marketing, retention, and CRM strategy.

---

**Author:** Rimsha Iram  
**Date:** October 2025  
**Internship Project — Elevvopath Analytics**
