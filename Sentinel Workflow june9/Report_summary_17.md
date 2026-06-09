# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story CNS-001 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

## Test Coverage Summary

| User Story ID | Title | Total Acceptance Criteria | Fully Covered Acceptance Criteria | Partially Covered Acceptance Criteria | Not Covered Acceptance Criteria | Coverage Score Percentage |
|---|---|---:|---:|---:|---:|---:|
| CNS-001 | Implement Customer Notification Service | 5 | 0 | 0 | 5 | 0.00 |

| Metric | Value |
|---|---|
| Total User Stories | 1 |
| Total Fully Covered User Stories | 0 |
| Total Partially Covered User Stories | 0 |
| Total Not Covered User Stories | 1 |
| Total Acceptance Criterias in All User Stories | 5 |
| Fully Covered Acceptance Criterias in All User Stories | 0 |
| Partially Covered Acceptance Criterias in All User Stories | 0 |
| Not Covered Acceptance Criterias in All User Stories | 5 |
| Overall Coverage Score Percentage | 0.00 |
| Overall Coverage Score Formula | (Fully Covered Acceptance Criteria in All User Stories / Total Acceptance Criteria in All User Stories) × 100 |
| Overall Coverage Score Calculation | (0 / 5) × 100 = 0.00 |
| Total Test Cases in All Test Plan | 0 |
| Total Test Cases in All Test Logs | 0 |
| Total Passed in All Test Logs | 0 |
| Total Failed in All Test Logs | 0 |
| Total Defects in All Test Logs | 0 |
| Overall Defect Rate Percentage | 0.00 |
| Overall Defect Rate Formula | (Total Defects / Total Test Cases) × 100 |
| Overall Defect Rate Calculation | (0 / 0) × 100 = 0.00 |

### Coverage Gap Details

| User Story ID | AC ID | Requirement ID | Missing Requirement | Gap Reason | Coverage Status |
|---|---|---|---|---|---|
| CNS-001 | AC1 | CNS-001-AC1-REQ-001 | send email notifications for all completed transactions | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC2 | CNS-001-AC2-REQ-001 | send SMS notifications for high-priority alerts | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC3 | CNS-001-AC3-REQ-001 | push notifications configurable per user preference | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC4 | CNS-001-AC4-REQ-001 | capture customer ID | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC4 | CNS-001-AC4-REQ-002 | capture notification type | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC4 | CNS-001-AC4-REQ-003 | capture timestamp | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC5 | CNS-001-AC5-REQ-001 | failed notifications trigger retry attempts | No testcase is mapped to this acceptance criterion. | Not Covered |
| CNS-001 | AC5 | CNS-001-AC5-REQ-002 | retry attempts up to 3 times | No testcase is mapped to this acceptance criterion. | Not Covered |

## Test Execution Summary

| Test Case ID | Acceptance Criteria ID | Status | Actual Result | Defect Details & Description |
|---|---|---|---|---|
| UT_CLP_001 | AC1 | Passed | Points awarded successfully | NaN |
| UT_CLP_002 | AC1 | Passed | Correct points calculated | NaN |
| UT_CLP_003 | AC1 | Failed | Points posting delayed | DEF-CLP-001 - Points posting service delay |
| UT_CLP_004 | AC2 | Passed | Reward redeemed successfully | NaN |
| UT_CLP_005 | AC2 | Passed | Points deducted correctly | NaN |
| UT_CLP_006 | AC2 | Passed | Reward issued successfully | NaN |
| UT_CLP_007 | AC3 | Passed | Balance displayed correctly | NaN |
| UT_CLP_008 | AC3 | Failed | Balance refresh issue observed | DEF-CLP-002 - Balance refresh cache issue |
| UT_CLP_009 | AC3 | Passed | Balance updated after redemption | NaN |
| UT_CLP_010 | AC4 | Passed | Customer ID logged | NaN |
| UT_CLP_011 | AC4 | Passed | Points value logged | NaN |
| UT_CLP_012 | AC4 | Passed | Timestamp logged | NaN |
| UT_CLP_013 | AC5 | Passed | Manager approval validated | NaN |
| UT_CLP_014 | AC5 | Passed | Fraud review validated | NaN |
| UT_CLP_015 | AC5 | Failed | High value workflow validation failed | DEF-CLP-003 - Redemption workflow synchronization issue |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_ORM_001 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_001 | ORM-001 | AC1 | Medium |
| UT_ORM_002 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_002 | ORM-001 | AC1 | Medium |
| UT_ORM_003 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_003 | ORM-001 | AC1 | Medium |
| UT_ORM_004 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_004 | ORM-001 | AC2 | Medium |
| UT_ORM_005 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_005 | ORM-001 | AC2 | Medium |
| UT_ORM_006 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_006 | ORM-001 | AC2 | Medium |
| UT_ORM_007 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_007 | ORM-001 | AC3 | Medium |
| UT_ORM_008 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_008 | ORM-001 | AC3 | Medium |
| UT_ORM_009 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_009 | ORM-001 | AC3 | Medium |
| UT_ORM_010 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_010 | ORM-001 | AC4 | Medium |
| UT_ORM_011 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_011 | ORM-001 | AC4 | Medium |
| UT_ORM_012 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_012 | ORM-001 | AC4 | Medium |
| UT_ORM_013 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_013 | ORM-001 | AC5 | Medium |
| UT_ORM_014 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_014 | ORM-001 | AC5 | Medium |
| UT_ORM_015 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_015 | ORM-001 | AC5 | Medium |
| UT_CLP_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_001 |  | AC1 | High |
| UT_CLP_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_002 |  | AC1 | High |
| UT_CLP_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_003 |  | AC1 | High |
| UT_CLP_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_004 |  | AC2 | High |
| UT_CLP_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_005 |  | AC2 | High |
| UT_CLP_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_006 |  | AC2 | High |
| UT_CLP_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_007 |  | AC3 | High |
| UT_CLP_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_008 |  | AC3 | High |
| UT_CLP_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_009 |  | AC3 | High |
| UT_CLP_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_010 |  | AC4 | High |
| UT_CLP_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_011 |  | AC4 | High |
| UT_CLP_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_012 |  | AC4 | High |
| UT_CLP_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_013 |  | AC5 | High |
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 |  | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 |  | AC5 | High |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 15 |
| Missing Test Logs | 15 |
| Extra Test Cases | 0 |
| Extra Test Logs | 0 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Test Case ID | Defect ID | Defect Description |
|---|---|---|
| UT_CLP_003 | DEF-CLP-001 | Points posting service delay |
| UT_CLP_008 | DEF-CLP-002 | Balance refresh cache issue |
| UT_CLP_015 | DEF-CLP-003 | Redemption workflow synchronization issue |

## Conclusion

Remediation is required as user story CNS-001 is Not Covered. The unit test suite requires immediate attention to address coverage gaps and mapping inconsistencies before progression.
