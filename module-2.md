# Module 2: Mapping to ATT&CK from Raw Data

While Module 1 focuses on "finished" narrative reports, this module addresses the technical challenge of analyzing raw evidence—such as logs, malware samples, and command-line captures—to identify adversary TTPs.

Resources for practice:

**Ticket 473822 (Guided)**

[Ticket 473822 Rich Text File](https://attack.mitre.org/docs/training-cti/ticket-473822.rtf) Provides raw data from a simulated incident for you to use to annotate applicable ATT&CK tactics and techniques.

[Ticket 473822 Answers](https://attack.mitre.org/docs/training-cti/ticket-473822%20answers.pdf) Provides one set of answers for the exercise.

**Ticket 473845 (Guided)**

[Ticket 473845 Rich Text File](https://attack.mitre.org/docs/training-cti/ticket-473845.rtf) Provides raw data from a simulated incident for you to use to annotate applicable ATT&CK tactics and techniques.

[Ticket 473845 Answers](https://attack.mitre.org/docs/training-cti/ticket-473845%20answers.pdf) Provides one set of answers for the exercise.

---

## 🛠️ 1. What is "Raw Data" in CTI?
Raw data represents the primary, unfiltered evidence collected during an incident. Key sources include:
* **Process Logs:** Data from Sysmon or Windows Event Logs.
* **Command-Line History:** Record of executed commands on a host.
* **Malware Analysis:** Results from sandboxing or static/dynamic analysis.
* **Network Traffic:** PCAP files and Netflow data.
* **System Changes:** Modifications to Registry keys and the file system.

## ⚖️ 2. The Challenge and Advantages of Mapping Raw Data to ATT&CK
Challenges: 

* A more advanced level of knowledge may be required
  
* You may need to review a lot more data that require different levels of expertise
  
* Adversary intent and tactics may be more difficult to identify, and require additional sources

Advantages: 

* Likely more information available at the procedure level/more detail in the data
  
* Not reinterpreting another analyst’s prose/more insight into the behaviors
  
* Facilitates enhanced learning of the “technical” side

**Pros/Cons of Mapping from the Two Sources**
<img width="840" height="442" alt="image" src="https://github.com/user-attachments/assets/016c6471-2dbc-4eb4-828d-102e5b64c1fb" />

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



---
