# 🧭 Area of Responsibility (AOR) – Use Cases

This document outlines how Aventra Global Holdings uses AOR (Area of Responsibility) in Oracle Fusion HCM to further define who can access what data, based on non-hierarchical ownership.

---

## ✅ What Is AOR?

- AOR is used to define **scoped access** for HR personnel, Business Partners, or other users who are **not managers**, but still need access to worker data
- AOR is **not based on line manager hierarchy**
- Can be configured for access by:
  - **Business Unit**
  - **Legal Employer**
  - **Department**
  - **Location**
  - **Job or Position**
  - **Country**

---

## 🧩 Real Use Cases in Aventra

| AOR Role                 | Scope Type     | Assigned To           | What It Enables                               |
|--------------------------|----------------|------------------------|------------------------------------------------|
| HRBP – India             | Business Unit  | Aventra India IT BU   | View & edit employees in India BU             |
| HRBP – Retail UK         | Department     | UK Retail Departments  | Access retail employees only                  |
| Global HR Analyst        | Country        | All Countries          | Access all worker data regardless of BU       |
| HR Specialist – USA Mfg  | Legal Employer | Aventra USA Corp       | View USA employees in all BUs                 |
| Finance Analyst – Dubai  | Location       | Dubai, UAE             | View employees working at Dubai location only |

---

## 🔗 How It Works

- AOR is assigned via:
  > **Manage Areas of Responsibility → Create**
- Then added to a person via:
  > **Person Management → Edit → Roles → Add AOR**
- Role assigned must be **enabled for AOR** in the Security Console

---

## 💡 Example: Assigning AOR to HRBP Retail UK

1. Create AOR definition → Department = Retail Tree
2. Assign Role: `HRBP Retail UK`
3. Result: Can view/manage workers in those departments only

---

## 🔒 Notes

- AOR can be **combined with Data Roles** to fine-tune access
- Useful when org structures are **matrixed** or span across BUs/LEs
- Works well with custom roles scoped to specific org elements

---

✅ Security model complete!
You're now ready to document **approvals and checklist automation** in the next section.
