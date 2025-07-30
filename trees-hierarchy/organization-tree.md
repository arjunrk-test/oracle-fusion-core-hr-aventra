# 🌐 Organization Tree – Aventra Global Holdings

This document outlines the enterprise-wide organization tree used to define the structural hierarchy of Legal Entities, Business Units, and Divisions across regions.

---

## ✅ Purpose

- Logical grouping of Legal Entities → BUs → Divisions
- Supports **reporting**, **extracts**, **position control**, and **managerial visibility**
- Used in some approval flows and **organization-based security profiles**

---

## 🏢 Tree Name: `Aventra_Org_Tree`

| Node                                | Type           | Description                          |
|-------------------------------------|----------------|--------------------------------------|
| Aventra Global Holdings (Root)      | Enterprise     | Parent Organization                  |
| ├── Aventra Global HQ               | Legal Entity   | Based in UAE                         |
| │   └── Aventra Global Shared BU    | Business Unit  | HR, IT, Finance                      |
| ├── Aventra India Pvt Ltd           | Legal Entity   | Registered in India                  |
| │   └── Aventra India IT BU         | Business Unit  | Tech, development                    |
| ├── Aventra UAE Services LLC        | Legal Entity   | Registered in UAE                    |
| │   └── Aventra UAE Consulting BU   | Business Unit  | Regional consulting                  |
| ├── Aventra UK Consulting Ltd       | Legal Entity   | Registered in UK                     |
| │   └── Aventra UK Retail BU        | Business Unit  | Store and eComm ops                  |
| └── Aventra USA Corp                | Legal Entity   | Registered in USA                    |
    └── Aventra USA Manufacturing BU  | Business Unit  | Plants, logistics                    |

---

## 🛠️ Setup Steps

1. Task: `Manage Organization Trees`
2. Create new tree: `Aventra_Org_Tree`
3. Add structure: LE → BU → Division (if applicable)
4. Activate the latest version
5. Use for **Org-based reporting**, security scopes

---

## 📌 Use Cases

- OTBI Report: "Headcount by Organization Tree"
- HCM Extract: Export org hierarchy + headcount
- Position Control: In org-based approval routing

---

## 🔐 Security Example

- AOR → Org = Aventra UK Retail BU only
- HRBP Retail sees only that subtree

---

## 📎 Tips

- Keep versions named clearly: `2024_v1`, `2025_v2`
- Use **date-effective** versions for org restructuring
- Include all BUs to ensure security roles work fully

---

## 🔜 Next Step

→ [position-tree.md](position-tree.md): Create position hierarchy for use in approvals and reporting.
