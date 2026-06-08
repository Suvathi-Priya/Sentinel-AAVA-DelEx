<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 3 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:**
- Total number of user stories included in analysis: 3
- These user stories form the baseline for evaluation
- Scope limited to unit test coverage and execution records mapped to these user stories

# Test Coverage Summary

**Total User Stories:** 3

## Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 3 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

## Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---------------|-------|---------------------|-----------------|
| ORM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold for high-value refunds. | Partially Covered |
| CLP-001 | AC5 | No testcase explicitly validates fraud review requirement for reward redemptions above 5000 points. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times for failed notifications. | Partially Covered |

## Coverage Score

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| ORM-001 | 60.00% | 🔴 Red |
| CLP-001 | 80.00% | 🟠 Amber |
| CNS-001 | 40.00% | 🔴 Red |

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

### Calculation Scope:

Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

# Test Execution Summary

**Overall Test Execution Summary:**

Total Test Cases Executed: 43

Total Test Cases Passed: 34

Total Test Cases Failed: 9

## Overall Test Execution Summary

Total Test Cases Executed: 43

Total Test Cases Passed: 34

Total Test Cases Failed: 9

## Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| ORM-001 | 15 | 15 | 12 | 3 |
| CLP-001 | 13 | 15 | 12 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |

# Consistency Analysis

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

## Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 43 |
| Total Test Logs | 43 |
| Missing Test Cases | 2 |
| Missing Test Logs | 2 |
| Consistency Status | Mismatch Detected |

# Defect Details

**Defect Rate:** 20.93%

## Defect Rate

20.93%

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
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

# Conclusion

The report indicates that remediation is required as all user stories are Partially Covered with coverage gaps identified and 9 defects exist across the test execution results.
