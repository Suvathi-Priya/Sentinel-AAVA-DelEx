# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

The baseline for evaluation consists of 1 user story with 5 acceptance criteria. The scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

**Total User Stories:** 1

## Coverage Details

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 0 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 1 | User stories where all acceptance criteria are Not Covered |

## Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---|---|---|---|
| CNS-001 | AC1 | No testcase explicitly validates sending email notifications for all completed transactions. | Not Covered |
| CNS-001 | AC2 | No testcase explicitly validates sending SMS notifications for high-priority alerts. | Not Covered |
| CNS-001 | AC3 | No testcase explicitly validates push notifications configurable per user preference. | Not Covered |
| CNS-001 | AC4 | No testcase explicitly validates capture of customer ID in notification logs. | Not Covered |
| CNS-001 | AC4 | No testcase explicitly validates capture of notification type in notification logs. | Not Covered |
| CNS-001 | AC4 | No testcase explicitly validates capture of timestamp in notification logs. | Not Covered |
| CNS-001 | AC5 | No testcase explicitly validates that failed notifications trigger retry attempts. | Not Covered |
| CNS-001 | AC5 | No testcase explicitly validates retry attempts up to 3 times. | Not Covered |

## Coverage Score

| User Story ID | Coverage Score | Color |
|---|---|---|
| CNS-001 | 0.00% | 🔴 Red |

## Legend

| Color | Coverage Range | Interpretation |
|---|---|---|
| 🟢 Green | 90–100% | High coverage (meets quality expectations) |
| 🟠 Amber | 70–89% | Moderate coverage (requires attention) |
| 🔴 Red | <70% | Low coverage (critical gaps present) |

## Formula Analysis for Coverage Score

### Formula

```text
Coverage Score (%) = (Fully Covered Acceptance Criteria for the User Story / Total Acceptance Criteria in the User Story) × 100
```

### Description

Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

### Components

| Component | Description |
|---|---|
| Covered Acceptance Criteria for the User Story | Number of acceptance criteria within the user story that have at least one mapped test case. |
| Total Acceptance Criteria in the User Story | Total number of acceptance criteria defined for that specific user story. |

### Calculation Scope

Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

## Test Execution Summary

## Overall Test Execution Summary

**Total Test Cases Executed:** 15

**Total Test Cases Passed:** 12

**Total Test Cases Failed:** 3

## Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| CNS-001 | 0 | 0 | 0 | 0 |

## Consistency Analysis

## Data Mapping Inconsistency Details

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

## Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 15 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 20.00%

## Defect Rate

20.00%

## Formula Analysis for Defect Rate

### Formula

```text
Defect Rate = (Total Defects / Total Test Cases) × 100
```

### Description

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

### Components

| Component | Description |
|---|---|
| Total Defects | Total number of defects identified during the test cycle |
| Total Test Cases | Total number of test cases executed |

## Defect Details

No defects are associated with the analyzed user story CNS-001 as no test cases are mapped to this user story.

## Conclusion

The report indicates that remediation is required as user story CNS-001 is Not Covered. Critical coverage gaps exist across all acceptance criteria, requiring immediate attention before progression.
