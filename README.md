# MITRE ATT&CK® for Cyber Threat Intelligence (CTI) Training

A comprehensive summary of the MITRE ATT&CK CTI training modules (0-4), outlining the methodology for mapping, analyzing, and operationalizing threat intelligence.

## 📌 Series Overview
This training provides a structured approach to using the ATT&CK framework to transform narrative reports and raw technical data into actionable defensive recommendations.

---

## 📂 Module Breakdown

### [Module 0] Introducing ATT&CK for CTI
* **Core Goal:** Establish ATT&CK as a "Common Language" between analysts and defenders.
* **CTI Definition:** Actionable knowledge about adversaries that reduces harm through better decision-making.
* **Key Value:** Move away from "Indicators of Compromise" (IPs/Hashes) and focus on "Tactics, Techniques, and Procedures" (TTPs).

### [Module 1] Mapping from Narrative Reports
* **Methodology:** A 10-step process to extract TTPs from prose (vendor blogs, news, internal reports).
* **Key Principle:** Map the **behavior**, not just the keywords.
* **Evidence-Based:** Always record the original text ("the evidence") alongside the Technique ID to maintain data integrity.

### [Module 2] Mapping from Raw Data
* **Data Sources:** Analyzing Sysmon logs, Windows Event Logs, Command-line history, and Malware sandboxing results.
* **Challenges:** High volume and low context.
* **Strategic Approaches:**
    * **Data-Driven:** Start with the log type (e.g., Registry) and see which techniques use it.
    * **Tool-Driven:** Identify the software (e.g., AdFind) and map its known capabilities.

### [Module 3] Storing and Analyzing Mapped Data
* **Aggregation:** Comparing multiple threat groups to find **Choke Points** (techniques used by many actors).
* **Visualization:** Using the **ATT&CK Navigator** to create heatmaps of threat activity.
* **Trend Analysis:** Tracking how adversary behaviors evolve over time (e.g., shifts in persistence mechanisms).

### [Module 4] Making Defensive Recommendations
* **Closing the Loop:** Turning analysis into **Mitigations** (prevention) and **Detections** (visibility).
* **Actionability:** * **For Blue Teams:** Provide specific log sources for new detection rules.
    * **For Red Teams:** Provide TTPs for realistic adversary emulation.
    * **For Leadership:** Use heatmaps to justify security spend and show risk reduction.

---

## 🛠️ The 10-Step Mapping Methodology
1. **Understand ATT&CK** (Tactics vs. Techniques)
2. **Find the Behavior** (Look for the action)
3. **Research the Behavior** (Verify technical details)
4. **Translate to a Tactic** (Determine the 'Why')
5. **Translate to a Technique** (Determine the 'How')
6. **Compare to Other Techniques** (Avoid bias)
7. **Identify Sub-Techniques** (Be specific)
8. **Record the Mapping** (Save the evidence)
9. **Review with Peers** (Quality control)
10. **Re-evaluate Over Time** (Keep it current)

---

## 🧰 Recommended Tools
* [ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/) - Visualization and scoring.
* [TRAM](https://github.com/mitre-attack/TRAM) - NLP-powered threat report mapping.
* [ATT&CK Website](https://attack.mitre.org/) - Primary knowledge base for mitigations and data sources.

---

