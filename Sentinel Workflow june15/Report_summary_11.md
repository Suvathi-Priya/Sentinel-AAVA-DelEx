# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 7 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-001 | AC5 | No testcase explicitly validates fraud review requirement for high-value refunds. | Partially Covered |

## Consistency Analysis

Data Mapping Inconsistency Details:

## Data Mapping Inconsistency Details

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
| TP_SCM2_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_001 | NULL | NULL | High |
| TP_SCM2_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_002 | NULL | NULL | High |
| TP_SCM2_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_003 | NULL | NULL | High |
| TP_SCM2_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_004 | NULL | NULL | High |
| TP_SCM2_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_005 | NULL | NULL | High |
| TP_SCM2_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_006 | NULL | NULL | High |
| TP_SCM2_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_007 | NULL | NULL | High |
| TP_SCM2_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_008 | NULL | NULL | High |
| TP_SCM2_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_009 | NULL | NULL | High |
| TP_SCM2_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_010 | NULL | NULL | High |
| TP_SCM2_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_011 | NULL | NULL | High |
| TP_SCM2_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_012 | NULL | NULL | High |
| TP_SCM2_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_013 | NULL | NULL | High |
| TP_SCM2_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_014 | NULL | NULL | High |
| TP_SCM2_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_015 | NULL | NULL | High |
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC2 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | Medium |

## Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 105 |
| Total Test Logs | 101 |
| Missing Test Cases | 15 |
| Missing Test Logs | 19 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM1-001 | UT_SCM1_005 | SCM-001 | Notification template rendering issue |
| DEF-SCM1-002 | UT_SCM1_009 | SCM-001 | Refund workflow synchronization error |
| DEF-SCM2-101 | TP_SCM2_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM2-102 | TP_SCM2_009 | SCM-002 | Activation allowed without completed approval |
| DEF-SCM3-101 | TP_SCM3_004 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM4-101 | TP_SCM4_004 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_009 | SCM-004 | Finance team approval workflow fails for mixed currency outstanding balances |
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-103 | TP_SCM5_011 | SCM-005 | System sends reminder even when subscription expiry date is null |
| DEF-SCM5-104 | TP_SCM5_013 | SCM-005 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |
| DEF-SCM5-105 | TP_SCM5_015 | SCM-005 | Reminder log delivery status remains blank when notification channel fails |
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCM-006 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCM-006 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCM-007 | Audit log authorization reference field empty when transfer initiated via bulk admin API |

## Conclusion

Remediation is required as test case failures and defects exist across multiple user stories.
