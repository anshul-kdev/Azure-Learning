# Day 8 - Virtual Machine Deep Dive (Disks & Sizes)

## 🎯 Objective

Understand internal components of Azure Virtual Machines including disk types, VM sizes, and storage concepts.

---

## 🧠 Concepts Learned

### 💻 VM Components

* CPU and RAM (size)
* OS Disk (operating system)
* Data Disk (extra storage)
* Temporary Disk (not persistent)

---

### 💾 Disk Types

| Type           | Description                              |
| -------------- | ---------------------------------------- |
| OS Disk        | Stores operating system                  |
| Data Disk      | Stores application data                  |
| Temporary Disk | Temporary storage (data lost on restart) |

---

### ⚡ Disk Performance Types

* HDD → Low cost, slow
* SSD → Balanced
* Premium SSD → High performance

---

## 🛠️ Hands-on Implementation

### ✅ Checked VM Details

* Reviewed VM size and configuration

### ✅ Added Data Disk

* Name: `disk-data-01`
* Size: 10 GB

### ✅ Verified Disk

Used command:

```bash
lsblk
```

---

### ✅ Explored VM Sizes

* Viewed available VM sizes in Azure

---

## 💻 Azure CLI Command

```bash
az vm list-sizes --location centralindia --output table
```

---

## 🔍 Observations

* Data disks can be attached separately
* Temporary disk is not reliable
* VM size affects performance and cost

---

## 📚 What I Learned

* Structure of Azure Virtual Machine
* Disk management basics
* Importance of selecting correct VM size

---

## 🚀 Next Step

* Learn VM networking deeper
* Explore load balancing and availability
