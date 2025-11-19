# 📊 Import Trade Data Analysis (2017–2025)
### Siddharth Associates – Data Analyst Assignment  
This project analyzes India’s steel household products import data from **2017 to 2025** using Excel.  
The objective is to clean, transform, summarize, and visualize import patterns, product categories, unit economics, HSN structures, and supplier trends.

---

## 🗂️ Project Structure

The workbook contains the following sheets:

| Sheet Name | Purpose |
|-----------|----------|
| **Raw Data** | Direct copy of the original dataset (unmodified). |
| **Cleaned Data** | Parsed, cleaned, and formula-driven dataset. Model, Qty, Unit Price, Categories extracted. |
| **HSN Lookup** | Mapping table for HSN code → description. |
| **Year Summary** | Pivot table summarizing annual import values, duty paid, YoY growth. |
| **HSN Summary** | HSN code–wise summary with total value and % contribution. |
| **Model Summary** | Model-wise and capacity-level summaries. |
| **Supplier Summary** | Year-wise analysis based on IEC (supplier). |
| **Charts** | Visual dashboards using PivotCharts. |
| **Notes** | Explanation of formulas, parsing logic, and assumptions. |

---

## 🧹 Data Cleaning & Parsing

### Columns extracted from GOODS DESCRIPTION:
- **Model Name**
- **Model Number**
- **Capacity**
- **Quantity**
- **Unit of Measure**
- **Unit Price (USD/CNY)**

### Common Excel text formulas used:
```excel
=TEXTBEFORE([@GOODS_DESCRIPTION], "(")
=TEXTAFTER([@GOODS_DESCRIPTION], "QTY:")
=MID(...)
=FIND(...)
=IFERROR(...)
=TRIM(...)
