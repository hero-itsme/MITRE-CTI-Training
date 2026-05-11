# Module 1: Mapping to ATT&CK from Narrative Reports

This module focuses on the interpretive methodology of translating text-based threat intelligence—such as vendor blogs and internal reports—into standardized ATT&CK techniques[cite: 1].

---

## 🎯 1. Why Map Narrative Reports?
Mapping external reports from vendors (e.g., Mandiant, CrowdStrike, Unit 42) provides several strategic advantages:
* **Standardized Comparison:** Enables "apples-to-apples" comparisons between different vendors' reports on the same threat actor or campaign[cite: 1].
* **Automated Ingestion:** Facilitates the ingestion of threat data into automated security tools[cite: 1].
* **Gap Analysis:** Helps security teams identify specific blind spots in their current defensive posture[cite: 1].

## 🛠️ 2. The 10-Step Mapping Methodology
The core of this module is a repeatable, rigorous process designed to ensure accuracy and consistency[cite: 1]:

1.  **Understand ATT&CK:** Master the definitions of Tactics (the "Why"), Techniques (the "How"), and Procedures (the "Specifics")[cite: 1].
2.  **Find the Behavior:** Identify verbs and actions in the text while ignoring indicators (IPs/domains) unless they reveal a specific behavior[cite: 1].
3.  **Research the Behavior:** Use the ATT&CK website or search engines to clarify unknown malware or actions[cite: 1].
4.  **Translate to a Tactic:** Determine the adversary's primary goal (e.g., gaining access vs. hiding tracks)[cite: 1].
5.  **Translate to a Technique:** Match the observed behavior to a specific ATT&CK ID[cite: 1].
6.  **Compare Techniques:** Ensure you have selected the most accurate match available[cite: 1].
7.  **Identify Sub-Techniques:** Check for more specific sub-categories (e.g., *T1547.001* vs. *T1547*)[cite: 1].
8.  **Record the Mapping:** Document the Technique ID alongside the original text ("The Evidence")[cite: 1].
9.  **Review with Peers:** Utilize a second opinion to minimize individual analyst bias[cite: 1].
10. **Re-evaluate Over Time:** Update your mappings as the ATT&CK framework or your understanding of the threat evolves[cite: 1].

## ⚠️ 3. Key Challenges & Tips
* **The "Bias" Problem:** Avoid forcing a behavior into a familiar technique; always verify against official definitions[cite: 1].
* **Tactics vs. Techniques:** Recognize that a single action may represent multiple tactics (e.g., "deleting logs" serves both *Defense Evasion* and *Impact*)[cite: 1].
* **Level of Detail:** Map only what is explicitly stated in the text; avoid making assumptions about unreported actions[cite: 1].

## 🧰 4. Practical Tools
* **ATT&CK Website:** The primary source of truth for all definitions and data sources[cite: 1].
* **ATT&CK Navigator:** A web-based tool for visualizing and color-coding techniques on the matrix[cite: 1].
* **TRAM (Threat Report ATT&CK Mapper):** An open-source tool designed to assist in automating the identification of ATT&CK techniques within prose[cite: 1].

---
*Summary generated based on MITRE ATT&CK Training Materials.*
