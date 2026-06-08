# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 8 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

Coverage Boundary: The total number of user stories included in the analysis is 8, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

Inclusions:
- Unit test cases linked to the identified user stories
- Test execution results (executed, not executed, passed, failed)
- Defect data directly associated with these user stories

Exclusions:
- Integration tests, system tests, or performance tests
- User stories not mapped to test cases

## Test Coverage Summary

Total User Stories: 8

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 8 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-002 | AC2 | No testcase explicitly validates that the resume date is included in the notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that the scheduled resume date is viewable in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that the pause start date is captured in the audit log. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that the timestamp is captured in the audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that the pause is blocked from activation before manager approval is granted. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates that the revised billing amount is included in the notification. Testcase TP_SCM3_005 failed for this reason. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that the subscription ID is captured in the audit log. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that the upgrade date is captured in the audit log. | Partially Covered |
| SCM-003 | AC5 | No testcase explicitly validates that the upgrade is blocked from activation before manager approval is granted. | Partially Covered |
| SCM-004 | AC2 | No testcase explicitly validates that applicable refund details are included in the notification. Testcase TP_SCM4_005 failed for this reason. | Partially Covered |
| SCM-004 | AC4 | No testcase explicitly validates that the effective date is captured in the audit log. | Partially Covered |
| SCM-006 | AC2 | No testcase explicitly validates that the adjusted billing amount is detailed in the notification. Testcase TP_SCM6_005 failed for this reason. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that the effective date is captured in the audit log. | Partially Covered |
| SCM-006 | AC5 | No testcase explicitly validates that processing is blocked until both approval and review are complete. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer details are included in the notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that the billing change summary is viewable in the customer portal. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that compliance team approval is required. Testcase TP_SCM7_014, which may have covered this, is missing. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that the transfer is blocked pending compliance approval. Testcase TP_SCM7_015, which may have covered this, is missing. | Partially Covered |
| CLP-001 | AC5 | No testcase explicitly validates that a fraud review is required. Testcase UT_CLP_014, which may have covered this, is missing. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates that the timestamp is captured in the notification log. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates that retry attempts are limited to 3 times. Testcase UT_CNS_014, which may have covered this, is missing. | Partially Covered |

## Test Execution Summary

Total Test Cases Executed: 108

Total Test Cases Passed: 91

Total Test Cases Failed: 17

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-002 | 15 | 15 | 13 | 2 |
| SCM-003 | 15 | 15 | 13 | 2 |
| SCM-004 | 15 | 15 | 13 | 2 |
| SCM-005 | 15 | 15 | 13 | 2 |
| SCM-006 | 15 | 13 | 12 | 1 |
| SCM-007 | 13 | 13 | 11 | 2 |
| CLP-001 | 13 | 13 | 10 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |

## Consistency Analysis

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| TP_SCM7_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_014 | SCM-007 | AC5 | High |
| TP_SCM7_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_015 | SCM-007 | AC5 | High |
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

| Metric | Count |
|--------|-------|
| Total Test Cases | 116 |
| Total Test Logs | 116 |
| Missing Test Cases | 4 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

Defect Rate: 12.50%

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:
Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:
- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM4-101 | TP_SCM4_005 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_014 | SCM-004 | Finance team approval workflow fails to initiate for accounts with mixed currency outstanding balances |
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-102 | TP_SCM5_015 | SCM-005 | Account manager reminder not sent when subscription value exceeds threshold but account manager assignment is pending |
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

## Conclusion

The report indicates outstanding coverage and execution issues based on the provided data that require remediation before progression. All 8 user stories contain partially covered acceptance criteria, 17 test cases have failed, and 14 defects have been identified across the test suite.
