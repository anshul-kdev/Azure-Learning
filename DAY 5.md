# Day 5 - Network Security Groups (NSG)

## 🎯 Objective

Learn how to secure Azure resources using Network Security Groups (NSG) and control traffic using rules.

---

## 🧠 Concepts Learned

### 🔐 Network Security Group (NSG)

* NSG acts as a firewall in Azure.
* Controls inbound and outbound traffic.
* Applies rules based on port, IP, and protocol.

---

## 🧾 Key Notes

* Inbound = Incoming traffic

* Outbound = Outgoing traffic

* NSG rules define:

  * Allow or Deny
  * Based on port and protocol

* Example:

  * Port 22 → SSH
  * Port 80 → HTTP

---

## 🛠️ Hands-on Implementation (Portal)

### ✅ Created NSG

* Name: `nsg-anshul-dev`

### ✅ Added Rules

1. allow-ssh → Port 22
2. allow-http → Port 80

### ✅ Attached NSG

* Linked NSG to `subnet-web`

---

## 💻 Azure CLI Commands

### Create NSG

```bash
az network nsg create \
  --resource-group rg-anshul-dev \
  --name nsg-cli \
  --location centralindia
```

---

### Add SSH Rule

```bash
az network nsg rule create \
  --resource-group rg-anshul-dev \
  --nsg-name nsg-cli \
  --name allow-ssh \
  --protocol Tcp \
  --direction Inbound \
  --priority 1000 \
  --source-address-prefix '*' \
  --source-port-range '*' \
  --destination-port-range 22 \
  --access Allow
```

---

## 🔍 Observations

* NSG controls traffic at subnet or VM level.
* Rules are processed based on priority.
* Default rules exist (allow VNet, deny all).

---

## 📚 What I Learned

* How to secure Azure resources
* How to create and apply NSG rules
* Basics of network security in Azure

---

## 🚀 Next Step

* Create Virtual Machine (VM)
* Connect using NSG rules
