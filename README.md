# Entra ID Inactive Guest Governance Automation

Automates lifecycle governance for **inactive Microsoft Entra ID (Azure AD) guest users** using **Dynamic Security Groups** and **Access Reviews** with **automatic disable and delete actions**.

This solution is designed to help organizations continuously enforce **least privilege**, reduce **external access risk**, and eliminate stale guest accounts — without manual user management.

---

## 🔐 What This Solution Does

For each partner or external company:

1. Creates (or updates) a **Dynamic Security Group** for guest users based on email domain  
2. Assigns **business owners** as group owners (reviewers)  
3. Creates an **Access Review** scoped to **inactive guest users only**  
4. Applies **Microsoft‑recommended lifecycle actions** automatically:
   - Disable inactive guest accounts
   - Delete them after a grace period (~30 days)

Result: **Continuous, auditable, and scalable guest access governance**

---

## 🔄 End‑to‑End Flow

```text
CSV Input
   ↓
Dynamic Guest Security Group (per partner)
   ↓
Group Owners = Reviewers
   ↓
Access Review (Inactive Guests Only)
   ↓
Auto‑Apply Decision
   ↓
Disable Guest → Delete After Grace Period
``
