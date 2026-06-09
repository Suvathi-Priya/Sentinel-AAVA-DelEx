# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 5 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 5, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

**Total User Stories:** 5

## Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 1 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 4 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

## Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---------------|-------|---------------------|-----------------|
| CLP-001 | AC5 | No testcase explicitly validates fraud review requirement. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times. | Partially Covered |
| ORM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates revised billing amount inclusion in notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates subscription ID capture. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates upgrade date capture. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates timestamp capture in audit log. | Partially Covered |

## Coverage Score

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| CLP-001 | 80.00% | 🟠 Amber |
| CNS-001 | 60.00% | 🔴 Red |
| ORM-001 | 60.00% | 🔴 Red |
| SCM-003 | 60.00% | 🔴 Red |
| SCM-002 | 60.00% | 🔴 Red |

## Legend

| Color | Coverage Range | Interpretation |
|-------|----------------|----------------|
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
|-----------|-------------|
| Covered Acceptance Criteria for the User Story | Number of acceptance criteria within the user story that have at least one mapped test case. |
| Total Acceptance Criteria in the User Story | Total number of acceptance criteria defined for that specific user story. |

### Calculation Scope

Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

## Test Execution Summary

## Overall Test Execution Summary

**Total Test Cases Executed:** 70

**Total Test Cases Passed:** 56

**Total Test Cases Failed:** 14

## Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| CLP-001 | 13 | 15 | 12 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |
| ORM-001 | 15 | 15 | 12 | 3 |
| SCM-003 | 15 | 15 | 13 | 2 |
| SCM-002 | 15 | 15 | 13 | 2 |

## Consistency Analysis

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| UT_CLP_013 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_013 | CLP-001 | AC5 | Medium |
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

## Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 73 |
| Total Test Logs | 70 |
| Missing Test Cases | 2 |
| Missing Test Logs | 3 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 17.81%

## Formula Analysis for Defect Rate

### Formula

```text
Defect Rate = (Total Defects / Total Test Cases) × 100
```

### Description

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

### Components

| Component | Description |
|-----------|-------------|
| Total Defects | Total number of defects identified during the test cycle |
| Total Test Cases | Total number of test cases executed |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |

## Conclusion

The report indicates outstanding coverage and execution issues that require remediation before progression. Multiple user stories contain partially covered acceptance criteria with critical coverage gaps, test case failures are present across all user stories, and 13 defects have been identified requiring resolution.
