# Superstore Analytics Dashboard

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](#)
[![DAX](https://img.shields.io/badge/DAX-Data_Analysis_Expressions-yellowgreen?style=for-the-badge)](#)
[![Power Query](https://img.shields.io/badge/Power_Query-ETL-orange?style=for-the-badge)](#)
[![SQL](https://img.shields.io/badge/SQL-Data_Validation-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](#)
[![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](#)

An executive-level business intelligence dashboard built in **Power BI** to evaluate multi-year retail performance, year-over-year (YoY) revenue trajectories, sub-category profitability, and regional distribution across global operations.

---

## Dashboard Preview

<img width="1307" height="732" alt="Screenshot 2026-10-07 150027" src="https://github.com/user-attachments/assets/5e1255a6-ec4b-4a11-84dd-ecc3c102b8f4" />


---

## Business Problem & Objectives

Retail enterprises managing high-volume global transactions face distinct operational challenges:
* **Growth vs. Margin Disconnect:** High-volume sales categories often operate at razor-thin or negative profit margins due to steep discounting.
* **Return Rate Drag:** Unmonitored order returns degrade operational margins and inflate logistics overhead.
* **Segment Allocation:** Leadership requires immediate clarity on how customer segments (Consumer, Corporate, Home Office) contribute to bottom-line profitability.

This dashboard delivers continuous visibility into core retail metrics, enabling stakeholders to benchmark performance against prior-year baselines and isolate growth opportunities.

---

## Executive KPIs & Key Findings

* **Overall Revenue & Profit Surge:**
  * Total Sales achieved **$9.48M** (+51.30% vs. PY $6.26M).
  * Total Profit reached **$1.09M** (+51.34% vs. PY $720.18K).
* **Return Rate Optimization:**
  * Maintained a low return rate of **4.68%**, improving by **-0.07%** against prior year levels (4.75%).
* **Segment Dominance:**
  * **Consumer** leads profitability at **51.44%**, followed by **Corporate** at **30.21%** and **Home Office** at **18.35%**.
* **Regional Leaders:**
  * Top profit-generating states/regions are led by **England**, **New York**, and **California**.
* **Product Profitability Divergence:**
  * While Technology sub-categories (Phones, Copiers) drive substantial sales and profit margins, specific Furniture segments (such as Tables) show noticeable margin compression requiring discount reviews.

---

## Data Architecture & Workflow Pipeline

```text
┌─────────────────┐      ┌───────────────┐      ┌─────────────────┐      ┌─────────────────┐
│   Source Data   │ ───► │  SQL Queries  │ ───► │   Power Query   │ ───► │ Power BI Model  │
│  (Excel / CSV)  │      │ (Aggregation) │      │  (ETL & Types)  │      │  (DAX & Visual) │
└─────────────────┘      └───────────────┘      └─────────────────┘      └─────────────────┘
