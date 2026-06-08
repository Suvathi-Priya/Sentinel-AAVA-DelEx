# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 9 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The 9 user stories form the baseline for evaluation, covering unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

## Test Coverage Summary

**Total User Stories:** 9

**Coverage Details:**

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 6 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 3 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

**Coverage Gap Details:**

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-002 | AC2 | No testcase explicitly validates that the resume date is included in the pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that the scheduled resume date is viewable in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that the pause start date is captured in the pause audit logs. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that the timestamp is captured in the pause audit logs. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that the pause is prevented from being activated before manager approval is complete. | Partially Covered |
| SCM-003 | AC5 | Manager approval workflow not initiated when price increase equals exactly 50% | Partially Covered |
| SCM-004 | AC2 | Applicable refund details not included in cancellation confirmation notification | Partially Covered |
| SCM-004 | AC5 | Finance team approval workflow fails to initiate for accounts with mixed currency outstanding balances | Partially Covered |
| SCM-005 | AC2 | Renewal amount not populated in 30-day reminder notification for monthly billing plans | Partially Covered |
| SCM-005 | AC5 | Account manager reminder not sent when subscription value exceeds threshold but account manager assignment is pending | Partially Covered |
| SCM-006 | AC2 | Adjusted billing amount not included in downgrade confirmation notification to customer | Partially Covered |
| SCM-007 | AC2 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint | Partially Covered |
| SCM-007 | AC5 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change | Partially Covered |

## Test Execution Summary

**Overall Test Execution Summary:**

Total Test Cases Executed: 131

Total Test Cases Passed: 108

Total Test Cases Failed: 23

**Test Execution Summary Details:**

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-002 | 15 | 15 | 13 | 2 |
| SCM-003 | 15 | 15 | 13 | 2 |
| SCM-004 | 15 | 15 | 13 | 2 |
| SCM-005 | 15 | 15 | 13 | 2 |
| SCM-006 | 14 | 14 | 13 | 1 |
| SCM-007 | 14 | 14 | 12 | 2 |
| ORM-001 | 15 | 15 | 12 | 3 |
| CLP-001 | 13 | 13 | 10 | 3 |
| CNS-001 | 15 | 15 | 12 | 3 |

## Consistency Analysis

**Data Mapping Inconsistency Details:**

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

**Consistency Metrics Summary:**

| Metric | Count |
|--------|-------|
| Total Test Cases | 131 |
| Total Test Logs | 131 |
| Missing Test Cases | 4 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 17.56%

**Defect Rate Analysis:**

Defect Rate = (Total Defects / Total Test Cases) × 100

**Description:**

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

**Components:**

Total Defects: Total number of defects identified during the test cycle

Total Test Cases: Total number of test cases executed

**Defect Details:**

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
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

## Conclusion

Remediation is required as test case failures and defects exist across multiple user stories, indicating outstanding coverage and execution issues that must be addressed before progression.