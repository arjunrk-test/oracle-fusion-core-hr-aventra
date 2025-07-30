# 📤 HCM Extracts – Outbound Reporting & Integrations

This document describes how Aventra Global Holdings uses HCM Extracts to generate outbound reports and send data to downstream systems or for internal auditing.

---

## ✅ What Are HCM Extracts?

- HCM Extracts allow you to **pull employee data** from Fusion and export in XML, CSV, Excel, or TXT formats
- Commonly used for:
  - **Payroll integrations**
  - **Audit reports**
  - **Length-of-service tracking**
  - **Regulatory compliance**

---

## 📄 Sample Extracts

| Extract Name                        | Output Type | Purpose / Consumer             | Frequency  |
|------------------------------------|-------------|-------------------------------|------------|
| `Employees by Grade Ladder`        | Excel       | Promotion trend analysis      | Monthly    |
| `Length of Service > 6 Years`      | CSV         | Identify long-tenured staff   | Quarterly  |
| `Terminated Employees – UK BU`     | Excel       | Compliance check              | Ad Hoc     |
| `US Payroll Output File`           | XML         | Send to external payroll vendor | Biweekly  |

---

## 🔁 How to Build an Extract

1. Task: `Manage HCM Extract Definitions`
2. Create new Extract → Define data group (e.g., Worker)
3. Add attributes (e.g., Name, Job, BU, Grade)
4. Add **filters** (e.g., Grade = ‘L3’)
5. Define Output Format: XML / CSV / Excel
6. Optionally add **Delivery** (FTP, email, BI Publisher)
7. Test run → Review logs → Schedule

---

## 📎 Tips

- Combine with **Enterprise Scheduler** for automation
- Use **Extracts + OTBI** for layered reporting
- Extracts are **better for structured data**, while OTBI is better for ad hoc analytics

---

## 🧠 Pro Tip

For real-world client readiness, prepare:
- Extracts for government reporting (India, UAE, UK)
- Length of service report with **tenure bands**
- Audit: Active users without recent login

---


Next up: Build `reports-analytics/` folder to document OTBI and dashboards.
