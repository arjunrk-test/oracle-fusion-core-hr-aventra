# 👥 Hiring Employees (Add Work Relationship)

This document outlines the steps to hire employees into Aventra Global Holdings using the “Add Work Relationship” task in Oracle Fusion HCM.

---

## ✅ Hire Use Cases

| Scenario                           | Legal Employer             | BU                         | Country     |
|------------------------------------|----------------------------|----------------------------|-------------|
| Full-time Developer in India       | Aventra India Pvt Ltd      | Aventra India IT BU        | India       |
| Retail Staff in London             | Aventra UK Consulting Ltd  | Aventra UK Retail BU       | UK          |
| HR Specialist (shared services)    | Aventra Global HQ          | Aventra Global Shared BU   | UAE         |

---

## 📝 Hire Form Fields (Standard)

| Field                     | Example Value                    |
|---------------------------|----------------------------------|
| Legal Employer            | Aventra India Pvt Ltd            |
| Person Type               | Employee                         |
| Action                    | Hire                             |
| Action Reason             | New Hire                         |
| Business Unit             | Aventra India IT BU              |
| Job                       | Software Engineer I              |
| Grade                     | Developer I                      |
| Department                | Software Development             |
| Location                  | Chennai, India                   |
| Manager                   | Select from reporting hierarchy  |
| Assignment Category       | Full-Time                        |
| Working Hours             | 40/week                          |
| Probation Period          | 6 Months                         |
| Person Number             | Auto-generated                   |

---

## 🔄 Other Hire Variants to Test

- ✅ Contingent Worker (UK)
- ✅ Rehire (UAE)
- ✅ Add Work Relationship (dual employment)
- ✅ Future-Dated Hire (USA)
- ✅ Term Hire (fixed duration)

---

## 🔁 Approvals

- Configured via BPM:
  - India: Manager → HR
  - UK: Manager only
  - UAE: No approvals (auto-approved)

---

## 📋 Triggered Checklists

- **India Hire** → Laptop, Induction, ID card tasks
- **UK Hire** → Store uniform, POS login setup

---

## 🔗 Notes

- Test multiple **LDGs** and **BU visibility** for security validation
- Check that legal employer is from the correct **country-specific LDG**
- Ensure proper RDS allows visibility of job/grade/department

---

## 🔜 Next Step

→ [transfer.md](transfer.md): Handle BU, department, or legal employer transfers.
