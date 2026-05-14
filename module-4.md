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
   
## 🔄 4. The Recommendation Process
1. **Determine Priority Techniques:**
   <img width="902" height="520" alt="image" src="https://github.com/user-attachments/assets/9fdb3b5d-3ea4-4e94-a08e-697bace32044" />
2. **Research How Techniques or Sub-techniques Are Being Used:**
   <img width="912" height="505" alt="image" src="https://github.com/user-attachments/assets/6785b435-6263-4bf0-bd34-f70721ef63c7" />
4. **Research Defensive Options Related to Technique or Sub-technique:**
   <img width="898" height="520" alt="image" src="https://github.com/user-attachments/assets/ca5af21b-6435-4c8e-8f1d-21ec81672e89" />
    <img width="928" height="469" alt="image" src="https://github.com/user-attachments/assets/9fc7eaa9-fa3f-4f2e-b9d1-8c91a2409dc3" />
5. **Research Organizational Capabilities/Constraints:**
   <img width="907" height="476" alt="image" src="https://github.com/user-attachments/assets/e865c1ec-1fc8-4f27-8d0c-c66384d4ce31" />
6. **Determine the Option-specific Trade-offs for Your Enterprise:**
   <img width="915" height="499" alt="image" src="https://github.com/user-attachments/assets/399f7457-3de9-442d-bf9a-8dba9dfa2f4a" />
8. **Make Defensive Recommendations:**
   <img width="901" height="443" alt="image" src="https://github.com/user-attachments/assets/a361d7a1-376d-423d-8c1d-49b05cc4dcd9" />


## 🤝 5. Bridging the Gap: CTI to SOC & Red Team
CTI analysts function as "scouts" for other security units:
* **For the SOC (Blue Team):** Provide "What to look for," enabling the creation of high-fidelity alerts based on actual adversary behaviors.
* **For the Red Team/Pentest:** Provide "How to emulate the enemy," ensuring security testing is realistic and threat-informed.

## 📈 6. Communicating to Leadership
Reporting must be tailored to the audience to be effective:
* **Technical Teams:** Require granular details, including Technique IDs, specific log sources, and configuration parameters.
* **Executive Leadership:** Requires **Risk Analysis**. Utilize Navigator heatmaps to demonstrate "Before and After" scenarios, showing how specific investments reduce threat coverage gaps.

---


