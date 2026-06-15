<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-004 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

# Test Coverage Summary

## Coverage Gap Details

| **User Story ID** | **AC ID** | **Coverage Gap Reason** | **Coverage Status** |
|---|---|---|---|
| SCM-004 | AC1 | No testcase explicitly validates submission of a cancellation request.; No testcase explicitly validates specifying the cancellation reason.; No testcase explicitly validates specifying preferred cancellation date. | Not Covered |
| SCM-004 | AC2 | No testcase explicitly validates sending cancellation confirmation notifications to customers.; No testcase explicitly validates including the effective cancellation date in notifications.; No testcase explicitly validates including any applicable refund details in notifications. | Not Covered |
| SCM-004 | AC3 | No testcase explicitly validates viewing cancellation request status in the customer portal.; No testcase explicitly validates viewing refund status in the customer portal.; No testcase explicitly validates viewing service end date in the customer portal. | Not Covered |
| SCM-004 | AC4 | No testcase explicitly validates capture of customer ID in cancellation audit logs.; No testcase explicitly validates capture of subscription ID in cancellation audit logs.; No testcase explicitly validates capture of cancellation reason in cancellation audit logs.; No testcase explicitly validates capture of effective date in cancellation audit logs.; No testcase explicitly validates capture of refund amount in cancellation audit logs.; No testcase explicitly validates capture of timestamp in cancellation audit logs. | Not Covered |
| SCM-004 | AC5 | No testcase explicitly validates cancellation requests with outstanding balances greater than $500.; No testcase explicitly validates requirement for finance team approval before the cancellation is processed. | Not Covered |

# Consistency Analysis

## Data Mapping Inconsistency Details

| **Test Case ID** | **Consistency Type** | **Description** | **User Story ID** | **AC ID** | **Impact Level** |
|---|---|---|---|---|---|
| TP_SCM3_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_001 | SCM-003 | AC1 | Medium |
| TP_SCM3_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_002 | SCM-003 | AC1 | Medium |
| TP_SCM3_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_003 | SCM-003 | AC2 | Medium |
| TP_SCM3_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_004 | SCM-003 | AC2 | Medium |
| TP_SCM3_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_005 | SCM-003 | AC2 | Medium |
| TP_SCM3_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_006 | SCM-003 | AC3 | Medium |
| TP_SCM3_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_007 | SCM-003 | AC3 | Medium |
| TP_SCM3_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_008 | SCM-003 | AC4 | Medium |
| TP_SCM3_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_009 | SCM-003 | AC5 | Medium |
| TP_SCM3_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_010 | SCM-003 | AC1 | Medium |
| TP_SCM3_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_011 | SCM-003 | AC2 | Medium |
| TP_SCM3_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_012 | SCM-003 | AC4 | Medium |
| TP_SCM3_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_013 | SCM-003 | AC5 | Medium |
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |
| TP_SCM_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_001 | SCM-002 | AC1 | High |
| TP_SCM_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_002 | SCM-002 | AC1 | High |
| TP_SCM_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_003 | SCM-002 | AC1 | High |
| TP_SCM_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_004 | SCM-002 | AC2 | High |
| TP_SCM_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_005 | SCM-002 | AC2 | High |
| TP_SCM_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_006 | SCM-002 | AC3 | High |
| TP_SCM_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_007 | SCM-002 | AC3 | High |
| TP_SCM_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_008 | SCM-002 | AC4 | High |
| TP_SCM_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_009 | SCM-002 | AC5 | High |
| TP_SCM_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_010 | SCM-002 | AC1 | High |
| TP_SCM_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_011 | SCM-002 | AC2 | High |
| TP_SCM_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_012 | SCM-002 | AC4 | High |
| TP_SCM_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_013 | SCM-002 | AC5 | High |
| TP_SCM_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_014 | SCM-002 | AC1 | High |
| TP_SCM_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM_015 | SCM-002 | AC5 | High |

## Consistency Metrics Summary

| **Metric** | **Count** |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 15 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

# Defect Details

No defects reported for this User Story.

# Conclusion

Remediation is required as user story SCM-004 is Not Covered.
