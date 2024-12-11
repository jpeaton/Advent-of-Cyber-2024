# DAY 4 - DETECTION GAPS
Date: December 11, 2024

## Objective: 
The 4th challenge of TryHackMe's Advent of Cyber 2024 focused on understanding detection gaps in cybersecurity and addressing them using frameworks and tools like MITRE ATT&CK and Atomic Red Team. The goal was to explore how to identify, analyze, and close detection gaps to improve an organization's defensive posture.

## TASKS AND LEARNING OUTCOMES

### Understanding Detection Gaps:
Detection gaps are inevitable due to:

A) The constant evolution of threat actor techniques (cat-and-mouse game).

B) The thin line between normal and anomalous behavior (e.g. international logins).

Key Takeaway: While perfect detection is unattainable, minimizing gaps through continuous learning and improvement is critical.

### Cyber Attacks and the Kill Chain:
Unified Cyber Kill Chain:

Cyberattacks follow a structured process. Detecting and disrupting attacks across multiple stages increases the chances of success.

Detection Strategy:
Aim to detect early but ensure coverage throughout the entire kill chain to compensate for gaps in specific phases.

The dream is to stop it in the first phase, but this is typically unfeasible.

### MITRE ATT&CK Framework:
Overview:
A comprehensive framework detailing tactics, techniques, and procedures (TTPs) used by real-world threat actors.

Tools:
Used the MITRE Navigator to investigate TTPs and understand their application across the kill chain.

### Atomic Red Team:
Overview:
A library of red team test cases mapped to the MITRE ATT&CK framework.
Helps blue teams test detection gaps and improve defenses.

Practical Use:
Simulated attacks using pre-built tests, including automated execution and artifact cleanup.

### Practical Application:
Scenario: Investigated unauthorized use of Atomic Red Team to emulate a spearphishing attack (MITRE ATT&CK T1566.001).

Extracted artifacts like PhishingAttachment.xlsm, a malicious payload.

Mapped findings to detection rules, including identifying malicious/uncommon commands and event details in Windows Event Viewer.

Simulation: Ran a small ransomware simulation using PowerShell.

## Reflection:
This challenge highlighted the importance of understanding and addressing detection gaps in cybersecurity. By simulating attacks and analyzing their artifacts, I strengthened my ability to craft effective detection rules and apply frameworks like MITRE ATT&CK in a practical setting. The exercise reinforced the need for a proactive and dynamic approach to security.

## Skills Developed:
Proficiency in identifying and addressing detection gaps.
Hands-on experience with the MITRE ATT&CK framework and Atomic Red Team.
Enhanced ability to simulate attacks and craft detection rules.
