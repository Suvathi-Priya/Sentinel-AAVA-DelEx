# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 8 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 8

The user stories form the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

**Coverage Details:**

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 2 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 2 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 4 | User stories where all acceptance criteria are Not Covered |

**Coverage Gap Details:**

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-002 | AC2 | No testcase explicitly validates that resume date is included in the pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that customers can view the scheduled resume date in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that pause start date is captured in the audit log. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that timestamp is captured in the audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval is required before the pause is activated. | Partially Covered |
| CNS-001 | AC1 | No testcase explicitly validates that the service accepts a notification payload containing user ID. | Not Covered |
| CNS-001 | AC1 | No testcase explicitly validates that the service accepts a notification payload containing message. | Not Covered |
| CNS-001 | AC1 | No testcase explicitly validates that the service accepts a notification payload containing channel preferences. | Not Covered |
| CNS-001 | AC2 | No testcase explicitly validates that the service correctly routes notifications to the user's preferred email address. | Partially Covered |
| CNS-001 | AC3 | No testcase explicitly validates that the service correctly routes notifications to the user's preferred SMS number. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates that the service correctly routes push notifications to the user's registered devices. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that the system generates a report of all successful and failed updates. | Not Covered |
| SCM-003 | AC5 | No testcase explicitly validates that an error is logged for any rows with non-numeric quantities. | Partially Covered |

## Test Execution Summary

**Overall Test Execution Summary:**

Total Test Cases Executed: 28

Total Test Cases Passed: 26

Total Test Cases Failed: 2

**Test Execution Summary Details:**

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-002 | 15 | 14 | 13 | 1 |
| CLP-001 | 5 | 5 | 5 | 0 |
| CNS-001 | 4 | 5 | 5 | 0 |
| SCM-003 | 4 | 4 | 3 | 1 |
| SCM-004 | 0 | 0 | 0 | 0 |
| SCM-005 | 0 | 0 | 0 | 0 |
| SCM-006 | 0 | 0 | 0 | 0 |
| SCM-007 | 0 | 0 | 0 | 0 |

## Consistency Analysis

**Data Mapping Inconsistency Details:**

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_015 | SCM-002 | AC5 | Medium |
| CNS_TC_07 | missing_testcase | Mapped testcase definition is missing for testcase ID: CNS_TC_07 | CNS-001 | AC3 | High |

**Consistency Metrics Summary:**

| Metric | Count |
|--------|-------|
| Total Test Cases | 28 |
| Total Test Logs | 28 |
| Missing Test Cases | 1 |
| Missing Test Logs | 1 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 7.14%

**Defect Rate Analysis:**

Defect Rate = (Total Defects / Total Test Cases) × 100

**Description:**

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

**Components:**

Total Defects: Total number of defects identified during the test cycle

Total Test Cases: Total number of test cases executed

**Defect Details:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-881 | TP_SCM_012 | SCM-002 | Audit log for subscription pause events is not capturing the pause reason. The field is being written as NULL instead of the user-selected reason. |
| DEF-882 | SCM03_TC03 | SCM-003 | Bulk sale inventory update failed when processing multiple locations. The update process is adding the new quantity to the old one instead of replacing it for some locations. |

## Conclusion

Remediation is required as 4 user stories are Not Covered and 2 test cases have failed with associated defects.
