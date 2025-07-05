# 🔐 **Open-Source SOC Stack: Automated Threat Detection & Incident Response**

This project demonstrates a fully integrated open-source **Security Operations Center (SOC)** using tools like **Wazuh**, **Graylog**, **MISP**, **Grafana**, and **DFIR-IRIS**, all orchestrated via **SOCFortress CoPilot**. It enables real-time **IOC detection**, **visualization**, and **case management** for effective cybersecurity monitoring and response.

---

## 📌 **Architecture Overview**
<!-- Replace with your architecture diagram image -->
*(Add a network diagram showing how all components connect)*

---

## 🧩 **Components**

| **Tool**               | **Purpose**                                 |
|------------------------|---------------------------------------------|
| **Wazuh**              | Security monitoring, threat detection       |
| **Graylog**            | Log management and alerting                 |
| **MISP**               | Threat intelligence (IOC database)          |
| **Grafana**            | Real-time dashboards & visualizations       |
| **DFIR IRIS**          | Case management and incident response       |
| **SOCFortress CoPilot**| Integration and automation between tools    |

---

## 🚀 **Key Features**

- ✅ **Real-time log analysis** from Wazuh agents (Linux & Windows)
- ✅ **IOC detection** using MISP feeds matched against live logs
- ✅ **Alerting pipeline** from Graylog to DFIR-IRIS for triage
- ✅ **Grafana dashboards** for visualizing login activity, privilege escalations, and IOC hits
- ✅ **Automated orchestration** using SOCFortress CoPilot

---

## 🛠️ **Setup Instructions**

You can replicate this SOC stack on your system with the following steps:

### **🔹 Wazuh Setup**
- Install **Wazuh Manager** and agents
- Configure **log collection** and **forwarding** to Graylog

### **🔹 Graylog Setup**
- Install and configure **Graylog**
- Set up **Fluent Bit or Filebeat** to ingest logs
- Configure **inputs** (TCP/UDP) for receiving Wazuh logs

### **🔹 MISP Integration**
- Install and configure **MISP**
- Sync **threat feeds**
- Create **pipeline rules** in Graylog to match IOCs from MISP

### **🔹 Grafana Dashboard**
- Add **Elasticsearch** or **OpenSearch** as a data source
- Import custom dashboards (e.g., **Sankey panels** for user access patterns)

### **🔹 DFIR IRIS**
- Install and configure **DFIR IRIS**
- Connect **Graylog alerts** to IRIS using **HTTP notifications**
- Use IRIS to **triage and investigate** security incidents

### **🔹 SOCFortress CoPilot**
- Deploy and configure **SOCFortress CoPilot**
- Use it to **automate integration** across all tools

---

## 📊 **Screenshots**

<!-- Insert image links or local image references -->
- 🧠 **IOC Detection**
- 🔐 **User Access Sankey Flow**
- 📁 **DFIR IRIS Case Management View**

---

## 🔍 **Use Cases**

- 🛡️ Detect **brute-force** & **unauthorized access** attempts
- 👤 Track **privilege escalation** (e.g., `sudo → root`)
- 🕵️ Investigate **IOC matches** tied to **MITRE ATT&CK**
- 📁 Escalate alerts into **DFIR IRIS** for incident response

---

## 📚 **References**

- [**Wazuh Documentation**](https://documentation.wazuh.com/)
- [**Graylog Docs**](https://docs.graylog.org/)
- [**MISP Project**](https://www.misp-project.org/)
- [**Grafana Documentation**](https://grafana.com/docs/)
- [**DFIR IRIS GitHub**](https://github.com/dfir-iris/iris-web)
- [**SOCFortress CoPilot**](https://github.com/socfortress/copilot)

---

## 📄 **License**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
This project is licensed under the MIT License.

A short and simple permissive license with conditions only requiring preservation of copyright and license notices.
Licensed works, modifications, and larger works may be distributed under different terms and without source code.

**Permissions**
✔ Commercial use  
✔ Modification  
✔ Distribution  
✔ Private use  

**Limitations**
✖ Liability  
✖ Warranty  

**Conditions**
📜 License and copyright notice  

> This is not legal advice. [Learn more about repository licenses](https://choosealicense.com/licenses/mit/)

---
