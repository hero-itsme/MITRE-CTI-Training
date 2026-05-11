# Module 2: Mapping to ATT&CK from Raw Data

While Module 1 focuses on "finished" narrative reports, this module addresses the technical challenge of analyzing raw evidence—such as logs, malware samples, and command-line captures—to identify adversary TTPs.

---

## 🛠️ 1. What is "Raw Data" in CTI?
Raw data represents the primary, unfiltered evidence collected during an incident. Key sources include:
* **Process Logs:** Data from Sysmon or Windows Event Logs.
* **Command-Line History:** Record of executed commands on a host.
* **Malware Analysis:** Results from sandboxing or static/dynamic analysis.
* **Network Traffic:** PCAP files and Netflow data.
* **System Changes:** Modifications to Registry keys and the file system.

## ⚖️ 2. The Challenge of Raw Data
The transition from narrative reports to raw data introduces significant complexity:
* **High Volume, Low Context:** Raw data is massive in scale and lacks the pre-interpreted "story" found in narrative reports.
* **Intent Identification:** Analysts must find the "needle in the haystack" and manually determine the **Tactic** (intent) behind a specific technical action.

## 🔍 3. Mapping Methodologies
The 10-step methodology from Module 1 remains the foundation, supplemented by three specific approaches for raw evidence:

### **Approach A: Start with the Data Source**
Analyze the log entry directly. 
* *Example:* Seeing `whoami.exe` in a log leads an analyst to look up its associated technique, such as *System Service Discovery (T1007)*.

### **Approach B: Start with Tools or Attributes**
Identify known tools within the logs.
* *Example:* Finding *Mimikatz* or *AdFind* allows an analyst to map the logs to the specific techniques those tools are designed to execute.
### **Approach C: Use Detection Rules**
Leverage automated classification.
* *Example:* Use existing rules (e.g., Sigma or YARA) that are already tagged with ATT&CK IDs to classify behaviors automatically.

## 💡 4. Best Practices for Analysts
* **Look for Sequential Actions:** Avoid analyzing commands in isolation. A file download followed immediately by a registry change often signals *Persistence*.
* **Filter for Relevance:** Do not map every log line. Focus strictly on actions that align with the adversary's lifecycle.
* **Leverage the ATT&CK Knowledge Base:** Pivot to the "Data Sources" section of any technique page on the MITRE website to verify if your log type is a recognized detection vector for that technique.

---
