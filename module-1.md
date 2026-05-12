# Module 1: Mapping to ATT&CK from Narrative Reports

This module focuses on the interpretive methodology of translating text-based threat intelligence—such as vendor blogs and internal reports—into standardized ATT&CK techniques.
Resources for practice
## Cybereason Cobalt Kitty Report (Guided)
[Highlights Only](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20highlights%20only.pdf) Identifies the highlighted behaviors you should map to tactics and techniques for a more challenging exercise.

[Tactic Hints](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20tactic%20hints.pdf) Identifies the highlighted behaviors you should map to tactics and techniques for a more challenging exercise.

[Report Answers](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20answers.pdf) One set of answers for the exercise.

[Original Report](https://attack.mitre.org/docs/training-cti/Cybereason%20Cobalt%20Kitty%20-%20original%20report.pdf)

## FireEye APT39 Report (Unguided)
[Highlights Only](https://attack.mitre.org/docs/training-cti/FireEye%20APT39%20-%20highlights%20only.pdf) Identifies the highlighted behaviors you should map to tactics and techniques for a more challenging exercise.

[Answers](https://attack.mitre.org/docs/training-cti/FireEye%20APT39%20-%20answers.pdf) One set of answers for the exercise

[Original Report](https://attack.mitre.org/docs/training-cti/FireEye%20APT39%20-%20original%20report.pdf)

---
## Understand ATT&CK
▪ Complete the ATT&CK Fundamentals training

▪ Watch an ATT&CK presentation like MITRE ATT&CK: The Play at
Home Edition, from Black Hat USA 2019

▪ Read the Philosophy Paper and items from ATT&CK’s Getting
Started page

▪ Read the Tactic descriptions

▪ Skim the Techniques and Sub-techniques

▪ Learn a Technique and associated Sub-techniques a week

▪ Review Techniques and Sub-techniques with another analyst or a
team

## 🎯 1.Mapping to ATT&CK: Challenges and Advantages
Advantages

▪ Forces a shift in thinking about
behaviors: from indicators

▪ Allows opportunities to
discover new adversary
techniques

▪ Facilitates enhanced learning
of the “technical” side

Challenges

▪ Mapping to ATT&CK
requires a shift in thinking

▪ The volume of ATT&CK
techniques & subtechniques can seem
overwhelming

▪ The “technical” detail of
some ATT&CK techniques
can seem complex

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

## 🛠️ 3. Strategy for identifying What Technique & Sub Applies
1. **Strategy 1:** Review the list of Techniques and Sub-techniques for the Tactic you previously identified
2. **Strategy 2:** Search the ATT&CK site for Key Words and Details and Commands Strings
3. **Strategy 3:** Assess a few “Techniques Used” on the Group and Software pages to review how ATT&CK performs technique analysis
   
   For Example: Take adversary behaviors such as:
   
□ (1) ‘used email attachments,’

□ (2) ‘create scheduled task,’ and

□ (3) ‘installed tools’

## ⚠️ 3. Hedging Your Biases
It is critical to recognize our biases in CTI

▪ Two key types of bias in technique examples in ATT&CK

□ Bias introduced by us as consumers

□ Bias inherent in the sources we use

## Consumer Bias:

□ (1) Novelty Bias
Repetitive behaviors vs. Exciting Emerging Threat

□ (2) Availability Bias
Techniques we remember vs. techniques we’re not as familiar with

## Source Bias:

□ (1) Availability Bias
Reporting and Attribution skewed towards the incident
response data/specific behaviors each vendor sees regularly

□ (2) Visibility Bias
Data aligned with sensors vs all activity

□ (3) Victim Bias
Report development impacted by the interest the victim/
target engenders, and how open they are to reporting

□ (4) Novelty Bias
Marketing and Level of Impact can motivate what type of
reports are produced

## Strategies for Hedging Biases

▪ Collaborate and identify ways to
  mitigate biases
  
▪ Diversity of thought makes for stronger teams

▪ Adjust and calibrate your data
  sources
  
▪ Add different data sources
  (including your own)
  
▪ Prioritize the known over the
  unknown
  
▪ As opposed to absolute comparis

## 🧰 4. Practical Tools
* **ATT&CK Website:** The primary source of truth for all definitions and data sources.
* **ATT&CK Navigator:** A web-based tool for visualizing and color-coding techniques on the matrix.
* **TRAM (Threat Report ATT&CK Mapper):** An open-source tool designed to assist in automating the identification of ATT&CK techniques within prose.

---

