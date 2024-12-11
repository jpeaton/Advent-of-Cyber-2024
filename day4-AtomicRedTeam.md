# Day 4 - Atomic Red Team

## Overview
As part of the Advent of Cyber 2024 challenge, I explored detection gaps, the attack kill chain, and practical tools for understanding and simulating cyberattacks. The day's challenge provided valuable insights into blue team operations and the importance of improving detection capabilities across the kill chain.

## Key Learnings

### Detection Gaps
Reality Check: Detecting every step in an attack kill chain is rarely possible, but gaps can be minimized.

#### Reasons for Gaps:
A.) Cat-and-Mouse Game: Threat actors adapt to avoid detection, requiring constant updates to detection methods.

B.) Ambiguity in Behavior: Normal and malicious activities can overlap, complicating rule creation (e.g., international login anomalies).

### Cyber Attack Kill Chain
Cyberattacks follow a structured process, well-explained by the Unified Cyber Kill Chain.

#### Detection Strategy:
Ideal: Prevent attacks early in the chain (often not feasible).

Practical: Detect at multiple stages to reduce undetected threats before goal execution.

### MITRE ATT&CK Framework
A robust framework outlining tactics, techniques, and procedures (TTPs) used by real-world threat actors.

Includes tools like the Navigator, enabling in-depth exploration of TTPs.

### Atomic Red Team
A library of red team test cases mapped to the MITRE ATT&CK framework.

Enables blue teams to:

A.) Test detection gaps.

B.) Automate red team techniques for proactive defense improvements.

## Day's Scenario
Incident: Unauthorized use of Atomic Red Team to emulate a spearphishing attack (MITRE ATT&CK T1566.001). Left test artifacts in the system.

#### Objective: 
Recreate the emulated attack, extract artifacts, and craft detection rules to improve defenses.

#### Key Steps:
Emulation: Used PowerShell and Atomic Red parameters for testing.

Relevant parameters: -AtomicTechnique, -TestNumbers, -Cleanup, etc.

#### Artifact Analysis:
Identified artifacts like PhishingAttachment.xlsm (malicious payload).

Investigated malicious domains used to host payloads.

#### Simulation: 
Ran a test to simulate ransomware activity (e.g., BlackByte Ransomware Print Bombing).

Command: Invoke-AtomicTest T1059.003 -TestNumbers 4.

## Challenge

### Goal: 
Identify the appropriate atomic test for scripting interpreter techniques, execute it, and extract artifacts to craft effective detection rules.

### Key Artifacts:
Extracted artifacts from the attack simulation (e.g., Wareville_Ransomware.txt).

Mapped results to MITRE ATT&CK techniques and sub-techniques for improved detection.

## Reflection
This exercise deepened my understanding of the blue team's challenges and reinforced my knowledge of leveraging frameworks and tools like MITRE ATT&CK and Atomic Red Team to enhance cybersecurity defenses.
