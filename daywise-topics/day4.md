# Day 4 - Azure Networking Basics (VNet & Subnet)

## 🎯 Objective

Learn and implement basic Azure networking concepts including Virtual Network (VNet) and Subnets using both Azure Portal and Azure CLI.

---

## 🧠 Concepts Learned

### 🔹 Virtual Network (VNet)

* A Virtual Network is a private network in Azure.
* It allows Azure resources (VMs, Apps, Databases) to communicate securely.
* Acts as a **network boundary**.

### 🔹 Subnet

* A Subnet is a smaller network inside a VNet.
* Used to organize and segment resources.
* Helps in security and traffic management.

---

## 🧾 Key Notes

* VNet = Network boundary

* Subnet = Segmentation inside network

* Example:

  * VNet: 10.0.0.0/16
  * Subnet: 10.0.1.0/24

👉 Smaller subnet = more control over resource grouping

---

## 🛠️ Hands-on Implementation (Portal)

### ✅ Created Virtual Network

* Name: `vnet-anshul-dev`
* Resource Group: `rg-anshul-dev`
* Region: Central India

### ✅ Created Subnets

1. `subnet-web` → 10.0.1.0/24
2. `subnet-db` → 10.0.2.0/24
3. (Optional) `subnet-app`

---

## 💻 Azure CLI Commands Used

### 🔹 Create Virtual Network with Subnet

```bash
az network vnet create \
  --name vnet-cli \
  --resource-group rg-anshul-dev \
  --location centralindia \
  --address-prefix 10.1.0.0/16 \
  --subnet-name subnet-cli \
  --subnet-prefix 10.1.1.0/24
```

---

### 🔹 List Virtual Networks

```bash
az network vnet list --output table
```

---

## 🔍 Observations

* VNets must be created in a region.
* Subnets divide the network logically.
* Address space defines IP range.
* CLI is faster and useful for automation.

---

## 📚 What I Learned

* How to create and structure Azure networks
* Difference between VNet and Subnet
* Basics of IP addressing in Azure
* Using Azure CLI alongside Portal

---

## 🚀 Next Step

* Learn Network Security Groups (NSG)
* Control traffic using allow/deny rules
