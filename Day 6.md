# Day 6 - Virtual Machine (VM) Creation and Connection

## 🎯 Objective

Create and connect to an Azure Virtual Machine using networking and security components.

---

## 🧠 Concepts Learned

### 💻 Virtual Machine (VM)

* A VM is a compute resource in Azure.
* It acts like a computer in the cloud.
* Can be accessed remotely using SSH or RDP.

---

## 🔗 VM Connectivity Flow

Internet → Public IP → NSG → Subnet → VNet → VM

---

## 🧾 Key Notes

* VM requires:

  * Public IP for external access
  * NSG rule to allow port
  * Correct credentials

* SSH uses port 22

* If port is blocked → connection fails

---

## 🛠️ Hands-on Implementation

### ✅ Created VM

* Name: `vm-anshul-dev`
* OS: Ubuntu
* Resource Group: `rg-anshul-dev`

### ✅ Networking

* VNet: `vnet-anshul-dev`
* Subnet: `subnet-web`
* Public IP assigned

### ✅ Security

* NSG allowed SSH (port 22)

---

## 💻 Azure CLI Command

```bash
az vm create \
  --resource-group rg-anshul-dev \
  --name vm-cli \
  --image Ubuntu2204 \
  --admin-username azureuser \
  --generate-ssh-keys
```

---

## 🔍 Observations

* VM deployment takes 1–2 minutes
* Public IP is required for remote access
* NSG controls access to VM

---

## 📚 What I Learned

* How to create a VM in Azure
* How networking and security connect to VM
* How to access VM using SSH

---

## 🚀 Next Step

* Learn VM troubleshooting
* Monitor VM performance
* Explore disk and scaling options
