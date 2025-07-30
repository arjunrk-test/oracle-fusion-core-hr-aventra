# 🔁 Employee Transfer

This document outlines the various employee transfer scenarios at Aventra Global Holdings, including inter-BU, inter-legal entity, and inter-country transfers.

---

## ✅ Transfer Types and Use Cases

| Scenario                                     | From BU                      | To BU                          | Legal Entity Change? |
|----------------------------------------------|------------------------------|--------------------------------|-----------------------|
| Internal department transfer in India        | Aventra India IT BU          | Aventra India IT BU            | ❌ No                |
| Inter-BU transfer within same LE (UK)         | UK Retail BU                 | UK Consulting BU               | ❌ No                |
| Inter-LE transfer India → USA                 | India IT BU                  | USA Manufacturing BU           | ✅ Yes               |
| Cross-country with same LE (UAE + Shared)     | UAE Consulting BU            | Global Shared BU               | ❌ No                |

---

## 📝 Key Fields Updated in Transfer

| Field                  | Notes |
|------------------------|-------|
| Business Unit          | New BU (mandatory for inter-BU) |
| Department             | New department within BU        |
| Job / Grade / Position | May or may not change           |
| Manager                | Often changed on transfer       |
| Legal Employer         | Required if inter-LE transfer   |
| Action / Reason        | e.g., “Transfer” / “Restructure”|
| Assignment Category    | Can remain same or change       |

---

## 🔁 Global Transfer Notes

- A Global Transfer creates a **new Work Relationship** in the target LDG
- The existing one is **terminated automatically**
- Typically used for:
  - Country change
  - Legal employer change
  - LDG shift (India → USA)

---

## 📋 Approval Variants

| Transfer Type                    | Approval Route                         |
|----------------------------------|----------------------------------------|
| Internal Dept Transfer (India)   | Manager → HR                           |
| Inter-BU (UK)                    | Manager only                           |
| Inter-LE / Global Transfer       | Source HR → Global HR → Target HR      |

---

## 🔗 Notes

- Ensure data access is available in **both source and target BUs**
- Security profiles should allow manager/HR to see both sides
- Manager may be auto-updated based on **position hierarchy**

---

## 🔜 Next Step

→ [termination.md](termination.md): End work relationships and manage exit flow.
