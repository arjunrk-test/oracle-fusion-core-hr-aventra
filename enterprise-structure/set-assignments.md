# 🔗 Reference Data Set (RDS) Assignments

This document outlines how Reference Data Sets (RDS) are assigned to Business Units in Aventra Global Holdings, to control visibility of jobs, grades, departments, etc.

---

## ✅ Reference Data Sets Created

| RDS Code     | RDS Name                  | Used For                    | Notes                                 |
|--------------|---------------------------|-----------------------------|----------------------------------------|
| SET000COMMON | Aventra Common Set        | Shared jobs, grades, depts  | Used across all countries              |
| SET000IN     | Aventra India Set         | India-specific jobs, grades | Used only for India BUs                |
| SET000AE     | Aventra UAE Set           | UAE-specific departments    | Local visa/Arabic HR config            |
| SET000UK     | Aventra UK Set            | Retail grades/departments   | Store structure, UK-specific roles     |
| SET000US     | Aventra USA Set           | USA jobs and positions      | Position-controlled BU                 |

---

## 🏢 Set Assignments by BU

| Business Unit Name            | Common RDS | Country-Specific RDS |
|------------------------------|------------|-----------------------|
| Aventra UAE Consulting BU    | ✅ Yes     | SET000AE              |
| Aventra India IT BU          | ✅ Yes     | SET000IN              |
| Aventra UK Retail BU         | ✅ Yes     | SET000UK              |
| Aventra USA Manufacturing BU | ✅ Yes     | SET000US              |
| Aventra Global Shared BU     | ✅ Yes     | N/A                   |

---

## 🧠 Notes

- Each BU can access both **SET000COMMON** and its **country-specific RDS**
- This setup ensures proper data segregation while still allowing global jobs/grades

---

## 🔜 Enterprise Structure Complete!

Next up:

- Workforce Structures (Jobs, Grades, Positions)
- Security, Approvals, and Workforce Lifecycle
