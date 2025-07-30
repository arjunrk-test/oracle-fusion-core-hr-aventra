# 🧱 Extensible Flexfields (EFF) – Setup

This document outlines the Extensible Flexfields (EFFs) created in Aventra Global Holdings to add custom attributes to **business objects** like Job, Grade, and Department.

---

## ✅ What Are EFFs?

- EFFs are used to add custom fields **inside business object structures**
- Unlike DFFs, EFFs are defined as **logical extensions to objects** (e.g., Jobs, Grades, Departments)
- You can define **contexts**, **attributes**, and **UI visibility**

---

## 🧩 EFF Use Cases in Aventra

| Object        | Context Name      | Attribute Label       | Field Type         | Purpose                               |
|---------------|-------------------|------------------------|--------------------|----------------------------------------|
| Job           | Global Job Info   | Skill Category         | List of Values     | Capture skill area (Java, Retail)      |
| Job           | Global Job Info   | Min Certification Level| Independent LOV     | Required certification level           |
| Grade         | Global Grade Info | Allow Variable Pay?    | Yes/No (Boolean)   | Indicate if grade is eligible for bonus|
| Department    | Global Dept Info  | Budget Code            | Table Value Set    | Financial tracking                     |

---

## 🛠️ Setup Steps

1. Go to **Setup and Maintenance**
2. Task: `Manage Extensible Flexfields`
3. Search for the object (e.g., `Job`)
4. Create or edit the **Context** (e.g., Global Job Info)
5. Add attributes → Define label, type, default
6. Save and Deploy the Flexfield
7. Navigate to the corresponding UI (e.g., Manage Jobs) to test

---

## 📎 Best Practices

- Use **clear context names** (e.g., Global Job Info)
- Align attribute names with HR or business terminology
- Use **value sets** to control data input
- Always **deploy in Sandbox**, and verify UI display

---

## 🧪 Objects Where You Can Use EFF

- Job
- Grade
- Department
- Location
- Business Unit
- Legal Entity (in some cases)

---

## 🔜 Next Step

→ [kff-design.md](kff-design.md): Define key flexfields for Jobs, Grades, and Locations using KFFs.
