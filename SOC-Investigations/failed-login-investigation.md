# SOC Lab 01: Failed Login Investigation

## 1. Overview

- **Category:** SOC / Blue Team
- **Lab type:** Simulated investigation
- **Difficulty:** Beginner
- **Status:** Initial analysis completed; further investigation required
- **Tools:** Manual log analysis
- **Data source:** Fictional training records

## 2. Objective

Investigate repeated failed login attempts against a single user account and identify the next steps a SOC analyst should take.

## 3. Scenario

A security monitoring system detects five failed login attempts against the same account within approximately five minutes. The analyst must review the evidence and determine whether further investigation is necessary.

## 4. Evidence

| Time | Account | Source IP | Result |
|---|---|---|---|
| 10:01 | user1 | 192.0.2.45 | Failed |
| 10:02 | user1 | 192.0.2.45 | Failed |
| 10:03 | user1 | 192.0.2.45 | Failed |
| 10:04 | user1 | 192.0.2.45 | Failed |
| 10:05 | user1 | 192.0.2.45 | Failed |

*Note: All records are fictional. The IP address belongs to a range reserved for documentation examples.*

## 5. Analysis

- Five failed login attempts targeted the same account.
- All five events originated from the same source IP.
- The repeated pattern may be consistent with password guessing.
- The available evidence does not establish whether the attempts were malicious.
- No successful login information was provided in this exercise.

## 6. Risk Assessment

**Preliminary assessment: Suspicious activity requiring further investigation.**

The severity cannot be reliably determined from these records alone. Additional evidence, account context and the organisation's alerting criteria would be required.

## 7. Recommended Next Steps

1. Review authentication logs for successful logins after the failed attempts.
2. Check whether other accounts were targeted by the same source.
3. Review related events and determine whether the activity is expected.
4. Escalate according to the organisation's incident response procedures if suspicious activity is substantiated.

## 8. Conclusion

Repeated failed logins were identified in the simulated records. The pattern warrants further investigation, but there is insufficient evidence to confirm an account compromise.

## 9. Key Learnings

- Recognising repeated authentication failures.
- Distinguishing suspicious activity from a confirmed security incident.
- Identifying additional evidence needed for investigation.
- Documenting findings and recommending appropriate next steps.

## 10. Limitations

This was a manual exercise using fictional records. No live environment was accessed, no SIEM queries were executed, and no actual security incident was investigated.
