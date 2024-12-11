# DAY 4 - DETECTION GAPS
**Date**: December 11, 2024

**Objective**: 
The fourth challenge of TryHackMe's Advent of Cyber 2024 focused on understanding detection gaps in cybersecurity and addressing them using frameworks and tools like MITRE ATT&CK and Atomic Red Team. The goal was to explore how to identify, analyze, and close detection gaps to improve an organization's defensive posture.

## TASKS AND LEARNING OUTCOMES

### Understanding Detection Gaps:
Detection gaps are an unavoidable reality in cybersecurity due to the constant evolution of threat actor techniques and the thin line between normal and anomalous behavior. For example, while an international login might seem suspicious, it could also be a legitimate access attempt by an employee traveling for business. These challenges make it difficult to create detection rules that eliminate noise without missing critical threats. The key takeaway is that while perfect detection is unattainable, continuous learning and improvement are essential to minimizing these gaps and enhancing overall security.

### Cyber Attacks and the Kill Chain:
Cyberattacks typically follow a structured process, as outlined in the Unified Cyber Kill Chain. Detecting and disrupting attacks across multiple stages of the kill chain significantly increases the chances of mitigating threats. While the ideal scenario is to stop an attack during its initial phases, this is often unfeasible. Instead, the strategy focuses on ensuring detection coverage throughout the entire kill chain to compensate for gaps in specific phases, aiming to intercept threats before they achieve their ultimate goal.

### MITRE ATT&CK Framework:
The MITRE ATT&CK framework provides a comprehensive collection of tactics, techniques, and procedures (TTPs) observed in real-world threat actor behavior. During this exercise, the MITRE Navigator tool was used to explore TTPs and understand their application across the kill chain, helping to build a clearer picture of how adversaries operate and how to defend against them effectively.

### Atomic Red Team:
Atomic Red Team is a library of red team test cases mapped to the MITRE ATT&CK framework, designed to help blue teams identify and close detection gaps. By simulating attacks, it provides a practical way to test and refine detection capabilities. This exercise involved running pre-built tests, automating execution where possible, and ensuring cleanup of test artifacts to maintain a clean environment.

### Practical Application:
The day’s scenario involved investigating the unauthorized use of Atomic Red Team to emulate a spearphishing attack (MITRE ATT&CK T1566.001). Artifacts such as a malicious payload file, PhishingAttachment.xlsm, were extracted and analyzed. Findings were mapped to detection rules, identifying malicious or uncommon commands and relevant event details within Windows Event Viewer. The exercise concluded with a small ransomware simulation executed using PowerShell, demonstrating how adversaries might operate and how to respond effectively.

This challenge reinforced the importance of leveraging frameworks and tools like MITRE ATT&CK and Atomic Red Team to address detection gaps and improve overall defensive strategies.

## Reflection:
This challenge highlighted the importance of understanding and addressing detection gaps in cybersecurity. By simulating attacks and analyzing their artifacts, I strengthened my ability to craft effective detection rules and apply frameworks like MITRE ATT&CK in a practical setting. The exercise reinforced the need for a proactive and dynamic approach to security. 

## Skills Developed:
Gained a deeper understanding of detection gaps, how they work, and how they are handled. Developed foundational knowledge of the MITRE ATT&CK framework and Atomic Red Team, enhancing my ability to leverage these tools for improving detection capabilities. Improved my ability to simulate attacks and analyze artifacts to craft meaningful and actionable detection rules.
