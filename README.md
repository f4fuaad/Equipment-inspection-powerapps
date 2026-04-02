# Equipment Inspection Tracker — Power Apps Portfolio Project

> Full CRUD Power Apps canvas app for industrial equipment 
> inspection management — built for an HSE & Compliance division 
> on a major offshore LNG construction project.

![Dashboard](screenshots/02_dashboard.png)

---

## 🔍 Business Problem
HSE teams in large-scale industrial construction environments 
needed a mobile-friendly digital inspection system to replace 
manual paper checklists — with automatic alerts when equipment 
items fail inspection.

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
- Full CRUD — Create, Read, Update, Delete with confirmation popup
- Inline edit panel — no screen navigation needed
- Conditional colour coding throughout

### SharePoint Online
- `Equipment_Inspections` list — 16 columns
- Stores all inspection records in real time
- Direct connector to Power Apps

### Power Automate
- Triggered on every new submission
- Sends alert email if Overall Status is Review or Fail
- Updates `Alert_Sent` column automatically

---

## 🛠️ Tools & Stack
Power Apps | SharePoint Online | Power Automate | Power BI

---

## 📐 Data Flow
```
Inspector submits form (Power Apps)
        ↓
Record saved to SharePoint list
        ↓
Power Automate triggered
        ↓
Alert email sent to HSE Manager (if Review/Fail)
        ↓
Power BI dashboard refreshes automatically
```

---

## 📸 Screenshots

### Home Screen
![Home Screen](screenshots/01_home_screen.png)

### Dashboard
![Dashboard](screenshots/02_dashboard.png)

### Inspection Form
![Inspection Form](screenshots/03_inspection_form.png)

### Success Screen
![Success Screen](screenshots/04_success_screen.png)

---

## ⚠️ Data Note
All data shown is fully synthetic — no real company, project, 
or individual data is used. Generated for portfolio 
demonstration purposes only.

---

## 👤 Author
**Syed Mohammed Fuaad**  
Power BI & Automation Analyst | Qatar  
[GitHub](https://github.com/f4fuaad) | [LinkedIn](https://www.linkedin.com/in/syed-fuaad)
