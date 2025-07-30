# 🧩 Descriptive Flexfields (DFF) – Setup

This document outlines how Aventra Global Holdings uses Descriptive Flexfields (DFFs) to extend delivered Oracle pages with additional custom fields.

---

## ✅ What Are DFFs?

- Descriptive Flexfields are customizable fields that appear on **delivered Oracle UI pages**
- You can define **segments** (fields), assign **value sets**, and determine **display logic**
- DFFs are useful when you need extra data on **person**, **assignment**, **grades**, etc.

---

## 🔧 DFF Use Cases in Aventra

| Object            | Segment Name            | Value Set or Field Type | Purpose                            |
|-------------------|--------------------------|--------------------------|-------------------------------------|
| Person Assignment | Blood Group              | Independent Value Set    | Store employee medical group        |
| Person Assignment | Joining Bonus Eligible?  | Yes/No (Boolean)         | Track bonus eligibility             |
| Grade             | Max Salary Cap Code      | Table Value Set          | Pull from Compensation Table        |
| Job               | Role Type                | Independent Value Set    | Functional / Technical / Hybrid     |

---

## 🛠️ Configuration Steps

1. **Navigate to Setup and Maintenance**
2. Search task: `Manage Descriptive Flexfields`
3. Search for the target object (e.g., “Person Assignment”)
4. Click “Edit” → Create a new **Context Segment** or use Global
5. Add fields (segments), define value sets
6. Save and Deploy to Sandbox
7. Test using **Person Management → Assignment**

---

## 🧠 Tips

- Use **Global Context** if field applies to all users
- Use **Context-Sensitive Segments** if different fields per job/region
- Always test in a **Sandbox** before deploying to Production
- Track DFF changes in your GitHub for audit/version control

---

## 📎 Example Screenshot to Add Later:
- DFF Segment List on Person Assignment
- DFF visible on Assignment Info tab (after deploy)

---

## 🔜 Next Step

→ [eff-setup.md](eff-setup.md): Add custom fields to objects like Job, Grade, or Department using Extensible Flexfields (EFF).
