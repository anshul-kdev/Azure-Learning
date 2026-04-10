# Day 7 - Revision and Mini Lab Challenge

## 🎯 Objective

Revise all Azure fundamentals and rebuild infrastructure independently to strengthen understanding.

---

## 🧠 Topics Revised

* Azure structure (Subscription, Resource Group, Region)
* Azure CLI basics
* Virtual Network and Subnet
* Network Security Group (NSG)
* Virtual Machine (VM) creation and connection

---

## 🔗 Azure Flow Understanding

User → Internet → Public IP → NSG → Subnet → VNet → VM

---

## 🛠️ Mini Lab Challenge

Recreated full setup from scratch:

* Resource Group: `rg-day7-test`
* VNet: `vnet-day7`
* Subnet: `subnet-test`
* NSG: allow SSH (port 22)
* VM: created and connected successfully

---

## 🔍 Troubleshooting Practice

* Removed SSH rule → connection failed
* Re-added rule → connection restored

---

## 📚 What I Learned

* How all Azure components connect together
* Importance of NSG rules
* Real-world troubleshooting basics
* Confidence in building infra from scratch

---

## 🚀 Key Takeaway

Understanding flow is more important than memorizing steps.

---

## 🔜 Next Step

* Deep dive into VM (disks, scaling, availability)
