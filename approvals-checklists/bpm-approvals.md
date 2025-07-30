# 🔁 BPM Approval Rules

This document outlines the approval workflows configured in Aventra Global Holdings for HCM transactions using the BPM Worklist.

---

## ✅ Actions Requiring Approval

| Transaction     | Requires Approval? | Routed via              | Notes                                        |
|------------------|--------------------|--------------------------|----------------------------------------------|
| Hire             | ✅ Yes             | Supervisory Hierarchy    | Manager → HR (India, UK)                     |
| Transfer         | ✅ Yes             | Role-Based (India, US)   | Manager → BU Head or HRBP                    |
| Promotion        | ✅ Yes             | Position Hierarchy       | Only in USA BU (uses position tree)          |
| Termination      | ✅ Yes             | Role-Based (USA)         | HRBP → BU Director                           |
| Global Transfer  | ✅ Yes             | Multi-Step               | Source HR → Global HR → Target HR            |
| Term Contract End| ❌ No              | Auto-Approved            | Based on termination reason logic            |

---

## 🔗 Approval Routing Types Used

| Method                | Used In BUs / Countries                  |
|------------------------|------------------------------------------|
| Supervisory Hierarchy  | India, UK                                |
| Position Hierarchy     | USA (manufacturing org)                 |
| Role-Based             | UAE, Global Shared BU                   |

---

## 🔧 Sample: Hire Approval (India)

1. Hiring Manager initiates Hire action
2. Routed to:
   - Direct Manager (if needed)
   - HR Specialist (India)
3. Once approved → Worker becomes Active

---

## 🔁 Sample: Promotion Approval (USA – Position Based)

1. Supervisor initiates promotion
2. Routed via Position Tree:
   - Supervisor’s superior
   - HRBP for final approval

---

## 🔄 How to Configure

1. Go to **BPM Worklist**
2. Navigate to: `HCM > Transaction Name`
3. Use **If-Then Rules** with:
   - Action Type (e.g., Transfer)
   - Country / Legal Employer / BU
   - Role or Hierarchy routing
4. Save → Test in Sandbox

---

## 💡 Notes

- Some actions (e.g., Termination for retirees) are auto-approved by rule
- BPM allows full customization per **country, BU, legal entity, or job**
- Keep it simple where possible; complexity = support burden

---

## 🔜 Next Step

→ [onboarding-checklist.md](onboarding-checklist.md): Automate pre/post-hire tasks using checklist templates.
