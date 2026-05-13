# Module 3: Storing and Analyzing ATT&CK-Mapped Data

After identifying techniques in Modules 1 and 2, this module focuses on the organization, storage, and analysis of threat data to identify patterns and inform strategic decision-making.

---

## 🎯 1. The Goal of Data Storage
Mapping data is only effective if it can be systematically retrieved and compared. High-quality storage allows analysts to solve critical problems:
* **Prevalence Identification:** Determine which techniques are most common across groups targeting specific industries.
* **Behavioral Evolution:** Track how specific actor behaviors have changed over time.
* **Resource Prioritization:** Identify where to allocate detection budgets for maximum impact.

## 🏗️ 2. Structuring the Data
Data storage must prioritize **relationships** rather than isolated files. Key data points to link include:
* **The Actor:** Who performed the action? (e.g., APT28).
* **The Technique:** What specific action was taken? (e.g., *T1566.001 - Spearphishing Attachment*).
* **The Software:** What tools were utilized? (e.g., *Mimikatz*).
* **Success/Failure:** Was the technique successful within the target environment?.
* **The Evidence:** A direct link to the source report or raw log file.

## 🗺️ 3. Key Tool: ATT&CK Navigator
The **ATT&CK Navigator** is the essential tool for visualizing and analyzing threat data:
* **Layers:** Create individual maps for different threat groups.
* **Scoring/Color Coding:** Assign weights to techniques based on frequency, severity, or internal defensive capabilities.
* **Layer Overlays:** Combine multiple layers to find overlaps. 
    * *Example:* Merging three ransomware layers might reveal a shared reliance on RDP for lateral movement, highlighting a critical detection priority.

## 🗺️ 4. Comparing Layers in Navigator
Refer to the Resources section for Exercise 

[Comparing Layers in Navigator](https://attack.mitre.org/docs/training-cti/Comparing%20Layers%20in%20Navigator.pdf) Provides detailed instructions for using Navigator to compare techniques used by APT39 and Cobalt Kitty (OceanLotus). You may find it useful to print this document (in color if possible) to have it as a reference as you work through the exercise on your screen.

[APT39 and Cobalt Kitty techniques](https://attack.mitre.org/docs/training-cti/APT39%20and%20Cobalt%20Kitty%20techniques.pdf) A list of the techniques used by APT39 and Cobalt Kitty (OceanLotus) extracted from the reports in Exercise 2. If you are already familiar with Navigator, you could use these techniques to try to create and compare layers yourself.

• The techniques and sub-techniques are listed in the “APT39 and Cobalt Kitty Techniques” PDF

Here are the following steps to do this task:
* Open ATT&CK Navigator: [http://bit.ly/attacknav](http://bit.ly/attacknav)
* Enter the techniques and sub-techniques from APT39 and Cobalt Kitty/OceanLotus into separate Navigator layers with a unique score for each layer.
* Combine the layers in Navigator to create a third layer
* Color score your third layer
* Make a list of the techniques and sub-techniques that overlap between the twogroups
   
## 🔍 5. Analysis Techniques
* **Adversary Comparison (Choke Points):** Identify techniques used by multiple adversaries. Defending a "choke point" breaks the attack chain for various groups simultaneously.
* **Trend Analysis:** Monitor shifts in adversary TTPs, such as the move from document Macros to ISO or LNK files.
* **Gap Analysis:** Compare external threat intelligence (adversary actions) against internal coverage (existing detections and visibility).

## 🌐 6. Data Standards: STIX and TAXII
To facilitate information sharing across the security community, the module highlights:
* **STIX (Structured Threat Information eXpression):** A standardized language for representing CTI.
* **TAXII (Trusted Automated eXchange of Intelligence Information):** The protocol used to transport STIX data.
* **MITRE Support:** MITRE provides the ATT&CK dataset in STIX format via a public TAXII server.

---
