# 🌳 Department Tree – Aventra Global

This document outlines the Department Tree structure created in Aventra Global Holdings to support approvals, AOR-based access, and reporting by business division.

---

## ✅ Purpose of Department Trees

- Enable approval chains in **Retail UK** and **Manufacturing USA**
- Scope **security profiles** by department
- Organize departments by **division or region**

---

## 🏢 Sample Department Tree: `Aventra_Department_Tree`

| Node                         | Type        | Description                              |
|------------------------------|-------------|------------------------------------------|
| Aventra Global (Root)        | Root        | All Departments                          |
| ├── Shared Services          | Division    | Common support depts (HR, Finance)       |
| │   ├── HR Shared Services   | Department  | Global HR operations                     |
| │   └── Global Finance       | Department  | Centralized payroll and AP               |
| ├── IT Services              | Division    | UAE, India                               |
| │   ├── Dev Team India       | Department  | Software development                     |
| │   └── Infra UAE            | Department  | Infrastructure Ops                       |
| ├── Retail (UK)              | Division    | Used in AOR, Approvals                   |
| │   ├── Store Ops            | Department  | Store workforce                          |
| │   └── eCommerce            | Department  | Online team                              |
| └── Manufacturing (USA)      | Division    | Plant structure                          |
    ├── Production Unit        | Department  | Assembly line                            |
    └── Logistics              | Department  | Warehouse + shipping                     |

---

## 🛠️ Setup Steps

1. Task: `Manage Department Trees`
2. Create New Tree: `Aventra_Department_Tree`
3. Add tree version, mark **active**
4. Add nodes (Divisions → Departments)
5. Publish → Use in approvals/security

---

## 🔐 Used In:

- Security Profile: UK Retail HRBP → Scoped by Retail subtree
- Approval Rule: Promotion → Position in Retail tree → Route to Director

---

## 📎 Tips

- You can create **multiple versions** (e.g., 2024 vs 2025)
- Only one version is **active** at a time
- Trees are essential for **matrixed orgs** and **access control**

---

## 🔜 Next Step

→ [organization-tree.md](organization-tree.md): Structure all Business Units and LEs for reporting and approvals.
