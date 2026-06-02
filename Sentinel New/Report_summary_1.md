# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 2, forming the baseline for evaluation.

**Inclusions:**
- Unit test cases linked to the identified user stories
- Test execution results (executed, not executed, passed, failed)
- Defect data directly associated with these user stories

**Exclusions:**
- Integration tests, system tests, or performance tests
- User stories not mapped to test cases

## Test Coverage Summary

**Total Use Cases:** 2

**Coverage Details:**

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 1 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 1 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

**Coverage Gap Details:**

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture in notification logs | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times | Partially Covered |

**Coverage Score Details:**

**Step-by-step Coverage Score Calculation:**

**CLP-001:**
- Count of Fully Covered Acceptance Criteria: 5
- Count of Total Acceptance Criteria: 5
- Coverage Score (%) = (5 / 5) × 100 = 100.00%

**CNS-001:**
- Count of Fully Covered Acceptance Criteria: 3
- Count of Total Acceptance Criteria: 5
- Coverage Score (%) = (3 / 5) × 100 = 60.00%

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| CLP-001 | 100.00% | 🟢 Green |
| CNS-001 | 60.00% | 🔴 Red |

**Legend:**
- 🟢 Green (90–100%) → High coverage (meets quality expectations)
- 🟠 Amber (70–89%) → Moderate coverage (requires attention)
- 🔴 Red (<70%) → Low coverage (critical gaps present)

**Coverage Score Analysis:**

Coverage Score (%) = (Fully Covered Acceptance Criteria for the User Story / Total Acceptance Criteria in the User Story) × 100

**Description:** Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

**Components:**
- Covered Acceptance Criteria for the User Story: Number of acceptance criteria within the user story that have at least one mapped test case
- Total Acceptance Criteria in the User Story: Total number of acceptance criteria defined for that specific user story

**Calculation Scope:** Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

## Test Execution Summary

**Total Test Cases Executed:** 13

**Total Test Cases Passed:** 10

**Total Test Cases Failed:** 3

**Test Execution Summary Details:**

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| CLP-001 | 15 | 0 | 0 | 0 |
| CNS-001 | 15 | 13 | 10 | 3 |

**Data Mapping Inconsistency Details:**

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| UT_CLP_001 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_001 | CLP-001 | AC1 | Medium |
| UT_CLP_002 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_002 | CLP-001 | AC1 | Medium |
| UT_CLP_003 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_003 | CLP-001 | AC1 | Medium |
| UT_CLP_004 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_004 | CLP-001 | AC2 | Medium |
| UT_CLP_005 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_005 | CLP-001 | AC2 | Medium |
| UT_CLP_006 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_006 | CLP-001 | AC2 | Medium |
| UT_CLP_007 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_007 | CLP-001 | AC3 | Medium |
| UT_CLP_008 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_008 | CLP-001 | AC3 | Medium |
| UT_CLP_009 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_009 | CLP-001 | AC3 | Medium |
| UT_CLP_010 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_010 | CLP-001 | AC4 | Medium |
| UT_CLP_011 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_011 | CLP-001 | AC4 | Medium |
| UT_CLP_012 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_012 | CLP-001 | AC4 | Medium |
| UT_CLP_013 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_013 | CLP-001 | AC5 | Medium |
| UT_CLP_014 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | Medium |
| UT_CLP_015 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | Medium |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

**Consistency Metrics Summary:**

| Metric | Count |
|--------|-------|
| Total Test Cases | 30 |
| Total Test Logs | 13 |
| Missing Test Cases | 0 |
| Missing Test Logs | 17 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Step-by-step Defect Rate Calculation:**
- Count of Total Defects for all User Stories: 3
- Count of Total Test Cases for all User Stories: 30
- Defect Rate = (3 / 30) × 100 = 10.00%

**Defect Rate Analysis:**

Defect Rate = (Total Defects / Total Test Cases) × 100

**Description:** Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

**Components:**
- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

**Defect Details:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

## Conclusion

Remediation is required as user story CNS-001 has coverage gaps and test case failures with defects present.
