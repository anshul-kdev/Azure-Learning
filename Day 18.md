# Day 18 - Role-Based Access Control (RBAC)

## 🎯 Objective

Learn how to control access to Azure resources using RBAC.

---

## 🧠 Concepts Learned

### 🔐 RBAC

* Controls access to Azure resources
* Based on:

  * User/Group
  * Role
  * Scope

---

### 🧾 Roles

* Reader → View only
* Contributor → Create and modify
* Owner → Full access

---

### 📍 Scope

* Subscription
* Resource Group
* Resource

---

## 🛠️ Hands-on Implementation

### ✅ Assigned Role

* Group: `grp-dev-team`
* Role: Reader
* Scope: Resource Group (`rg-anshul-dev`)

---

### ✅ Updated Role

* Changed to Contributor

---

### ✅ Explored Scope

* Tested role at resource level

---

## 💻 Azure CLI Commands

```powershell id="q89rpx"
az ad group list --display-name "grp-dev-team" --query "[0].id" -o tsv
```

```powershell id="5y3cl3"
az role assignment create --assignee <group-object-id> --role "Reader" --scope /subscriptions/<subscription-id>/resourceGroups/rg-anshul-dev
```

---

## 🔍 Observations

* Role defines permissions
* Scope defines where permissions apply
* Groups simplify access management

---

## 📚 What I Learned

* How RBAC works in Azure
* How to assign roles and manage access
* Importance of least privilege principle

---

## 🚀 Next Step

* Build complete Azure project (Day 19)
