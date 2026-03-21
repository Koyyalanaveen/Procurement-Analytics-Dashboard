# 📊 Procurement & Supplier Performance Analytics Dashboard

## 📌 Project Overview
An end-to-end Business Intelligence solution analyzing 
procurement operations and supplier performance using 
real-world Kaggle data — 777 purchase orders, $49M spend, 
5 suppliers, 5 product categories (2022–2024).

---

## 🎯 Business Problem
Procurement managers struggled to identify:
- Which suppliers are delivering on time
- Where money is being overspent
- Which vendors pose operational risk
- Cost savings opportunities vs negotiated prices

---

## 📂 Dataset
- **Source:** Kaggle — Procurement KPI Analysis Dataset
- **Records:** 777 purchase orders
- **Period:** January 2022 — January 2024
- **Suppliers:** 5 (Alpha_Inc, Beta_Supplies, 
  Gamma_Co, Delta_Logistics, Epsilon_Group)
- **Categories:** Electronics, MRO, Office Supplies, 
  Packaging, Raw Materials

---

## 🛠️ Tools Used
| Tool | Purpose |
|------|---------|
| Microsoft Excel | Data cleaning & preparation |
| Power BI Desktop | Data modeling & visualization |
| DAX | Custom measure calculations |
| Power Query | Data transformation |

---

## 📐 Data Model — Star Schema
```
        [Suppliers]
             |
             | (1 to *)
             |
[Products]——[Purchase_Orders]——[Date_Table]
```

---

## 📊 DAX Measures (12 Total)
| Measure | Purpose |
|---------|---------|
| Total Spend | SUM of Qty × Unit Price |
| Total Orders | COUNT of all POs |
| On-Time Delivery % | Delivered / Total Orders |
| Avg Lead Time | Average delivery days |
| Defect Rate % | Defective units / Total qty |
| Supplier Performance Score | Composite rating /5 |
| Total Negotiated Savings | Price gap × Quantity |
| Cost Savings Opportunity % | Savings / Total Spend |
| Compliance Rate % | Compliant orders / Total |
| Avg Cost Per Supplier | Total Spend / Suppliers |
| Pending Orders | Count of pending POs |
| Cancelled Orders | Count of cancelled POs |

---

## 🔍 Key Insights
- ⚠️ **Delta_Logistics** flagged as high-risk supplier
  - 70.2% OTD (lowest)
  - 10.83% defect rate (highest)
  - 60.82% compliance (lowest)
- 💰 **$4M savings opportunity** (8% of total spend)
  — all categories overpaying vs negotiated price
- 📦 **72.1% overall OTD** — 1 in 4 orders delayed
- 🏆 **Alpha_Inc & Epsilon_Group** — top rated at 4.3/5

---

## 📁 Repository Structure
```
Procurement-Analytics-Dashboard/
├── Procurement_Dashboard.pbix    # Power BI file
├── Procurement_KPI_Dataset.xlsx  # Cleaned dataset
├── README.md                     # Project documentation
└── screenshots/                  # Dashboard images
    ├── page1_overview.png
    ├── page2_supplier.png
    └── page3_cost.png
```

---

## 👤 Author
**Naveen Koyyala**
- LinkedIn: https://www.linkedin.com/in/naveen-koyyala/
- Email: koyyalanaveen566@gmail.com
