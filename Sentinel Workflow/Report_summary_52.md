# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 5 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log.; No testcase explicitly validates timestamp capture in audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that approval is required before pause activation. | Partially Covered |
| ORM-001 | AC4 | No testcase explicitly validates approval timestamp capture in audit log. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold for high-value refunds. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates revised billing amount inclusion in notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates subscription ID capture in upgrade audit log.; No testcase explicitly validates upgrade date capture in upgrade audit log. | Partially Covered |
| SCM-003 | AC5 | No testcase explicitly validates that approval is required before upgrade activation. | Partially Covered |
| CLP-001 | AC5 | No testcase explicitly validates fraud review requirement for high-value redemptions. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times. | Partially Covered |

## Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 73

**Total Test Cases Passed:** 59

**Total Test Cases Failed:** 14

### Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| SCM-002 | 15 | 15 | 13 | 2 |
| ORM-001 | 15 | 15 | 12 | 3 |
| SCM-003 | 15 | 15 | 13 | 2 |
| CLP-001 | 13 | 15 | 11 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 73 |
| Total Test Logs | 73 |
| Missing Test Cases | 2 |
| Missing Test Logs | 2 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

## Conclusion

Remediation is required as multiple user stories have partial coverage gaps and 14 test cases have failed with associated defects identified.
