# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 2

The baseline for this analysis consists of 2 user stories that form the reference for measuring coverage, execution success, and defect quality. The scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

**Overall Coverage Score:** 70.0%

### Formula Analysis for Overall Coverage Score

**Formula:** `(fully_covered_acceptance_criterias_in_all_user_stories / total_acceptance_criterias_in_all_user_stories) × 100`

**Calculation:** `(7 / 10) × 100 = 70.00`

**Coverage Gap Details**

| User Story ID | AC ID | Missing Requirement | Gap Reason | Coverage Status |
|---|---|---|---|---|
| CLP-001 | AC5 | require fraud review | No testcase explicitly validates fraud review requirement. | Partially Covered |
| CNS-001 | AC4 | capture timestamp | No testcase explicitly validates timestamp capture. | Partially Covered |
| CNS-001 | AC5 | retry attempts up to 3 times | No testcase explicitly validates the retry limit of 3 times. | Partially Covered |

**Coverage Score**

| User Story ID | Title | Coverage Score | Icon Rendering Instruction for Coverage Colors |
|---|---|---|---|
| CLP-001 | Implement Customer Loyalty Points Service | 80.0% | 🟠 Amber |
| CNS-001 | Implement Customer Notification Service | 60.0% | 🔴 Red |

## Test Execution Summary

| Scope | Total Test Cases in All Test Plan | Total Test Cases in All Test Logs | Total Passed in All Test Logs | Total Failed in All Test Logs |
|---|---:|---:|---:|---:|
| Overall | 28 | 28 | 22 | 6 |

| User Story ID | Total Test Cases in Test Plan | Total Test Cases in Test Logs | Total Passed | Total Failed |
|---|---:|---:|---:|---:|
| CLP-001 | 13 | 15 | 12 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |

## Consistency Analysis

**Data Mapping Inconsistency Details**

| Testcase ID | Consistency Type | Description | Mapped User Story ID |
|---|---|---|---|
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 |

**Consistency Metrics Summary**

| Metric | Value |
|---|---|
| Total Testcases | 28 |
| Total Testlogs | 28 |
| Consistency Status | Mismatch Detected |
| Missing Testlogs | 2 |
| Missing Testcases | 2 |

## Defect Details

**Defect Rate:** 17.86%

### Formula Analysis for Defect Rate

**Formula:** `(total_defects_in_all_test_logs / total_test_cases_in_all_test_plan) × 100`

**Calculation:** `(5 / 28) × 100 = 17.86`

| Defect ID | Testcase ID | Defect Description | User Story ID | AC ID |
|---|---|---|---|---|
| DEF-CLP-001 | UT_CLP_003 | Points posting service delay | CLP-001 | AC1 |
| DEF-CLP-002 | UT_CLP_008 | Balance refresh cache issue | CLP-001 | AC3 |
| DEF-CNS-001 | UT_CNS_004 | SMS gateway timeout prevents delivery | CNS-001 | AC2 |
| DEF-CNS-002 | UT_CNS_006 | SMS tracking service failed to update status | CNS-001 | AC2 |
| DEF-CNS-003 | UT_CNS_009 | Push notification service unavailable | CNS-001 | AC3 |

## Conclusion

Remediation is required as test case failures and defects exist in the current test execution results.
