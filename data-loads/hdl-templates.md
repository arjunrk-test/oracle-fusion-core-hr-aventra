# 📥 HDL Templates – HCM Data Loader

This document outlines the HDL (HCM Data Loader) templates used in Aventra Global Holdings to upload configuration and worker data in bulk.

---

## ✅ What is HDL?

- HDL is Oracle’s tool to **bulk load data** into Fusion HCM
- Uses `.dat` files packaged in `.zip` format
- Supports loading of **setup** and **transactional** data
- Often used during initial setup, testing, data migration, and mass updates

---

## 📂 HDL Templates Included in This Project

| Template File Name         | Object Loaded           | Notes                                |
|----------------------------|--------------------------|---------------------------------------|
| `Location.dat`             | Locations                | Country-specific, uses KFFs          |
| `Grade.dat`                | Grades                   | Includes Grade Ladder if needed      |
| `Job.dat`                  | Jobs                     | Includes KFF segments, EFF if any    |
| `Position.dat`             | Positions                | Uses position tree structure         |
| `Department.dat`           | Departments              | Part of enterprise structure         |
| `BusinessUnit.dat`         | Business Units           | Tied to Legal Entities               |
| `Worker.dat`               | Employees                | Hire records with assignments        |
| `DocumentRecords.dat`      | DOR entries              | Pre-loaded documents for test users  |

---

## 🧪 Sample Use Case

- Create 10 Jobs → Upload via `Job.dat`
- Hire 5 test users → Upload via `Worker.dat`
- Assign DORs → Upload via `DocumentRecords.dat`
- Create new Legal Entity & BU → Upload and validate in UI

---

## 🛠️ Tools to Use

- Excel → Save as `.csv` → Convert to `.dat` using **Notepad++** or scripts
- Zip your `.dat` files into a `.zip` archive
- Upload in: `Data Exchange → HCM Data Loader → Import and Load Data`

---

## 🧠 Pro Tips

- Always validate files using “**Check File Contents**” before load
- Use **source keys** properly (e.g., JobCode, DepartmentCode)
- Start with **Location**, **Grade**, **Job** → then load Employees

---

## 🔜 Next Step

→ [hsdl-templates.md](hsdl-templates.md): Create spreadsheets for mass update or hire via HSDL
