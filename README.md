# 🎓 TN ITI Trainee Admission Portal
### Google Sheets + Apps Script | Tata Technologies ITI Program

![Status](https://img.shields.io/badge/Status-Completed-00C853?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Google%20Sheets%20%7C%20Apps%20Script-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Scale](https://img.shields.io/badge/Scale-71%20ITIs%20%7C%20Tamil%20Nadu-FF6B35?style=for-the-badge)

---

## 📌 Overview

A **Google Sheets-based admission management system** for the Tamil Nadu ITI 2026 batch under the Tata Technologies Industry 4.0 program. Automates data entry, validation, and reporting across 71 Government ITIs in Tamil Nadu.

Built and deployed by **Sivaselvam P**, SME at Government ITI Salem, Tata Industry 4.0 Technology Center.

---

## 🎯 Problem Solved

Managing admission data for 71 ITIs manually was error-prone and time-consuming. This portal standardized data entry, automated cross-sheet data flow, and provided instant summary dashboards for program coordinators.

---

## ✨ Key Features

- 📋 **Structured data entry** — standardized admission form with dropdowns
- ✅ **Data validation** — prevents incorrect entries at source
- 📊 **Summary dashboard** — live intake counts per ITI and trade
- 🔄 **Automated data flow** — Google Apps Script syncs data across sheets
- 📁 **Reference lists** — trade names, ITI codes, district mapping
- 🖨️ **Print-ready reports** — formatted for submission

---

## 🗂️ Sheet Structure

```
TN ITI Admission Portal
├── New Admitted (Data Entry Sheet)
│   ├── Student Name
│   ├── Trade
│   ├── ITI Code & Name
│   ├── District & Zone
│   └── Admission Date
├── Overall ITIs List (Auto-updated)
├── Intake Count Summary (Dashboard)
├── Trade Reference List
└── District → Zone Mapping
```

---

## ⚙️ Automation (Google Apps Script)

```javascript
// Auto-sync from New Admitted → Overall ITIs List
function onFormSubmit(e) {
  var sheet = SpreadsheetApp.getActiveSpreadsheet();
  var newData = sheet.getSheetByName("New Admitted");
  var masterList = sheet.getSheetByName("Overall ITIs List");
  // Append and update intake count automatically
}
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Google Sheets | Database & UI |
| Google Apps Script | Automation |
| Data Validation | Input control |
| Pivot Tables | Summary dashboard |

---

## 📊 Scale

| Metric | Value |
|---|---|
| ITIs covered | 71 |
| Districts | 38 |
| Regional zones | 7 |
| Trades tracked | 20+ |
| Users | Program coordinators, SMEs |

---

## 👨‍💻 Developer

**Sivaselvam P** — Consultant & SME  
Government ITI Salem, Tata Industry 4.0 Technology Center  
📧 psivaselvam2@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/sivaselvam-p-976097192/)
