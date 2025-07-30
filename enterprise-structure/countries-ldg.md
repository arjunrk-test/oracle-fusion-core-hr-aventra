# 🌍 Countries and Legislative Data Groups (LDGs)

This document outlines the countries included in the Aventra Global Holdings Core HR setup and the Legislative Data Groups (LDGs) configured for localization.

---

## ✅ Countries Included

| Country     | Purpose & Localization Requirements                                     |
|-------------|-------------------------------------------------------------------------|
| UAE         | Visa/passport fields, Arabic address format, limited payroll support   |
| India       | PAN, Aadhar, high statutory compliance, dual employment edge cases     |
| UK          | NI Number, employment terms, legal employer variations                 |
| USA         | Social Security, 401K, position-based hierarchies                      |
| Singapore   | Compact structure, good for cross-country employee testing             |

---

## 📦 LDGs Created

| LDG Name      | Country     | Notes                                                   |
|---------------|-------------|----------------------------------------------------------|
| UAE LDG       | UAE         | Arabic DFFs, visa expiration tracking                    |
| India LDG     | India       | PAN, Aadhar, local statutory setups                     |
| UK LDG        | UK          | NI Number fields, local employment types                |
| USA LDG       | USA         | SSN, 401K, USA-specific validations                     |
| Global LDG    | Global      | For shared jobs, grades, departments across countries   |
