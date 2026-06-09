# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-002 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-002 | AC2 | No testcase explicitly validates inclusion of resume date in pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates viewing scheduled resume date in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates capture of pause start date in audit log.; No testcase explicitly validates capture of timestamp in audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval is required before pause activation. | Partially Covered |

## Test Execution Summary

**Overall Test Execution Summary:**

Total Test Cases Executed: 15

Total Test Cases Passed: 13

Total Test Cases Failed: 2

## Overall Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---|---|---|---|
| SCM-002 | 15 | 15 | 13 | 2 |

## Consistency Analysis

**Consistency Metrics Summary:**

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Consistency Status | Consistent |

## Data Mapping Inconsistency Details

No data available.

## Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Consistency Status | Consistent |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |

## Conclusion

Remediation is required as test case failures and defects exist in the unit test suite. The report indicates outstanding coverage gaps and execution issues that must be addressed before progression.
