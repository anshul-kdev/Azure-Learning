# Day 14 - Log Analytics and KQL (Query Logs)

## 🎯 Objective

Learn how to collect and analyze logs using Azure Log Analytics and KQL.

---

## 🧠 Concepts Learned

### 📊 Log Analytics

* Stores logs from Azure resources
* Used for troubleshooting and monitoring

---

### 📜 Logs vs Metrics

| Type    | Purpose                        |
| ------- | ------------------------------ |
| Metrics | Performance data (CPU, memory) |
| Logs    | Detailed events and records    |

---

### 🔍 KQL (Kusto Query Language)

* Used to query logs
* Helps analyze system behavior

---

## 🛠️ Hands-on Implementation

### ✅ Created Log Analytics Workspace

* Name: `law-anshul-dev`

### ✅ Connected VM to Workspace

* Enabled monitoring

---

### ✅ Ran Queries

```kusto
Heartbeat
```

```kusto
Heartbeat
| take 10
```

```kusto
Heartbeat
| where TimeGenerated > ago(1h)
```

---

## 💻 Azure CLI Command

```bash
az monitor log-analytics workspace list --output table
```

---

## 🔍 Observations

* Logs provide detailed system information
* KQL helps filter and analyze logs
* Heartbeat shows VM availability

---

## 📚 What I Learned

* How to collect logs from Azure resources
* How to query logs using KQL
* Importance of logs in troubleshooting

---

## 🚀 Next Step

* VM troubleshooting scenarios
