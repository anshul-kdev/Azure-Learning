# Day 9 - Azure Storage Accounts (Blob & File Storage)

## 🎯 Objective

Learn how to create and use Azure Storage Accounts, including Blob and File storage.

---

## 🧠 Concepts Learned

### 💾 Storage Account

* A storage account is used to store data in Azure.
* Acts like a cloud-based storage system.

---

### 📦 Types of Storage

#### Blob Storage

* Stores unstructured data (images, videos, files)
* Organized using containers

#### File Storage

* Shared file system
* Can be mounted on VMs

---

### 🔥 Access Tiers

* Hot → frequently accessed data
* Cool → less frequent access
* Archive → rarely accessed

---

## 🛠️ Hands-on Implementation

### ✅ Created Storage Account

* Name: `stanshuldev01`
* Type: Standard LRS

### ✅ Created Blob Container

* Name: `images`
* Uploaded sample file

### ✅ Tested Access

* Changed access level to public (for testing)

### ✅ Created File Share

* Name: `fileshare1`

---

## 💻 Azure CLI Commands

### Create Storage Account

```bash
az storage account create \
  --name stanshulcli01 \
  --resource-group rg-anshul-dev \
  --location centralindia \
  --sku Standard_LRS
```

---

### List Storage Accounts

```bash
az storage account list --output table
```

---

## 🔍 Observations

* Storage accounts must have globally unique names
* Blob storage is widely used for file storage
* Access level affects security

---

## 📚 What I Learned

* How Azure stores data
* Difference between blob and file storage
* Basic storage configuration and access

---

## 🚀 Next Step

* Connect storage with VM
* Learn access keys and security
