# Equipment Inspection Tracker — Power Apps Portfolio Project

> Full CRUD Power Apps canvas app for industrial equipment
> inspection management — built for an HSE & Compliance division
> on a major offshore LNG construction project.

![Power Apps](https://img.shields.io/badge/Power%20Apps-742774?style=flat&logo=powerapps&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![SharePoint](https://img.shields.io/badge/SharePoint-0078D4?style=flat&logo=microsoftsharepoint&logoColor=white)
![Power Automate](https://img.shields.io/badge/Power%20Automate-0066FF?style=flat&logo=powerautomate&logoColor=white)

![Power BI Dashboard](screenshots/equipment-inspection-powerapps-SC4.png)

---

## 🔍 Business Problem

HSE teams in large-scale industrial construction environments needed a mobile-friendly digital inspection system to replace manual paper checklists — with automatic email confirmation on every submission and instant supervisor notification.

---

## 💡 What Was Built

### Power Apps (Canvas App — 4 Screens)

- **Home screen** — branded splash with quick launch buttons
- **Dashboard** — live KPI cards (Total, Passed, Review, Failed) + inspection gallery
- **Inspection Form** — 8-item checklist with Good/Fair/Poor/Fail rating buttons
- **Success Screen** — confirmation with Power Automate trigger status
- Auto-generated Equipment ID on every submission
- Auto-filled Inspector Name via `User().FullName`
- Overall Status auto-calculated — Pass / Review / Fail
- Full CRUD operations:
  - **Create** — new inspection form with 8-item checklist
  - **Read** — live gallery showing all records with colour-coded status
  - **Update** — inline edit panel slides in from right — no screen navigation needed. Edit description, zone, overall status and remarks
  - **Delete** — trash icon on each row triggers confirmation popup before permanent deletion
- Conditional colour coding throughout — green Pass, amber Review, red Fail
- Delete confirmation popup — prevents accidental deletions

### SharePoint Online

- `Equipment_Inspections` list — 16 columns
- Stores all inspection records in real time
- Direct connector to Power Apps

### Power Automate

- Triggered on every new submission regardless of status
- Sends email confirmation to inspector automatically
- Supervisors CC'd — no manual steps required
- Updates `Alert_Sent` column automatically

### Power BI

- Connected to SharePoint Equipment Inspections list
- KPI cards — Total, Passed, Review, Failed, Avg Items Failed
- Bar chart — inspections by equipment type
- Donut chart — Pass/Review/Fail status split
- Line chart — daily inspection trend
- Status breakdown by zone table
- Recent inspections table with colour badges

---

## 🛠️ Tools & Stack

Power Apps | SharePoint Online | Power Automate | Power BI

---

## 📐 Data Flow
Inspector submits form (Power Apps)
↓
Record saved to SharePoint list
↓
Power Automate triggered
↓
Email confirmation sent to inspector (supervisors CC'd)
↓
Power BI dashboard refreshes automatically

---

## 📸 Screenshots

### 🎥 Demo Video
▶️ [Watch full walkthrough on YouTube](https://youtu.be/YI05PV3pmIM)

---

### Home Screen
![Home Screen](screenshots/equipment-inspection-powerapps-SC1_NEW1.png)

### Dashboard
![Dashboard](screenshots/equipment-inspection-powerapps-SC1_NEW.png)

### Edit Panel
![Edit Panel](screenshots/equipment-inspection-powerapps-SC1-EDIT_PAGE.png)

### Delete Confirmation
![Delete Confirmation](screenshots/equipment-inspection-powerapps-SC1-DELETE_PAGE.png)

### Inspection Form
![Inspection Form](screenshots/equipment-inspection-powerapps-SC2.png)

### Success Screen
![Success Screen](screenshots/equipment-inspection-powerapps-SC3.png)

### Power BI Dashboard
![Power BI Dashboard](screenshots/equipment-inspection-powerapps-SC4.png)

---

## ⚠️ Data Note

All data shown is fully synthetic — no real company, project, or individual data is used. Generated for portfolio demonstration purposes only.

---

## 👤 Author

**Syed Mohammed Fuaad**
Power BI & Power Apps Developer | SHES Division | LNG Mega-Project, Qatar
3+ years building BI solutions and digital inspection systems for industrial HSE teams.

[GitHub](https://github.com/f4fuaad) · [LinkedIn](https://www.linkedin.com/in/syed-fuaad) · [▶️ Demo Video](https://youtu.be/YI05PV3pmIM)
