# Day 16 - Azure Networking Deep Dive (IP, NIC, Concepts)

## 🎯 Objective

Understand Azure networking components including Public IP, Private IP, and NIC.

---

## 🧠 Concepts Learned

### 🌐 Public IP

* Used for external access
* Required to connect to VM from internet

---

### 🔒 Private IP

* Used for internal communication within Azure
* Assigned inside VNet

---

### 🔌 Network Interface (NIC)

* Connects VM to network
* Holds IP configuration and network settings

---

### 🔐 NSG Association

* Can be applied at:

  * Subnet level
  * NIC level

---

## 🛠️ Hands-on Implementation

### ✅ Checked VM Networking

* Viewed public and private IP

### ✅ Explored NIC

* Checked IP configuration and NSG association

---

### ✅ Verified Private IP

```bash
ip a
```

---

### ✅ Observed IP Behavior

* Stopped and started VM
* Observed public IP changes

---

## 💻 Azure CLI Command

```bash
az vm list-ip-addresses \
  --name vm-anshul-dev \
  --resource-group rg-anshul-dev \
  --output table
```

---

## 🔍 Observations

* Public IP used for external access
* Private IP used within network
* NIC connects VM to VNet

---

## 📚 What I Learned

* Difference between public and private IP
* Role of NIC in networking
* NSG association levels

---

## 🚀 Next Step

* Identity and Access (Entra ID)
