# Day 10 - Azure Storage Security (Access Keys, SAS, IAM)

## 🎯 Objective

Understand how to securely access Azure Storage using Access Keys, SAS tokens, and IAM roles.

---

## 🧠 Concepts Learned

### 🔐 Access Keys

* Provide full access to storage account
* Two keys available (Key1, Key2)
* Not recommended for frequent use due to security risk

---

### 🔑 SAS Token (Shared Access Signature)

* Provides limited and temporary access
* Can define:

  * Permissions (read/write)
  * Expiry time
  * Resource scope

---

### 👤 IAM (Role-Based Access Control)

* Assign roles to users
* More secure than keys
* Example roles:

  * Storage Blob Data Reader
  * Contributor

---

## 🔍 Security Comparison

| Method     | Access Level | Security |
| ---------- | ------------ | -------- |
| Access Key | Full         | Low      |
| SAS Token  | Limited      | Medium   |
| IAM        | Role-based   | High     |

---

## 🛠️ Hands-on Implementation

### ✅ Viewed Access Keys

* Observed Key1 and Key2

### ✅ Generated SAS Token

* Created temporary access link
* Tested file access via browser

### ✅ Assigned IAM Role

* Assigned Storage Blob Data Reader role

---

## 💻 Azure CLI Command

```bash id="mf89v2"
az storage account keys list \
  --account-name stanshuldev01 \
  --resource-group rg-anshul-dev
```

---

## 🔍 Observations

* Access keys give full control
* SAS tokens are useful for temporary sharing
* IAM is the safest approach for enterprise use

---

## 📚 What I Learned

* Different ways to secure Azure storage
* Importance of limiting access
* Role-based access control in Azure

---

## 🚀 Next Step

* Connect storage with VM
* Use storage in real applications
