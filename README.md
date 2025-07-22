# 🧪 Kimia Farma Analytics SQL Project

> A SQL-based data transformation project to build a clean analytical table from multiple raw sources, developed during a project-based internship at **Rakamin Academy**.

---

## 📌 Project Overview

In this project, I wrote a SQL query to join and enrich four different datasets from **Kimia Farma**, a pharmaceutical company in Indonesia. The goal was to create a single analytical table that includes key business metrics such as **nett sales** and **nett profit**, which can be used for further analysis and dashboarding.

---

## 🧰 Tools & Technologies

- SQL (BigQuery Standard SQL)
- Google BigQuery (cloud data warehouse)
- Rakamin Academy Project-based Internship

---

## 🗃️ Data Sources

The following tables were joined:

1. `kf_final_transaction` – Transactional data
2. `kf_kantor_cabang` – Branch details
3. `kf_product` – Product information
4. `kf_inventory` – Inventory records

---

## ⚙️ Key Calculations

The query includes several calculated fields:
- **Nett Sales**  
  `(price - (price * discount_percentage))`

- **Estimated Gross Margin (%)**  
  Based on pricing tiers using `CASE WHEN`

- **Nett Profit**  
  `nett_sales * gross_margin_percentage`

- **Branch Rating & Transaction Rating**  
  Included from related tables

---

## 💡 Insights

This analytics table can support a range of business questions such as:
- Which branches generate the most profit?
- What pricing tiers contribute most to revenue?
- How effective are the applied discount strategies?

---

## 🙋🏻‍♀️ Notes

This project was created as part of the **Rakamin Academy** project-based internship program. While the logic works well for the given structure, there is still room for optimization and validation with business stakeholders. Feedback is always welcome!

---
