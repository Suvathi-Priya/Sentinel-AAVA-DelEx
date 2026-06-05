# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 2, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

**Inclusions:** Unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

**Exclusions:** Integration tests, system tests, performance tests, and user stories not mapped to test cases.

**Baseline Definition:** The 2 user stories serve as the baseline reference for measuring coverage, execution success, and defect quality.

## Test Coverage Summary

**Total User Stories:** 2

### Coverage Details

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 2 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-006 | AC2 | No testcase explicitly validates that adjusted billing amount is detailed in the downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that effective date is captured in the downgrade audit log. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer details are included in the transfer notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that incoming owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that subscription transfers involving a change in billing entity require compliance team approval before the transfer is completed. | Not Covered |
| SCM-007 | AC5 | No testcase explicitly validates that subscription transfers involving a change in tax jurisdiction require compliance team approval before the transfer is completed. | Not Covered |

### Coverage Score

| User Story ID | Title | Total Acceptance Criterias | Fully Covered Acceptance Criterias | Partially Covered Acceptance Criterias | Not Covered Acceptance Criterias | Coverage Score Percentage |
|---|---|---:|---:|---:|---:|---:|
| SCM-006 | Subscription Downgrade Management | 5 | 3 | 2 | 0 | 60.00 |
| SCM-007 | Subscription Transfer and Ownership Change | 5 | 2 | 2 | 1 | 40.00 |
| Overall | Overall | 10 | 5 | 4 | 1 | 50.00 |

## Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 28

**Total Test Cases Passed:** 25

**Total Test Cases Failed:** 3

### Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| SCM-006 | 15 | 13 | 12 | 1 |
| SCM-007 | 13 | 15 | 13 | 2 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| TP_SCM7_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_014 | SCM-007 | AC5 | High |
| TP_SCM7_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_015 | SCM-007 | AC5 | High |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 28 |
| Total Test Logs | 28 |
| Missing Test Cases | 2 |
| Missing Test Logs | 2 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 10.71%

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |

## Conclusion

Remediation is required as test case failures and defects exist in the current test suite. The report indicates outstanding coverage gaps and execution issues that must be addressed before progression.
