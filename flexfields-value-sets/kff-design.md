# 🔢 Key Flexfields (KFF) – Design

This document outlines the design of Key Flexfields (KFFs) in Aventra Global Holdings, used to structure Job Codes, Grade Codes, and Location Codes.

---

## ✅ What Are KFFs?

- KFFs are structured, multi-segment fields used to **uniquely identify records** like Jobs, Grades, or Locations
- Used for **reporting, filtering, and logic-based access**
- Each segment can be associated with a **Value Set**

---

## 🔧 KFF Objects Used

| Object   | Flexfield Code       | Purpose                      |
|----------|----------------------|-------------------------------|
| Job      | Job Key Flexfield    | Define job codes by region/family |
| Grade    | Grade Key Flexfield  | Classify by ladder, level     |
| Location | Location Flexfield   | Region-based code structure   |

---

## 🧩 Sample Job Code Structure

| Segment         | Value Set             | Example Value     |
|------------------|------------------------|--------------------|
| Country Code     | Independent LOV        | IN, AE, UK, US     |
| Job Family       | Independent LOV        | DEV, RETAIL, HR    |
| Job Level        | Independent LOV        | I, II, SR, MGR     |

> Final Code Format: `IN.DEV.SR`

---

## 🧩 Sample Grade Code Structure

| Segment     | Value Set        | Example     |
|--------------|------------------|--------------|
| Grade Ladder | Independent LOV  | DEV_LADDER   |
| Level        | Independent LOV  | L1, L2, L3   |

> Final Code: `DEV_LADDER.L2`

---

## 🧩 Sample Location Code

| Segment     | Value Set        | Example     |
|--------------|------------------|--------------|
| Country      | Independent LOV  | UAE          |
| City         | Independent LOV  | Dubai        |

> Final Code: `UAE.DUBAI`

---

## 🛠️ Setup Steps

1. Task: **Manage Key Flexfields**
2. Search for relevant object (e.g., Job)
3. Create or edit the structure
4. Add segments → assign value sets
5. Deploy and test in **Manage Jobs/Grades/Locations**

---

## 🧠 Tips

- Design segments with **reporting in mind**
- Use **Value Sets** with descriptions for readability
- Keep segment order consistent across business units

---

✅ That’s the full coverage for DFF, EFF, and KFF.

Next up: Build `document-of-record/` for uploading and tracking critical employee documents.
