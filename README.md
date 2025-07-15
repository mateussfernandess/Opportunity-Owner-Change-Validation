# 🧠 Opportunity Owner Change Validation Process

This project simulates a real-world data quality audit used to validate CRM opportunity ownership changes, based on Dynamics-style fields. It was designed to reflect enterprise logic typically used in Sales Ops or Business Intelligence teams, using synthetic data for safe portfolio sharing.

---

## 🚀 Project Summary

This pipeline helps Sales Operations teams validate change requests submitted via intake forms by comparing them against current CRM records. It flags discrepancies (e.g. change in Rep Type, Region, or Owner) and automatically generates an approval status and a communication message for the requester.

The final result is a clean, exportable CSV that shows both the original CRM state and the requested changes — supporting review, compliance, and audit tracking.

---

## 📊 Skills Demonstrated

- 🐍 Python (Pandas, Jupyter)
- 🧪 Data validation and reconciliation
- 🔄 Logic replication from SQL to Python
- 📁 Modular project structure with reusable logic
- ✅ Automated flagging & decision rules
- 📦 Realistic CRM-style data structure (Dynamics)

---

## 🗂 Folder Structure

```
Opportunity-Owner-Change-Validation/
├── data/                        # Synthetic input datasets
│   ├── user_form_data.csv
│   ├── crm_audit_data.csv
│   └── previous_audit_data.csv
├── notebooks/                  # Main notebook with full workflow
│   └── Owner_Change_Validation_Demo.ipynb
├── output/                     # Output generated from notebook
│   └── final_result.csv
├── requirements.txt            # Required Python packages
└── README.md                   # This file
```

---

## 🧪 How It Works

1. **Load Inputs**: Simulated form submission, CRM snapshot, and past audit output
2. **Compare Fields**: Owner, Rep Type, Region, Quota Owner, Quota Manager
3. **Generate Flags**:
   - Owner Change?
   - Region Change?
   - QO Change? (Quota Owner)
   - QO Manager Change?
4. **Automated Logic**:
   - Assign `Approval Status`: Approved / Review / Adjust
   - Add `Communication Guidance` for the requester
5. **Export**: All rows saved to `final_result.csv`

---

## 📎 Notes

- This project uses **synthetic data only** and does **not** expose any confidential logic or internal tools.
- In real scenarios, the CRM and audit data would be extracted via **SQL queries from internal databases** — in this version, they are replaced by CSVs for demonstration purposes.

---

## 📫 Contact

Feel free to reach out if you’d like to know more about this workflow or how I’ve implemented similar systems in production environments.

