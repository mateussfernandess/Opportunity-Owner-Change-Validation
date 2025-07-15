# Opportunity Owner Change Validation Process (Demo with Synthetic Data)

**A demonstration project for validating opportunity owner changes using simulated Dynamics CRM data.**

## 🚩 What does this project do?

- Loads user-submitted "opportunity" data (simulating an **intake form** completed by Sales Reps requesting owner changes)
- Loads CRM records (simulating audit snapshots from Dynamics CRM)
- Loads previous audit results (e.g., prior month’s audit outcome)
- Flags changes in ownership, region, rep type, etc.
- Generates "Approval Status" (`Approved`, `Review`, `Adjust`) and communication guidance based on business rules
- Outputs a clear CSV with both perspectives for every opportunity

## 🔎 How the Data is Used

- In a **real scenario**, both CRM audit data and previous months' audit data would be retrieved directly from the company database using SQL queries.
- For sharing and demonstration purposes, these data sources are represented by simple CSV files in this repository.
- **All data is synthetic.**

## 📂 Folder structure

Opportunity-Owner-Change-Validation/
├── data/
│   ├── user_form_data.csv
│   ├── crm_audit_data.csv
│   └── previous_audit_data.csv
├── output/
│   └── final_result.csv (generated when you run the notebook)
├── notebooks/
│   └── Owner_Change_Validation_Demo.ipynb
└── README.md

## 🚀 How to run

1. Clone/download this repo
2. Open `notebooks/Owner_Change_Validation_Demo.ipynb` in Jupyter
3. Run all cells to generate `/output/final_result.csv`
4. Review the results

## ⚠️ Disclaimer

> This project uses only synthetic data and standard Dynamics CRM field names.  
> No proprietary, confidential, or real business data is included.
