# 📄 Document of Record (DOR) – Categories

This document outlines the Document of Record (DOR) categories configured in Aventra Global Holdings to maintain employee documents for legal, employment, and medical purposes.

---

## ✅ Purpose of DOR

- Store scanned or digital versions of employee documents
- Track expiration dates (e.g., Passport, Visa)
- Provide secure HR access to critical records
- Comply with legal and audit requirements

---

## 📂 Core DOR Categories in Use

| Category        | Sub-Type / Examples                     | Mandatory? | Country Scope     |
|------------------|------------------------------------------|-------------|--------------------|
| Identity         | Passport, Aadhar, PAN, SSN              | ✅ Yes     | All                |
| Employment       | Offer Letter, Contract, Transfer Letter | ✅ Yes     | All                |
| Medical          | Insurance Card, Fitness Certificate     | ❌ Optional| UAE, India         |
| Visa/Immigration | Emirates ID, Work Permit                | ✅ Yes     | UAE                |
| Retirement       | Pension Form, Retirement Letter         | ❌ Optional| UK, USA            |
| Education        | Degree Certificates                     | ✅ Yes     | India, UAE         |

---

## 🧠 Mapping by Country

| Country | Required DORs                                               |
|---------|--------------------------------------------------------------|
| India   | Aadhar, PAN, Offer Letter, Education Docs                   |
| UAE     | Passport, Emirates ID, Visa Copy, Insurance Card            |
| USA     | SSN, Contract, W-4 Form                                     |
| UK      | NI Number, Employment Contract, Pension Form                |

---

## 🛠️ Configuration Steps

1. Go to: `Setup and Maintenance`
2. Task: **Manage Document Types**
3. Add Category (e.g., Identity) → Add Document Types (e.g., Passport)
4. Define Validity Period (if applicable)
5. Configure upload permissions (Manager, HR only, Employee)
6. Test upload in: `Person Management → Document Records`

---

## 🔐 Access & Roles

- HR Specialist can **view/edit all DORs**
- Employees can **view/upload specific categories** (based on role)
- DORs can be hidden from self-service for compliance

---

## 📎 Optional Enhancements

- Add **alerts** for expiring documents (e.g., Visa in UAE)
- Link DORs to **Checklist Tasks** (Upload Passport before hire)

---

## 🔜 Next Step

→ [dor-sample-uploads.md](dor-sample-uploads.md): Real-world examples of DOR files uploaded by region and category.
