# SOC Lab 02: Suspected Account Compromise Investigation

## 1. Overview
- **Category:** SOC / Blue Team
- **Lab type:** Simulated investigation
- **Difficulty:** Beginner
- **Status:** Escalation recommended
- **Tools:** Manual log analysis
- **Data source:** Fictional training records

## 2. Objective
Investigate repeated failed login attempts followed by a successful login and suspicious administrative activity to determine the appropriate SOC response.

## 3. Scenario
A security alert identified three failed login attempts against the `admin` account, followed by a successful login from the same unfamiliar source IP. Subsequent events showed administrative privileges being used and sensitive settings being accessed.

The account user confirmed that they did not authorise the activity.

## 4. Evidence and Timeline

| Time | Event |
|---|---|
| 10:15 | Failed login for `admin` |
| 10:16 | Failed login for `admin` |
| 10:17 | Failed login for `admin` |
| 10:18 | Successful login |
| 10:19 | Administrative privileges used |
| 10:20 | Sensitive settings accessed |

- **Source IP:** `192.0.2.20`
- **Account:** `admin`
- **User confirmation:** Activity was unauthorised.

*Note: All records are fictional. The IP address belongs to a range reserved for documentation and examples.*

## 5. Investigation and Analysis

1. Identified three consecutive failed login attempts against the same account.
2. Observed a successful login immediately after the failed attempts.
3. Identified subsequent administrative activity and access to sensitive settings.
4. Checked whether the activity was authorised.
5. The user denied performing the activity.

The sequence is consistent with a possible account compromise. However, the available evidence does not establish the precise attack method or identify who performed the activity.

## 6. Risk Assessment

**Assessment:** Suspected account compromise requiring urgent investigation and escalation.

The combination of unauthorised access and sensitive administrative activity creates a potential risk to the affected system.

A formal severity rating should be assigned according to the organisation's incident classification criteria and the impact confirmed during further investigation.

## 7. Recommended Response

1. Escalate the alert to the authorised incident-response team.
2. Preserve relevant authentication and administrative audit logs.
3. Review active sessions and subsequent activity associated with the account.
4. Follow approved procedures to contain the suspected compromise, such as revoking sessions or resetting credentials.
5. Investigate whether additional accounts or systems were affected.
6. Document response actions and update the incident record.

## 8. Conclusion

The investigation identified repeated failed logins followed by a successful login and unauthorised administrative activity. The available evidence supports escalating the case as a suspected account compromise.

Further investigation is required to establish the attack method, scope and impact.

## 9. Key Learnings

- Recognising suspicious authentication patterns.
- Investigating activity after a successful login.
- Correlating events to establish a timeline.
- Verifying activity with the account owner.
- Escalating suspected incidents appropriately.
- Writing evidence-based incident summaries without unsupported claims.

## 10. Limitations

This was a simulated beginner exercise using fictional records. No live system was accessed, no SIEM queries were executed, and no actual incident was investigated. The findings are limited to the scenario provided.
