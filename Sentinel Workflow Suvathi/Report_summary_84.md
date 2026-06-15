# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-002 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates customer ID capture in pause audit logs.; No testcase explicitly validates subscription ID capture in pause audit logs.; No testcase explicitly validates pause reason capture in pause audit logs.; No testcase explicitly validates pause start date capture in pause audit logs.; No testcase explicitly validates timestamp capture in pause audit logs. | Not Covered |
| SCM-002 | AC5 | No testcase explicitly validates pause requests exceeding 90 days threshold.; No testcase explicitly validates manager approval requirement for pause requests exceeding 90 days.; No testcase explicitly validates that manager approval is required before pause activation. | Not Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

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
| DEF-SCM-101 | TP_SCM_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_009 | SCM-002 | Activation allowed without completed approval |

## Conclusion

Remediation is required as multiple user stories are Not Covered and defects exist in the test execution results.
