# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

Coverage Boundary: The total number of user stories included in the analysis is 2, which form the baseline for evaluation.

Inclusions:
- Unit test cases linked to the identified user stories
- Test execution results (executed, not executed, passed, failed)
- Defect data directly associated with these user stories

Exclusions:
- Integration tests, system tests, or performance tests
- User stories not mapped to test cases

## Test Coverage Summary

Total Use Cases: 2

Coverage Details:

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 1 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 1 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

Coverage Gap Details:

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| ORM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold for high-value refunds. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date viewing. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates timestamp capture in audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that approval is required before pause activation. | Partially Covered |

Coverage Score Details:

Step-by-step Coverage Score Calculation:

For ORM-001:
- Count of Fully Covered Acceptance Criteria: 3 (AC1, AC2, AC3)
- Count of Total Acceptance Criteria: 5
- Coverage Score = (3/5) × 100 = 60.00%

For SCM-002:
- Count of Fully Covered Acceptance Criteria: 1 (AC1)
- Count of Total Acceptance Criteria: 5
- Coverage Score = (1/5) × 100 = 20.00%

| User Story ID | Coverage Score | Color |
|---|---:|---|
| ORM-001 | 60.00% | 🔴 Red |
| SCM-002 | 20.00% | 🔴 Red |

Legend:
- 🟢 Green (90–100%) → High coverage (meets quality expectations)
- 🟠 Amber (70–89%) → Moderate coverage (requires attention)
- 🔴 Red (<70%) → Low coverage (critical gaps present)

Coverage Score Analysis:

Coverage Score (%) = (Fully Covered Acceptance Criteria for the User Story / Total Acceptance Criteria in the User Story) × 100

Description:
Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

Components:
- Covered Acceptance Criteria for the User Story: Number of acceptance criteria within the user story that have at least one mapped test case.
- Total Acceptance Criteria in the User Story: Total number of acceptance criteria defined for that specific user story.

Calculation Scope:
Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

## Test Execution Summary

Total Test Cases Executed: 30

Total Test Cases Passed: 25

Total Test Cases Failed: 5

Step-by-step Execution Success Rate Calculation:
- Count of total Test cases Passed for all User Stories: 25
- Count of Total Test Cases Executed for all User Stories: 30
- Execution Success Rate = (25/30) × 100 = 83.33%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| ORM-001 | 15 | 15 | 12 | 3 |
| SCM-002 | 15 | 15 | 13 | 2 |

## Defect Details

Step-by-step Defect Rate Calculation:
- Count of Total Defects for all User Stories: 5
- Count of Total Test Cases for all User Stories: 30
- Defect Rate = (5/30) × 100 = 16.67%

Defect Rate Analysis:

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:
Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:
- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

Defect Details:

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |

## Conclusion

Remediation is required as test case failures and defects exist in the current test suite.
