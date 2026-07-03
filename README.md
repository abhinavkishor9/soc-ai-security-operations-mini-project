# soc-ai-security-operations-mini-project
## Overview

This mini project demonstrates an end-to-end AI-assisted Security Operations Center (SOC) investigation using realistic cybersecurity scenarios. The investigation follows the complete incident lifecycle, including log analysis, event correlation, MITRE ATT&CK mapping, Sigma rule generation, incident reporting, and AI security risk assessment.

The objective was to evaluate how AI can support SOC analysts while ensuring that all findings are validated using evidence-based investigation practices.

---

## Objectives

- Analyze Windows Security and Sysmon events.
- Correlate multiple security events into a single attack timeline.
- Map attacker behavior to the MITRE ATT&CK framework.
- Generate Sigma detection rules.
- Produce a professional SOC incident report.
- Assess AI security risks and recommend secure AI usage practices.

---

## Skills Demonstrated

- Windows Event Log Analysis
- Sysmon Investigation
- Event Correlation
- Indicators of Compromise (IoC) Analysis
- MITRE ATT&CK Mapping
- Sigma Rule Generation
- Incident Reporting
- AI Security Risk Assessment
- Evidence-Based Investigation

---

## MITRE ATT&CK Mapping

| Technique ID | Technique |
|--------------|-----------|
| T1110 | Brute Force |
| T1078 | Valid Accounts |
| T1059.001 | PowerShell |
| T1027 | Obfuscated Files or Information |
| T1071.001 | Application Layer Protocol (Web Protocols) |
| T1547.001 | Registry Run Keys / Startup Folder |

---

## Investigation Summary

The investigation identified repeated failed authentication attempts against the Administrator account followed by a successful login from the same source IP. Shortly afterward, an encoded PowerShell command was executed, followed by an outbound HTTPS connection to an external IP address.

The correlated attack sequence suggested possible credential compromise, malicious code execution, and command-and-control communication. Sigma detection rules were generated to improve future detection capabilities, and an incident report documented findings, containment actions, and recommendations. The project also evaluated AI security risks associated with handling sensitive investigation data.

---


## Key Learning Outcomes

- Correlating multiple telemetry sources improves incident understanding.
- MITRE ATT&CK provides a structured framework for mapping attacker behavior.
- Sigma rules enable standardized threat detection.
- Professional incident reporting distinguishes confirmed evidence from assumptions.
- AI accelerates SOC investigations but requires analyst validation before action.
