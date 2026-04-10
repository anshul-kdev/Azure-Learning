# Day 11 - Connecting Azure File Share to Virtual Machine

## 🎯 Objective

Learn how to connect Azure File Share to a Virtual Machine and use it as shared storage.

---

## 🧠 Concepts Learned

### 📂 Azure File Share

* A shared storage service in Azure
* Can be mounted inside a VM
* Works like a network drive

---

## 🔗 Architecture

VM → File Share → Storage Account

---

## 🧾 Key Notes

* File share allows shared access across VMs
* Mounted using storage account credentials
* Data is stored in Azure, not inside VM

---

## 🛠️ Hands-on Implementation

### ✅ Mounted File Share

Created mount directory:

```bash
sudo mkdir /mnt/fileshare
```

Mounted using Azure-provided command

---

### ✅ Verified Access

```bash
ls /mnt/fileshare
```

---

### ✅ Created Test File

```bash
echo "hello azure" > /mnt/fileshare/test.txt
```

Verified file in Azure portal

---

## 💻 Azure CLI Command

```bash
az storage share list \
  --account-name stanshuldev01 \
  --output table
```

---

## 🔍 Observations

* Files created in VM reflect in Azure storage
* File share behaves like local folder
* Useful for shared storage scenarios

---

## 📚 What I Learned

* How to connect storage to VM
* Practical use of Azure File Share
* Real-world storage usage pattern

---

## 🚀 Next Step

* Learn backup and recovery
* Understand snapshots and redundancy
