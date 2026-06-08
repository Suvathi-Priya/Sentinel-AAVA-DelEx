# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

The baseline for evaluation consists of 1 user story with associated acceptance criteria. Unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories are included in the analysis. Integration tests, system tests, performance tests, and user stories not mapped to test cases are excluded from this scope.

## Test Coverage Summary

**Total User Stories:** 1

### Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 1 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| ORM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold for high-value refunds. | Partially Covered |

### Coverage Score

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| ORM-001 | 60.00% | 🔴 Red |

### Legend

| Color | Coverage Range | Interpretation |
|-------|----------------|----------------|
| 🟢 Green | 90–100% | High coverage (meets quality expectations) |
| 🟠 Amber | 70–89% | Moderate coverage (requires attention) |
| 🔴 Red | <70% | Low coverage (critical gaps present) |

### Formula Analysis for Coverage Score

#### Formula

```text
Coverage Score (%) = (Fully Covered Acceptance Criteria for the User Story / Total Acceptance Criteria in the User Story) × 100
```

#### Description

Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

#### Components

| Component | Description |
|-----------|-------------|
| Covered Acceptance Criteria for the User Story | Number of acceptance criteria within the user story that have at least one mapped test case. |
| Total Acceptance Criteria in the User Story | Total number of acceptance criteria defined for that specific user story. |

#### Calculation Scope

Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

## Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 0

**Total Test Cases Passed:** 0

**Total Test Cases Failed:** 0

### Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| ORM-001 | 15 | 0 | 0 | 0 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
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

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 15 |
| Total Test Logs | 0 |
| Missing Test Cases | 0 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 0.00%

### Formula Analysis for Defect Rate

#### Formula

```text
Defect Rate = (Total Defects / Total Test Cases) × 100
```

#### Description

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

#### Components

| Component | Description |
|-----------|-------------|
| Total Defects | Total number of defects identified during the test cycle |
| Total Test Cases | Total number of test cases executed |

### Defect Details

No defects identified in the provided data.

## Conclusion

Remediation is required as user story ORM-001 contains partially covered acceptance criteria and all test execution logs are missing. The unit test suite requires completion of coverage gaps and execution of all planned test cases before progression.
