<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-003 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

# Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-003 | AC1 | No testcase explicitly validates submission of a subscription upgrade request.; No testcase explicitly validates specifying the target plan.; No testcase explicitly validates specifying the preferred upgrade date. | Not Covered |
| SCM-003 | AC2 | No testcase explicitly validates sending upgrade confirmation notifications to customers.; No testcase explicitly validates including the new plan details in the notification.; No testcase explicitly validates including the effective date in the notification.; No testcase explicitly validates including the revised billing amount in the notification. | Not Covered |
| SCM-003 | AC3 | No testcase explicitly validates viewing upgrade request status in the customer portal.; No testcase explicitly validates viewing upgrade history in the customer portal.; No testcase explicitly validates viewing next billing cycle changes in the customer portal. | Not Covered |
| SCM-003 | AC4 | No testcase explicitly validates capture of customer ID in upgrade audit logs.; No testcase explicitly validates capture of subscription ID in upgrade audit logs.; No testcase explicitly validates capture of previous plan in upgrade audit logs.; No testcase explicitly validates capture of new plan in upgrade audit logs.; No testcase explicitly validates capture of upgrade date in upgrade audit logs.; No testcase explicitly validates capture of timestamp in upgrade audit logs. | Not Covered |
| SCM-003 | AC5 | No testcase explicitly validates price increase greater than 50%.; No testcase explicitly validates manager approval requirement before upgrade activation. | Not Covered |

# Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| TP_SCM_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_001 | SCM-002 | AC1 | Medium |
| TP_SCM_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_002 | SCM-002 | AC1 | Medium |
| TP_SCM_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_003 | SCM-002 | AC1 | Medium |
| TP_SCM_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_004 | SCM-002 | AC2 | Medium |
| TP_SCM_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_005 | SCM-002 | AC2 | Medium |
| TP_SCM_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_006 | SCM-002 | AC3 | Medium |
| TP_SCM_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_007 | SCM-002 | AC3 | Medium |
| TP_SCM_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_008 | SCM-002 | AC4 | Medium |
| TP_SCM_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_009 | SCM-002 | AC5 | Medium |
| TP_SCM_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_010 | SCM-002 | AC1 | Medium |
| TP_SCM_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_011 | SCM-002 | AC2 | Medium |
| TP_SCM_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_012 | SCM-002 | AC4 | Medium |
| TP_SCM_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_013 | SCM-002 | AC5 | Medium |
| TP_SCM_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_014 | SCM-002 | AC1 | Medium |
| TP_SCM_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_015 | SCM-002 | AC5 | Medium |
| UT_SCM1_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_001 | NULL | AC1 | High |
| UT_SCM1_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_002 | NULL | AC1 | High |
| UT_SCM1_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_003 | NULL | AC1 | High |
| UT_SCM1_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_004 | NULL | AC2 | High |
| UT_SCM1_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_005 | NULL | AC2 | High |
| UT_SCM1_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_006 | NULL | AC3 | High |
| UT_SCM1_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_007 | NULL | AC3 | High |
| UT_SCM1_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_008 | NULL | AC4 | High |
| UT_SCM1_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_009 | NULL | AC5 | High |
| UT_SCM1_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_010 | NULL | AC1 | High |
| UT_SCM1_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_011 | NULL | AC2 | High |
| UT_SCM1_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_012 | NULL | AC4 | High |
| UT_SCM1_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_013 | NULL | AC5 | High |
| UT_SCM1_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_014 | NULL | AC2 | High |
| UT_SCM1_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM1_015 | NULL | AC5 | High |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 15 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

# Defect Details

No defects reported for this User Story.

# Conclusion

Remediation is required as user story SCM-003 is Not Covered.
