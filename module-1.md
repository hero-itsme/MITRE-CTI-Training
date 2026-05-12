# Module 1: Mapping to ATT&CK from Narrative Reports

This module focuses on the interpretive methodology of translating text-based threat intelligence—such as vendor blogs and internal reports—into standardized ATT&CK techniques.
Resources for practice
## Cybereason Cobalt Kitty Report (Guided)
[Highlights Only](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20highlights%20only.pdf) Identifies the highlighted behaviors you should map to tactics and techniques for a more challenging exercise.

[Tactic Hints](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20tactic%20hints.pdf) Identifies the highlighted behaviors you should map to tactics and techniques for a more challenging exercise.
[Report Answers](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20answers.pdf) One set of answers for the exercise.
[Original Report](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20original%20report.pdf)

## FireEye APT39 Report (Unguided)
Highlights Only Identifies the highlighted behaviors you should map to tactics and techniques for a more challenging exercise.
Answers One set of answers for the exercise
Original Report

---

## 🎯 1. Why Map Narrative Reports?
Mapping external reports from vendors (e.g., Mandiant, CrowdStrike, Unit 42) provides several strategic advantages:
* **Standardized Comparison:** Enables "apples-to-apples" comparisons between different vendors' reports on the same threat actor or campaign.
* **Automated Ingestion:** Facilitates the ingestion of threat data into automated security tools.
* **Gap Analysis:** Helps security teams identify specific blind spots in their current defensive posture.

## 🛠️ 2. The 10-Step Mapping Methodology
The core of this module is a repeatable, rigorous process designed to ensure accuracy and consistency:

1.  **Understand ATT&CK:** Master the definitions of Tactics (the "Why"), Techniques (the "How"), and Procedures (the "Specifics").
2.  **Find the Behavior:** Identify verbs and actions in the text while ignoring indicators (IPs/domains) unless they reveal a specific behavior.
3.  **Research the Behavior:** Use the ATT&CK website or search engines to clarify unknown malware or actions.
4.  **Translate to a Tactic:** Determine the adversary's primary goal (e.g., gaining access vs. hiding tracks).
5.  **Translate to a Technique:** Match the observed behavior to a specific ATT&CK ID.
6.  **Compare Techniques:** Ensure you have selected the most accurate match available.
7.  **Identify Sub-Techniques:** Check for more specific sub-categories (e.g., *T1547.001* vs. *T1547*).
8.  **Record the Mapping:** Document the Technique ID alongside the original text ("The Evidence").
9.  **Review with Peers:** Utilize a second opinion to minimize individual analyst bias.
10. **Re-evaluate Over Time:** Update your mappings as the ATT&CK framework or your understanding of the threat evolves.

## ⚠️ 3. Key Challenges & Tips
* **The "Bias" Problem:** Avoid forcing a behavior into a familiar technique; always verify against official definitions.
* **Tactics vs. Techniques:** Recognize that a single action may represent multiple tactics (e.g., "deleting logs" serves both *Defense Evasion* and *Impact*).
* **Level of Detail:** Map only what is explicitly stated in the text; avoid making assumptions about unreported actions.

## 🧰 4. Practical Tools
* **ATT&CK Website:** The primary source of truth for all definitions and data sources.
* **ATT&CK Navigator:** A web-based tool for visualizing and color-coding techniques on the matrix.
* **TRAM (Threat Report ATT&CK Mapper):** An open-source tool designed to assist in automating the identification of ATT&CK techniques within prose.

---

