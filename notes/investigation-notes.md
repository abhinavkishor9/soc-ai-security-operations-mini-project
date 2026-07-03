# Investigation Notes

## Incident Overview

Multiple authentication events and Sysmon logs were analyzed to determine whether they formed a single security incident.

---

## Evidence Collected

### Windows Security Events

- Event ID 4625
  - Multiple failed Administrator login attempts.
  - Source IP: 192.168.10.25

- Event ID 4624
  - Successful Administrator login.
  - Same source IP.

### Sysmon Events

- Event ID 1
  - PowerShell executed with an encoded command.

- Event ID 3
  - Outbound HTTPS connection established to 203.0.113.50.

---

## Correlated Attack Timeline

1. Multiple failed Administrator login attempts.
2. Successful Administrator authentication.
3. Encoded PowerShell execution.
4. Outbound HTTPS communication.

---

## Indicators of Compromise

- Source IP: 192.168.10.25
- Destination IP: 203.0.113.50
- Administrator Account
- powershell.exe
- Encoded PowerShell command

---

## MITRE ATT&CK

- T1110 – Brute Force
- T1078 – Valid Accounts
- T1059.001 – PowerShell
- T1027 – Obfuscated Files or Information
- T1071.001 – Application Layer Protocol

---

## Overall Assessment

The correlated events indicate a likely compromise involving credential access, PowerShell execution, and outbound network communication. The activity warranted immediate containment, additional forensic investigation, and continuous monitoring for similar behaviors across the environment.
