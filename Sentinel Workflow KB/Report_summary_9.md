# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The 3 user stories form the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates that adjusted billing amount is included in downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that effective date is captured in downgrade audit logs. | Partially Covered |
| SCM-007 | AC1 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC1 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC1 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC1 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC2 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC2 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC2 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC2 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC2 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| SCM-007 | AC3 | No testcase explicitly validates that outgoing owner can view ownership history in the customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that incoming owner can view ownership history in the customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that incoming owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that compliance team approval is required before the transfer is completed. | Partially Covered |
| CNS-001 | AC1 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| CNS-001 | AC2 | No testcase definition available in test plan for mapped testcases. | Not Covered |
| CNS-001 | AC3 | No testcase explicitly validates that push notifications are configurable per user preference. | Not Covered |
| CNS-001 | AC4 | No testcase explicitly validates that timestamp is captured in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates that retry attempts are limited to 3 times. | Partially Covered |

## Test Execution Summary

| Metric | Value |
|--------|-------|
| Total Test Cases in All Test Plan | 29 |
| Total Test Cases in All Test Logs | 41 |
| Total Passed in All Test Logs | 37 |
| Total Failed in All Test Logs | 4 |
| Total Defects in All Test Logs | 5 |
| Overall Defect Rate Percentage | 17.24 |
| Overall Defect Rate Formula | (Total Defects / Total Test Cases) × 100 |
| Overall Defect Rate Calculation | (5 / 29) × 100 = 17.24 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| TP_SCM7_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_001 | SCM-007 | AC1 | High |
| TP_SCM7_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_002 | SCM-007 | AC1 | High |
| TP_SCM7_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_003 | SCM-007 | AC1 | High |
| TP_SCM7_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_004 | SCM-007 | AC2 | High |
| TP_SCM7_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_005 | SCM-007 | AC2 | High |
| TP_SCM7_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_006 | SCM-007 | AC2 | High |
| TP_SCM7_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_014 | SCM-007 | AC5 | High |
| TP_SCM7_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_015 | SCM-007 | AC5 | High |
| UT_CNS_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_001 | CNS-001 | AC1 | High |
| UT_CNS_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_002 | CNS-001 | AC1 | High |
| UT_CNS_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_003 | CNS-001 | AC1 | High |
| UT_CNS_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_004 | CNS-001 | AC2 | High |
| UT_CNS_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_005 | CNS-001 | AC2 | High |
| UT_CNS_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_006 | CNS-001 | AC2 | High |
| UT_CNS_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_007 | CNS-001 | AC3 | High |
| UT_CNS_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_008 | CNS-001 | AC3 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 29 |
| Total Test Logs | 41 |
| Missing Test Cases | 16 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|--------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

## Conclusion

Remediation is required as multiple user stories have Not Covered acceptance criteria and defects exist in the test execution results.
