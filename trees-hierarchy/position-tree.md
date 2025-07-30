# 🪜 Position Tree – Aventra Global

This document outlines the Position Tree created to define the reporting structure based on **positions** rather than people, used mainly in the USA BU for manufacturing operations.

---

## ✅ Purpose of Position Trees

- Required for **position-based approval workflows**
- Drives **reporting**, **managerial visibility**, and **vacancy tracking**
- Useful in orgs where **roles stay fixed** even when people change

---

## 🏢 Tree Name: `Aventra_Position_Tree_USA`

| Position Title             | Reports To Position         | Notes                                 |
|----------------------------|-----------------------------|----------------------------------------|
| Plant General Manager      | None (Top Node)             | Head of USA Manufacturing              |
| ├── Production Supervisor  | Plant General Manager       | Oversees production lines             |
| │   └── Assembly Technician| Production Supervisor       | Worker on manufacturing line          |
| ├── Logistics Manager      | Plant General Manager       | Manages inventory and shipping        |
| │   └── Warehouse Associate| Logistics Manager           | Operates within warehouse              |

---

## 🧩 Other Position Trees (Global Shared)

- `Aventra_Global_Position_Tree`
  - Global HR Director
    - HRBP – India
    - HRBP – UK
  - CIO
    - IT Manager UAE
    - Dev Manager India

---

## 🔁 Usage in Approvals

- **BPM Rule**: If Position = “Assembly Technician”  
  → Route to “Production Supervisor” → “Plant GM”
- Used in **USA BU only** (India/UK use Supervisory Hierarchy)

---

## 🛠️ Setup Steps

1. Task: `Manage Position Trees`
2. Create tree: `Aventra_Position_Tree_USA`
3. Add tree version and positions
4. Mark **Active**
5. Link positions via "Reports To" logic
6. Assign positions to **Jobs** via `Manage Positions`

---

## 🔐 Tip: Vacancy Tracking

- Use Position Tree to view **open vs filled positions**
- Can control **position hierarchy-based security profiles** for high sensitivity roles

---

## 📎 Notes

- Position Trees ≠ Line Managers (but they can align)
- Works best in **structured, plant-based, retail, or government orgs**

---

✅ Trees section complete!

Next up: move into 📂 `data-loads/` → starting with `hdl-templates.md`
