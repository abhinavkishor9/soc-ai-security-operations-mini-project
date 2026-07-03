# Troubleshooting Notes

## Challenges Encountered

### Correlating Individual Events

Initially, each security event appeared independent. Correlating authentication, PowerShell, and network events into a single timeline improved the overall understanding of the incident.

---

### Distinguishing Evidence from Assumptions

Not every suspicious event confirms malicious activity. Investigation findings were separated into:

- Confirmed evidence
- Investigative assumptions requiring additional validation

This reduced the likelihood of false conclusions.

---

### Sigma Rule Validation

Generated Sigma rules required review to ensure:

- Accurate detection logic.
- Appropriate severity levels.
- Relevant MITRE ATT&CK mappings.
- Reduced false positives.

---

### AI Output Verification

AI-generated findings were validated against the available log evidence before being incorporated into the investigation.

---

## Lessons Learned

- Correlation provides greater context than analyzing individual logs.
- Incident reports should remain evidence-driven.
- Sigma rules should be tested before deployment.
- AI improves investigation efficiency but does not replace analyst judgment.
- Human validation remains essential throughout the investigation process.
