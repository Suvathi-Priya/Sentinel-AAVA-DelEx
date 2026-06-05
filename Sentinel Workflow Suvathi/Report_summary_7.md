# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 2, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

**Inclusions:** Unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

**Exclusions:** Integration tests, system tests, performance tests, and user stories not mapped to test cases.

## Test Coverage Summary

**Overall Coverage Score:** 60.00%

## Formula Analysis for Overall Coverage Score

**Metric Value:** 60.00%

**Formula:** (fully_covered_acceptance_criterias_in_all_user_stories / total_acceptance_criterias_in_all_user_stories) × 100

**Description:** Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

**Components:**
- fully_covered_acceptance_criterias_in_all_user_stories: 6
- total_acceptance_criterias_in_all_user_stories: 10

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| CLP-001 | AC5 | No testcase explicitly validates fraud review requirement. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times. | Partially Covered |

### Coverage Score

| User Story ID | Coverage Score | Color Indicator |
|---|---|---|
| CLP-001 | 60.00% | 🔴 Red |
| CNS-001 | 60.00% | 🔴 Red |

## Test Execution Summary

### Overall Test Execution Summary

| Metric | Value |
|---|---|
| Total Test Cases in All Test Plan | 28 |
| Total Test Cases in All Test Logs | 28 |
| Total Passed in All Test Logs | 22 |
| Total Failed in All Test Logs | 6 |

### Test Execution Summary

| User Story ID | Total Test Cases in Test Plan | Total Test Cases in Test Logs | Total Passed | Total Failed |
|---|---|---|---|---|
| CLP-001 | 13 | 15 | 11 | 4 |
| CNS-001 | 15 | 13 | 10 | 3 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID |
|---|---|---|---|
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 28 |
| Total Test Logs | 28 |
| Consistency Status | Mismatch Detected |
| Missing Test Logs | 2 |
| Missing Test Cases | 2 |

## Defect Details

**Defect Rate:** 21.43%

## Formula Analysis for Defect Rate

**Metric Value:** 21.43%

**Formula:** (total_defects_in_all_test_logs / total_test_cases_in_all_test_plan) × 100

**Components:**
- total_defects_in_all_test_logs: 6
- total_test_cases_in_all_test_plan: 28

### Defect Details

| Defect ID | Test Case ID | Defect Description | User Story ID | AC ID |
|---|---|---|---|---|
| DEF-CLP-001 | UT_CLP_003 | Points posting service delay | CLP-001 | AC1 |
| DEF-CLP-002 | UT_CLP_008 | Balance refresh cache issue | CLP-001 | AC3 |
| DEF-CLP-003 | UT_CLP_015 | Redemption workflow synchronization issue | CLP-001 | AC5 |
| DEF-CNS-001 | UT_CNS_004 | SMS gateway timeout prevents delivery | CNS-001 | AC2 |
| DEF-CNS-002 | UT_CNS_006 | SMS tracking service failed to update status | CNS-001 | AC2 |
| DEF-CNS-003 | UT_CNS_009 | Push notification service unavailable | CNS-001 | AC3 |

## Conclusion

Remediation is required as both user stories have Partially Covered acceptance criteria, test case failures are present, and defects exist in the system.
