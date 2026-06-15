# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-005 forms the baseline reference for measuring coverage, execution success, and defect quality.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-005 | AC4 | No testcase explicitly validates reminder date capture in renewal reminder logs.; No testcase explicitly validates channel used capture in renewal reminder logs. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

No data mapping inconsistencies detected.

### Consistency Metrics Summary

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
| DEF-SCM5-103 | TP_SCM5_011 | SCM-005 | System sends reminder even when subscription expiry date is null |
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-105 | TP_SCM5_015 | SCM-005 | Reminder log delivery status remains blank when notification channel fails |
| DEF-SCM5-104 | TP_SCM5_013 | SCM-005 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |

## Conclusion

Remediation is required as coverage gaps exist in AC4 and multiple defects have been identified across the test execution results.
