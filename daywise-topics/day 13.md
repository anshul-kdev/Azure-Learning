# Day 13 - Azure Monitoring and Alerts

## 🎯 Objective

Learn how to monitor Azure resources and create alerts for proactive issue detection.

---

## 🧠 Concepts Learned

### 📊 Azure Monitor

* Tool used to track performance and health of resources

---

### 📈 Metrics

* Numerical performance data
* Example: CPU usage, network traffic

---

### 📜 Logs

* Detailed event data
* Used for debugging and analysis

---

### 🚨 Alerts

* Triggered when a condition is met
* Sends notifications (email, etc.)

---

## 🔗 Monitoring Flow

VM → Metrics/Logs → Alert → Notification

---

## 🛠️ Hands-on Implementation

### ✅ Checked Metrics

* Viewed CPU and network usage

### ✅ Created Alert Rule

* Condition: CPU > 70%
* Action: Email notification

### ✅ Explored Activity Log

* Observed VM operations and events

---

## 💻 Azure CLI (Optional)

```bash
az monitor metrics list \
  --resource <vm-resource-id> \
  --metric "Percentage CPU"
```

---

## 🔍 Observations

* Metrics provide real-time data
* Alerts help detect issues early
* Activity log tracks operations

---

## 📚 What I Learned

* Importance of monitoring in cloud
* Difference between metrics and logs
* How to create alerts in Azure

---

## 🚀 Next Step

* Log Analytics (deep monitoring)
