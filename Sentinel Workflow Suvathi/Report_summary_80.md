# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-005 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-005 | AC4 | No testcase explicitly validates reminder date capture.; No testcase explicitly validates channel used capture. | Partially Covered |
| SCM-005 | AC5 | No testcase explicitly validates that reminders are sent to both the customer and the assigned account manager for high-value subscriptions. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| TP_SCM5_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_001 | SCM-005 | AC1 | Medium |
| TP_SCM5_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_002 | SCM-005 | AC1 | Medium |
| TP_SCM5_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_003 | SCM-005 | AC1 | Medium |
| TP_SCM5_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_004 | SCM-005 | AC2 | Medium |
| TP_SCM5_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_005 | SCM-005 | AC2 | Medium |
| TP_SCM5_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_006 | SCM-005 | AC2 | Medium |
| TP_SCM5_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_007 | SCM-005 | AC3 | Medium |
| TP_SCM5_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_008 | SCM-005 | AC3 | Medium |
| TP_SCM5_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_009 | SCM-005 | AC3 | Medium |
| TP_SCM5_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_010 | SCM-005 | AC4 | Medium |
| TP_SCM5_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_011 | SCM-005 | AC1 | Medium |
| TP_SCM5_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_012 | SCM-005 | AC2 | Medium |
| TP_SCM5_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_013 | SCM-005 | AC5 | Medium |
| TP_SCM5_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_014 | SCM-005 | AC5 | Medium |
| TP_SCM5_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM5_015 | SCM-005 | AC4 | Medium |
| TP_SCM6_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_001 | SCM-006 | AC1 | High |
| TP_SCM6_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_002 | SCM-006 | AC1 | High |
| TP_SCM6_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_003 | SCM-006 | AC1 | High |
| TP_SCM6_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_004 | SCM-006 | AC2 | High |
| TP_SCM6_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_005 | SCM-006 | AC2 | High |
| TP_SCM6_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_006 | SCM-006 | AC2 | High |
| TP_SCM6_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_007 | SCM-006 | AC3 | High |
| TP_SCM6_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_008 | SCM-006 | AC3 | High |
| TP_SCM6_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_009 | SCM-006 | AC3 | High |
| TP_SCM6_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_010 | SCM-006 | AC4 | High |
| TP_SCM6_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_011 | SCM-006 | AC1 | High |
| TP_SCM6_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_012 | SCM-006 | AC4 | High |
| TP_SCM6_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_013 | SCM-006 | AC5 | High |
| TP_SCM6_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | High |
| TP_SCM6_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | High |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
| Missing Test Cases | 15 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

## Defect Details

No defects reported for this User Story.

## Conclusion

Remediation is required as coverage gaps exist in acceptance criteria AC4 and AC5, and all test execution logs are missing for the analyzed user story.
