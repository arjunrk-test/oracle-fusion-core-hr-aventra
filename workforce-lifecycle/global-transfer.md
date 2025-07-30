# 🌍 Global Transfer

This document outlines the Global Transfer functionality in Oracle Fusion HCM, used when an employee moves between countries, LDGs, or legal employers in Aventra Global Holdings.

---

## ✅ What Is a Global Transfer?

- A **Global Transfer** creates a **new Work Relationship**
- The original relationship is **terminated automatically**
- Typically used when:
  - Changing **legal employer**
  - Moving to a different **country/LDG**
  - Transferring to another **global entity**

---

## 🧭 Real-World Use Cases

| Scenario                                | From Country | To Country | From LE                   | To LE                 |
|-----------------------------------------|--------------|------------|---------------------------|------------------------|
| India Developer moves to USA office     | India        | USA        | Aventra India Pvt Ltd     | Aventra USA Corp       |
| UAE Employee joins Global Shared BU     | UAE          | UAE        | Aventra UAE Services LLC  | Aventra Global HQ      |
| Retail manager relocated to UK HQ       | UK           | UK         | Aventra UK Consulting Ltd | Aventra UK Retail Ltd  |

---

## 📝 Fields in Global Transfer

| Field               | Notes                                        |
|---------------------|----------------------------------------------|
| Transfer Type       | Global Transfer                              |
| New Legal Employer  | Must be from target country’s LDG            |
| Start Date          | Typically 1 day after termination of source  |
| Business Unit       | Must belong to new Legal Entity              |
| Manager             | Can be reassigned                            |
| Assignment Number   | May be reset or retained                     |

---

## 🔁 What Happens Automatically?

- Old work relationship is **terminated**
- New relationship is **created under new LE**
- Assignment category, job, grade, BU must be re-selected

---

## 🔐 Security Considerations

- HR role must have access to **both source and target LDG**
- Ensure **data roles** are properly scoped for Global HR
- **Checklists** may be triggered in both source & target countries

---

## ✅ Summary

- Global Transfers are used for **country or legal entity changes**
- They create **two separate work relationships** with proper date tracking
- Approvals can be configured in **BPM** (optional)

---

🎉 Next up: Document **Security & Roles**
