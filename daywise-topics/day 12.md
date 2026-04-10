# Day 12 - Azure Backup and Recovery Services Vault

## 🎯 Objective

Learn how to protect Azure Virtual Machines using backup and recovery services.

---

## 🧠 Concepts Learned

### 💾 Backup

* Backup is a copy of data or system
* Used for recovery in case of failure or data loss

---

### 🏦 Recovery Services Vault

* Stores backup data
* Central place for managing backups

---

### ⏰ Backup Policy

* Defines backup schedule and retention
* Example: daily backup

---

### 🔄 Restore

* Recover VM or data from backup

---

## 🔗 Backup Flow

VM → Backup → Recovery Services Vault → Restore

---

## 🛠️ Hands-on Implementation

### ✅ Created Recovery Services Vault

* Name: `rsv-anshul-dev`

### ✅ Enabled Backup

* Selected VM: `vm-anshul-dev`

### ✅ Configured Backup Policy

* Daily backup schedule

### ✅ Triggered Backup

* Ran manual backup job

---

## 💻 Azure CLI Command

```bash
az backup vault list --output table
```

---

## 🔍 Observations

* Backup jobs take time to complete
* Vault is required for storing backups
* Backup policies automate protection

---

## 📚 What I Learned

* Importance of backup in cloud
* How Azure backup works
* How to protect VM data

---

## 🚀 Next Step

* Learn restore process
* Explore high availability concepts
