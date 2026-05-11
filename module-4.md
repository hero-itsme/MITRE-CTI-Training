# Module 4: Making Defensive Recommendations from ATT&CK

As the final stage of the CTI lifecycle, this module focuses on operationalizing analyzed threat intelligence into concrete defensive actions to protect the organization.

---

## 🎯 1. The Goal: From "So What?" to Action
Analysis is only valuable if it results in a tangible change to the defensive posture. This stage uses patterns identified in previous modules to:
* **Prioritize Detections:** Focus on the most likely or impactful threats.
* **Update Security Policies:** Refine organizational rules and standards.
* **Influence Resource Allocation:** Provide evidence-based justifications for budget and staffing.

## 🛡️ 2. Two Main Defensive Categories
The ATT&CK framework categorizes defensive actions into two primary streams:

### **Mitigations**
Actions that **prevent** a technique from succeeding.
* **Examples:** Application sandboxing, strict user account management, or disabling unnecessary services.
* **Strategy:** Consult the "Mitigations" section on any specific ATT&CK technique page for MITRE-recommended best practices.

### **Detections**
Actions that **identify** when a technique is attempted or successful.
* **Examples:** Creating SIEM alerts for specific command-line strings or monitoring for unauthorized registry changes.
* **Strategy:** Utilize the "Data Sources" and "Detection" sections of ATT&CK to identify required telemetry and log types.

## 🔄 3. The Recommendation Workflow
To generate effective, actionable recommendations, analysts should follow this workflow:
1. **Identify the Threat:** Use mapped data to determine what techniques are targeting your sector.
2. **Assess Coverage:** Evaluate current ability to "see" or "stop" those specific techniques.
3. **Identify Gaps:** Pinpoint techniques that are highly likely but poorly defended.
4. **Evaluate Feasibility:** Determine if a mitigation is operationally possible without breaking business functions.
5. **Propose Action:** Suggest measurable changes, such as implementing *PowerShell Constrained Language Mode*.

## 🤝 4. Bridging the Gap: CTI to SOC & Red Team
CTI analysts function as "scouts" for other security units:
* **For the SOC (Blue Team):** Provide "What to look for," enabling the creation of high-fidelity alerts based on actual adversary behaviors.
* **For the Red Team/Pentest:** Provide "How to emulate the enemy," ensuring security testing is realistic and threat-informed.

## 📈 5. Communicating to Leadership
Reporting must be tailored to the audience to be effective:
* **Technical Teams:** Require granular details, including Technique IDs, specific log sources, and configuration parameters.
* **Executive Leadership:** Requires **Risk Analysis**. Utilize Navigator heatmaps to demonstrate "Before and After" scenarios, showing how specific investments reduce threat coverage gaps.

---


