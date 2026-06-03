# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:**
- Total number of user stories: 2
- User stories form the baseline for evaluation
- Scope limited to unit test coverage and execution records mapped to these user stories

**Inclusions:**
- Unit test cases linked to the identified user stories
- Test execution results (executed, not executed, passed, failed)
- Defect data directly associated with these user stories

**Exclusions:**
- Integration tests, system tests, or performance tests
- User stories not mapped to test cases

## Test Coverage Summary

**Total User Stories:** 2

**Coverage Details:**

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 1 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 1 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

**Coverage Gap Details:**

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| CLP-001 | AC5 | No testcase explicitly validates fraud review requirement. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times. | Partially Covered |

**Coverage Score:**

| User Story ID | Coverage Score | Color |
|---|---:|---|
| CLP-001 | 80.00% | 🟠 Amber |
| CNS-001 | 60.00% | 🔴 Red |

## Test Execution Summary

**Total Test Cases Executed:** 28

**Total Test Cases Passed:** 22

**Total Test Cases Failed:** 6

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| CLP-001 | 15 | 15 | 12 | 3 |
| CNS-001 | 13 | 13 | 10 | 3 |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

## Conclusion

Remediation is required as coverage gaps exist in user story CNS-001 and test case failures are present across both user stories.
