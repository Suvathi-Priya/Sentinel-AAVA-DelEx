# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 9 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM8 | AC5 | No testcase explicitly validates fraud review requirement for redemptions above 5000 points. | Partially Covered |
| SCRUM-58 | AC2 | No testcase explicitly validates that transfer details are included in the notification. | Partially Covered |
| SCRUM-58 | AC3 | No testcase explicitly validates that billing change summary is viewable in the portal. | Partially Covered |
| SCRUM-58 | AC4 | No testcase explicitly validates that subscription ID is captured in the audit log.; No testcase explicitly validates that transfer date is captured in the audit log.; No testcase explicitly validates that timestamp is captured in the audit log. | Partially Covered |
| SCRUM-58 | AC5 | No testcase explicitly validates that change in billing entity requires compliance team approval. | Partially Covered |
| SCRUM-56 | AC2 | No testcase explicitly validates that adjusted billing amount is included in the downgrade confirmation notification. | Partially Covered |
| SCRUM-56 | AC4 | No testcase explicitly validates that previous plan is captured in the audit log.; No testcase explicitly validates that downgraded plan is captured in the audit log.; No testcase explicitly validates that effective date is captured in the audit log.; No testcase explicitly validates that credit issued is captured in the audit log.; No testcase explicitly validates that timestamp is captured in the audit log. | Partially Covered |
| SCRUM-56 | AC5 | No testcase explicitly validates that customer retention review is required for enterprise-tier plan downgrades. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| TP_SCM8_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_001. Test log attachment uses testcase ID UT_SCM8_001 instead of planned testcase ID TP_SCM8_001. | SCM8 | AC1 | High |
| TP_SCM8_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_002. Test log attachment uses testcase ID UT_SCM8_002 instead of planned testcase ID TP_SCM8_002. | SCM8 | AC1 | High |
| TP_SCM8_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_003. Test log attachment uses testcase ID UT_SCM8_003 instead of planned testcase ID TP_SCM8_003. | SCM8 | AC1 | High |
| TP_SCM8_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_004. Test log attachment uses testcase ID UT_SCM8_004 instead of planned testcase ID TP_SCM8_004. | SCM8 | AC2 | High |
| TP_SCM8_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_005. Test log attachment uses testcase ID UT_SCM8_005 instead of planned testcase ID TP_SCM8_005. | SCM8 | AC2 | High |
| TP_SCM8_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_006. Test log attachment uses testcase ID UT_SCM8_006 instead of planned testcase ID TP_SCM8_006. | SCM8 | AC3 | High |
| TP_SCM8_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_007. Test log attachment uses testcase ID UT_SCM8_007 instead of planned testcase ID TP_SCM8_007. | SCM8 | AC3 | High |
| TP_SCM8_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_008. Test log attachment uses testcase ID UT_SCM8_008 instead of planned testcase ID TP_SCM8_008. | SCM8 | AC4 | High |
| TP_SCM8_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_009. Test log attachment uses testcase ID UT_SCM8_009 instead of planned testcase ID TP_SCM8_009. | SCM8 | AC5 | High |
| TP_SCM8_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_010. Test log attachment uses testcase ID UT_SCM8_010 instead of planned testcase ID TP_SCM8_010. | SCM8 | AC1 | High |
| TP_SCM8_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_011. Test log attachment uses testcase ID UT_SCM8_011 instead of planned testcase ID TP_SCM8_011. | SCM8 | AC2 | High |
| TP_SCM8_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_012. Test log attachment uses testcase ID UT_SCM8_012 instead of planned testcase ID TP_SCM8_012. | SCM8 | AC4 | High |
| TP_SCM8_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_013. Test log attachment uses testcase ID UT_SCM8_013 instead of planned testcase ID TP_SCM8_013. | SCM8 | AC5 | High |
| TP_SCM8_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_014. Test log attachment uses testcase ID UT_SCM8_014 instead of planned testcase ID TP_SCM8_014. | SCM8 | AC2 | High |
| TP_SCM8_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_015. Test log attachment uses testcase ID UT_SCM8_015 instead of planned testcase ID TP_SCM8_015. | SCM8 | AC5 | High |
| UT_SCM8_001 | missing_testcase | Execution record exists for testcase ID UT_SCM8_001 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_001. | SCM8 | AC1 | High |
| UT_SCM8_002 | missing_testcase | Execution record exists for testcase ID UT_SCM8_002 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_002. | SCM8 | AC1 | High |
| UT_SCM8_003 | missing_testcase | Execution record exists for testcase ID UT_SCM8_003 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_003. | SCM8 | AC1 | High |
| UT_SCM8_004 | missing_testcase | Execution record exists for testcase ID UT_SCM8_004 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_004. | SCM8 | AC2 | High |
| UT_SCM8_005 | missing_testcase | Execution record exists for testcase ID UT_SCM8_005 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_005. | SCM8 | AC2 | High |
| UT_SCM8_006 | missing_testcase | Execution record exists for testcase ID UT_SCM8_006 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_006. | SCM8 | AC3 | High |
| UT_SCM8_007 | missing_testcase | Execution record exists for testcase ID UT_SCM8_007 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_007. | SCM8 | AC3 | High |
| UT_SCM8_008 | missing_testcase | Execution record exists for testcase ID UT_SCM8_008 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_008. | SCM8 | AC4 | High |
| UT_SCM8_009 | missing_testcase | Execution record exists for testcase ID UT_SCM8_009 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_009. | SCM8 | AC5 | High |
| UT_SCM8_010 | missing_testcase | Execution record exists for testcase ID UT_SCM8_010 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_010. | SCM8 | AC1 | High |
| UT_SCM8_011 | missing_testcase | Execution record exists for testcase ID UT_SCM8_011 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_011. | SCM8 | AC2 | High |
| UT_SCM8_012 | missing_testcase | Execution record exists for testcase ID UT_SCM8_012 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_012. | SCM8 | AC4 | High |
| UT_SCM8_013 | missing_testcase | Execution record exists for testcase ID UT_SCM8_013 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_013. | SCM8 | AC5 | High |
| UT_SCM8_014 | missing_testcase | Execution record exists for testcase ID UT_SCM8_014 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_014. | SCM8 | AC2 | High |
| UT_SCM8_015 | missing_testcase | Execution record exists for testcase ID UT_SCM8_015 but no corresponding testcase ID exists in the Test Plan. Planned testcase appears to be TP_SCM8_015. | SCM8 | AC5 | High |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014. | SCRUM-52 | AC2 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015. | SCRUM-52 | AC5 | Medium |
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014. | SCRUM-50 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015. | SCRUM-50 | AC5 | Medium |
| SCM-008_Test_Log_upd.xlsx | invalid_mapping | Test Plan and Test Log for SCM-008 use inconsistent testcase ID prefixes (TP_ in plan vs UT_ in log), causing traceability mismatch across all 15 records. | SCM8 |  | High |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| total_testcases | 135 |
| total_testlogs | 133 |
| consistency_status | Mismatch Detected |
| missing_testlogs | 19 |
| missing_testcases | 15 |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM9-001 | UT_SCM9_004 | SCM9 | SMS gateway timeout prevents delivery |
| DEF-SCM9-002 | UT_SCM9_012 | SCM9 | Push notification service ignores user preference flag |
| DEF-SCM7-101 | TP_SCM7_005 | SCRUM-58 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-101 | TP_SCM7_015 | SCRUM-58 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCRUM-58 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCRUM-58 | Audit log authorization reference field empty when transfer initiated via bulk admin API |
| DEF-SCM6-101 | TP_SCM6_005 | SCRUM-56 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCRUM-56 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCRUM-56 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |

## Conclusion

Remediation is required as multiple user stories have coverage gaps and defects exist in the test execution results.
