# Day 17 - Microsoft Entra ID (Users and Groups)

## 🎯 Objective

Understand identity management in Azure using Microsoft Entra ID.

---

## 🧠 Concepts Learned

### 👤 Microsoft Entra ID

* Identity and access management service
* Manages users and groups

---

### 👥 Users

* Individual accounts in Azure
* Used to access resources

---

### 👨‍👩‍👧‍👦 Groups

* Collection of users
* Used to assign permissions efficiently

---

## 🧾 Key Notes

* Identity is required to access Azure resources
* Best practice: assign roles to groups, not individual users

---

## 🛠️ Hands-on Implementation

### ✅ Created User

* Username: `anshul-test-user`

### ✅ Created Group

* Name: `grp-dev-team`

### ✅ Added User to Group

* Verified membership

---

## 💻 Azure CLI Commands

```powershell
az ad user create --display-name "Test User" --user-principal-name "anshul-test-user@<your-domain>" --password "Temp@12345"
```

```powershell
az ad group create --display-name "grp-dev-team" --mail-nickname "grp-dev-team"
```

---

## 🔍 Observations

* Users represent identities
* Groups simplify permission management

---

## 📚 What I Learned

* Basics of identity in Azure
* How to create and manage users and groups

---

## 🚀 Next Step

* Role-Based Access Control (RBAC)
