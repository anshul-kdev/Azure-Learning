# Day 15 - VM Troubleshooting Scenarios

## 🎯 Objective

Learn how to troubleshoot common Azure Virtual Machine issues.

---

## 🧠 Concepts Learned

### 🔍 Troubleshooting Flow

User → Internet → Public IP → NSG → Subnet → VNet → VM

---

### ⚠️ Common Issues

* SSH not working
* VM stopped
* Wrong IP
* NSG blocking traffic

---

## 🛠️ Hands-on Scenarios

### ❌ Scenario 1: SSH Blocked

* Removed NSG rule for port 22
* Connection failed

### ✅ Fix

* Re-added NSG rule
* Connection restored

---

### ❌ Scenario 2: VM Stopped

* VM stopped manually
* Connection failed

### ✅ Fix

* Started VM
* Connection successful

---

### ❌ Scenario 3: Wrong IP

* Used incorrect public IP
* Connection failed

---

### 📊 Logs Analysis

```kusto
Heartbeat
| where TimeGenerated > ago(10m)
```

---

## 💻 Azure CLI Command

```bash
az vm get-instance-view \
  --name vm-anshul-dev \
  --resource-group rg-anshul-dev \
  --output table
```

---

## 🔍 Observations

* NSG rules directly affect connectivity
* VM must be running
* Logs help verify VM health

---

## 📚 What I Learned

* Step-by-step troubleshooting approach
* How to identify and fix issues
* Importance of logs and monitoring

---

## 🚀 Next Step

* Advanced networking concepts
