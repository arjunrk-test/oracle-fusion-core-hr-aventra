# 🧱 Security Profiles

This document outlines the security profiles configured in Aventra Global Holdings to control access by Person, LDG, Organization, Job, and Location.

---

## ✅ Security Profile Types

| Profile Type          | Purpose                                                   |
|------------------------|-----------------------------------------------------------|
| Person Security        | Filters what person records a role can access             |
| LDG Security           | Limits visibility by Legislative Data Group (country)     |
| Organization Security  | Grants access to departments or business units            |
| Job Security           | Limits access based on job roles                          |
| Position Security      | (Optional) Used when position control is active           |
| Location Security      | Filters based on physical location                        |

---

## 🔐 Person Security Profiles

| Profile Name           | Type      | Rule Example                                  |
|------------------------|-----------|-----------------------------------------------|
| India HR Person Access | Person    | Workers in India LDG                          |
| UK Retail HRBP Scope   | Person    | Workers in UK BU under Retail Department Tree |
| Global HR View All     | Person    | All persons in enterprise                     |

---

## 🌍 LDG Security Profiles

| Profile Name       | LDG Included        |
|--------------------|---------------------|
| UAE LDG Profile    | UAE LDG             |
| India LDG Profile  | India LDG           |
| Global Profile     | All LDGs            |

---

## 🏢 Organization Profiles

| Profile Name         | BU Scope                  | Department Tree Scope          |
|----------------------|---------------------------|--------------------------------|
| UK Retail Org Access | Aventra UK Retail BU      | Department Tree: Retail Only   |
| Global Shared Org    | Global Shared BU          | All departments                |

---

## 🔗 Data Role Mapping Example

| Data Role Name               | Job Role               | Person Profile        | LDG Profile        | Org Profile             |
|------------------------------|------------------------|------------------------|---------------------|--------------------------|
| HR Specialist – India        | HR Specialist          | India HR Person Access | India LDG Profile   | Aventra India IT Org     |
| HRBP Retail UK               | HR Specialist          | UK Retail HRBP Scope   | UK LDG Profile      | UK Retail Org Access     |
| Global HR Director           | HR Analyst (Custom)    | Global HR View All     | Global Profile      | Global Shared Org        |

---

## 🔐 Notes

- Profiles are created in **Manage Security Profiles**
- Combined via **Create Data Role** → assign to users via **Security Console**
- Area of Responsibility (AOR) can also be used — covered next

---

## 🔜 Next Step

→ [aor-examples.md](aor-examples.md): Show Area of Responsibility use cases and setups.
