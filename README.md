# Python Data Associate Practical Exam

## 📊 Project Overview
This repository contains solutions for the **Python Data Associate Practical Exam**.  
The project focuses on cleaning, analyzing, and aggregating production data for *Spectrum Shades LLC*, a company specializing in concrete color solutions.

The goal is to identify factors affecting product quality and provide data-driven insights to improve consistency and reduce customer complaints.

---

## 📁 Dataset
The analysis is based on the file: `production_data.csv`

It contains information about production batches, including:
- Production date
- Raw material supplier
- Pigment type and quantity
- Mixing time and speed
- Product quality score

---

## 🧹 Data Cleaning (Task 1)
Key steps performed:
- Converted and validated `production_date`
- Mapped supplier codes:
  - 1 → national_supplier
  - 2 → international_supplier
- Cleaned categorical fields (`pigment_type`, `mixing_speed`)
- Handled missing values:
  - Numeric columns filled with mean/median
  - Categorical columns filled with default values
- Ensured valid ranges for:
  - Pigment quantity (1–100)
  - Product quality score (1–10)

Output: `clean_data`

---

## 📊 Aggregation Analysis (Task 2)
Grouped data by `raw_material_supplier` to compute:
- Average product quality score
- Average pigment quantity

Output: `aggregated_data`

---

## 🔍 Filtered Analysis (Task 3)
Filtered data where:
- `raw_material_supplier = 2`
- `pigment_quantity > 35`

Computed:
- Average product quality score

Output: `pigment_data`

---

## 📈 Statistical Analysis (Task 4)
Calculated:
- Mean and standard deviation for:
  - pigment_quantity
  - product_quality_score
- Pearson correlation between:
  - pigment_quantity
  - product_quality_score

Output: `product_quality`

---

## 🛠️ Tools Used
- Python 🐍
- Pandas
- NumPy

---

## 🎯 Key Insights
- Data cleaning significantly improves analysis reliability
- Supplier type impacts product quality
- Pigment quantity may influence final quality score
- Statistical relationships help identify production trends

---

## 👤 Author
Haitham Nageh
Python Data Analyst Project
