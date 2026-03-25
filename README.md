# 🏥 Healthcare Business Analysis — Multi-Hospital Patient Performance Dashboard

![Excel](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Dataset](https://img.shields.io/badge/Records-55%2C500%20Patients-blue?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)
![Date](https://img.shields.io/badge/Project%20Date-December%202025-orange?style=flat)

---

## 📌 Project Overview

This project is a complete **Excel-based Business Intelligence Dashboard** built for a large U.S. healthcare network. The goal was to analyze patient performance data across multiple hospitals and deliver actionable insights to the executive team.

The dashboard was built entirely in **Microsoft Excel** using **data cleaning**, **Pivot Tables**, **Pivot Charts**, and a fully interactive **Dashboard with slicers**.

---

## 🎯 Business Problem

The executive team wanted answers to the following key questions:

| # | Business Question |
|---|-------------------|
| 1 | How are patient numbers changing over time, by age group, gender, admission type, and hospital? |
| 2 | What is driving average treatment costs and hospital stay duration? |
| 3 | Which hospitals have the highest or lowest patient volumes? |
| 4 | What medications are commonly administered, and what are test result distributions? |
| 5 | How does patient volume break down by insurance provider? |
| 6 | Are there seasonal patterns in admissions that affect staffing and resource planning? |

---

## 📊 Dataset Summary

| Field | Details |
|-------|---------|
| **Total Records** | 55,500 patients |
| **Time Period** | 2019 – 2024 |
| **Source Columns** | 15 (Name, Age, Gender, Blood Type, Medical Condition, Date of Admission, Doctor, Hospital, Insurance Provider, Billing Amount, Room Number, Admission Type, Discharge Date, Medication, Test Results) |
| **Hospitals** | Multiple hospitals across the U.S. |
| **Insurance Providers** | Cigna, Medicare, UnitedHealthcare, Blue Cross, Aetna |
| **Medical Conditions** | Arthritis, Diabetes, Hypertension, Obesity, Cancer, Asthma |

---

## 🧹 Data Cleaning Steps

Performed directly in Excel before building any analysis:

- Standardized text casing in Name, Hospital, and Doctor columns (removed inconsistent capitalization)
- Checked and removed duplicate rows
- Validated Date of Admission and Discharge Date formats (converted to YYYY-MM-DD)
- Created a calculated column: **Length of Stay (Days)** = Discharge Date minus Date of Admission
- Created **Age Group** bins: 0–20, 21–30, 31–40, 41–50, 51–60, 61–70, 71+
- Created **Year** and **Month** columns extracted from Date of Admission for trend analysis
- Verified no blank values in critical columns (Gender, Admission Type, Insurance Provider)

---

## 📈 Pivot Tables & Charts Created

| # | Pivot Table / Chart | Purpose |
|---|---------------------|---------|
| 1 | Yearly Admission Trend (Line Chart) | Track patient volume year-over-year (2019–2024) |
| 2 | Patients by Medical Condition (Bar Chart) | Identify the most prevalent conditions |
| 3 | Patients by Gender (Donut Chart) | Gender distribution across the network |
| 4 | Patients by Insurance Provider (Bar Chart) | Insurance mix and reimbursement insights |
| 5 | Patients by Admission Type (Donut Chart) | Emergency vs Urgent vs Elective breakdown |
| 6 | Patients by Age Group (Bar Chart) | Age demographic distribution |
| 7 | Patients by Blood Type (Column Chart) | Blood type distribution |
| 8 | Top 5 Hospitals by Patient Volume (Bar Chart) | Hospital performance comparison |
| 9 | Top 5 Doctors by Patient Volume (Bar Chart) | Doctor-level performance |
| 10 | KPI Cards | Total Patients, Total Treatment Cost, Avg Treatment Cost, Avg Length of Stay |

---

## 📋 Dashboard Highlights

### Key KPIs
| Metric | Value |
|--------|-------|
| Total Patients | 55,500 |
| Total Treatment Cost | $1,41,74,32,043.4 |
| Avg Treatment Cost | $25,539.32 |
| Avg Length of Stay | 16 Days |

### Interactive Slicers
The dashboard includes two dynamic slicers for real-time filtering:
- **Gender** (Male / Female)
- **Age Group** (0–20, 21–30, 31–40, 41–50, 51–60, 61–70, 71+)

All charts and KPI cards update dynamically when slicers are applied.

---

## 📁 File Structure

```
Healthcare-Analysis-Excel/
│
├── healthcare_dataset.csv          # Raw dataset (55,500 records)
├── Healthcare_Analysis.xlsx        # Main Excel workbook
│   ├── Sheet 1: Brief             # Project overview & instructions
│   ├── Sheet 2: Dataset           # Cleaned & processed data
│   ├── Sheet 3: Dashboard         # Interactive dashboard
│   └── Sheet 4: Insights          # Key findings & recommendations
├── Dashboard_Screenshot.png        # Dashboard preview image
└── README.md                       # This file
```

---

## 💡 Key Insights

1. **Peak Admission Year**: 2021 recorded the highest patient admissions (11,017), with a sharp decline in 2024 (3,854 — partial year data).
2. **Balanced Gender Split**: Almost equal distribution — Female 49.95% vs Male 50.05%.
3. **Arthritis is the Leading Condition**: 9,308 patients, closely followed by Diabetes (9,304) and Hypertension (9,245).
4. **Admission Type is Evenly Distributed**: Emergency (33%), Urgent (33%), and Elective (34%) — diverse healthcare needs across the network.
5. **Cigna Leads Insurance Coverage**: 11,249 patients, slightly ahead of Medicare (11,154) and UnitedHealthcare (11,125).
6. **Age Group 71+**: The largest patient segment with 12,142 patients — highlighting elder care as a critical priority.
7. **Lipitor is the Most Prescribed Medication**: 11,140 administrations, slightly ahead of Ibuprofen and Aspirin.
8. **Abnormal Test Results**: 18,627 patients (33.6%) — a significant proportion requiring follow-up care.

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data Cleaning, Pivot Tables, Pivot Charts, Dashboard, Slicers
- **Excel Functions**: TEXT(), DATEDIF(), IF(), COUNTIFS(), SUMIFS(), AVERAGEIFS()

---

## 👩‍💻 About

📅 December 2025

---

## 📜 License

This project is for educational and portfolio purposes only. The dataset used is synthetic and does not contain real patient information.
