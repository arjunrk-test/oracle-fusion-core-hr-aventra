# 📊 HSDL Templates – HCM Spreadsheet Data Loader

This document outlines the HSDL (HCM Spreadsheet Data Loader) templates used in Aventra Global Holdings to perform mass operations via Excel-based spreadsheets.

---

## ✅ What is HSDL?

- HSDL is Oracle’s **Excel-integrated** mass upload tool
- Allows **HR users** to load/update data via preconfigured spreadsheets
- Ideal for **mass hiring**, **transfers**, **work schedule changes**, etc.

---

## 📂 Templates in Use

| Template Name          | Purpose                         | Notes                                   |
|------------------------|----------------------------------|------------------------------------------|
| `Mass Hire Template`   | Onboard 10+ new hires at once   | Includes assignment and location         |
| `Mass Termination`     | Terminate multiple employees    | Tracks final work date + reason          |
| `Work Schedule Update` | Change working hours globally   | For shared services or production teams  |
| `Mass Transfer`        | Move employees across BUs       | Used in reorg simulation                 |
| `Grade Change Upload`  | Apply grade progression         | Triggered by promotion checklist         |

---

## 🔁 Sample Use Case

- Open `Mass Hire Template` → Add 10 new employees → Submit
- Apply `Work Schedule Update` to all UAE shared BU workers
- Bulk terminate employees in UK Retail → Store shutdown scenario

---

## 🛠️ How to Use

1. Navigate to: `My Client Groups → Data Exchange → Spreadsheet Templates`
2. Select a published HSDL Template (e.g., `Worker`)
3. Download → Open in Excel with Oracle Plugin
4. Fill rows → Validate → Submit data → Check logs

---

## 📎 Tips

- Use **saved filters** to restrict editable columns
- You can use HSDL for **data correction** too
- Combine with **Checklists** (e.g., terminate → trigger offboarding)

---

## ✅ When to Use HSDL vs HDL?

| Use Case                    | Tool       |
|-----------------------------|------------|
| Mass one-time loads         | HDL        |
| Regular HR admin updates    | HSDL       |
| Initial configuration       | HDL        |
| Department transfers        | HSDL       |
| Controlled access templates | HSDL       |

---

## 🔜 Next Step

→ [hcm-extracts.md](hcm-extracts.md): Scheduled outbound reports using HCM Extract
