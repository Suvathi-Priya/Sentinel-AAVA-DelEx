# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 2

The user stories form the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

**Total User Stories:** 2

### Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 1 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 1 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-002 | AC2 | No testcase explicitly validates that the resume date is included in the pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that customers can view the scheduled resume date in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that the pause start date is captured in the pause audit logs. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that the timestamp is captured in the pause audit logs. | Partially Covered |

## Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 18

**Total Test Cases Passed:** 16

**Total Test Cases Failed:** 2

### Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-002 | 15 | 12 | 11 | 1 |
| ORM-001 | 5 | 5 | 4 | 1 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_013 | SCM-002 | NULL | Medium |
| TP_SCM_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_014 | SCM-002 | NULL | Medium |
| TP_SCM_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_015 | SCM-002 | NULL | Medium |
| TC_EXTRA_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TC_EXTRA_001 | NULL | NULL | High |

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 20 |
| Total Test Logs | 18 |
| Missing Test Cases | 1 |
| Missing Test Logs | 3 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 10.00%

### Defect Rate Analysis

**Formula:** (Total Defects / Total Test Cases) × 100

**Calculation:** (2 / 20) × 100 = 10.00

**Description:**
Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

**Components:**
- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

### Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|--------------------|
| DEF-812 | TP_SCM_004 | SCM-002 | Email notification service failed to dispatch pause confirmation emails due to an SMTP configuration issue. |
| DEF-955 | TC_ORM_05 | ORM-001 | The email service is not triggering for refund confirmations. The API call to the notification service returns a 500 error. |

## Conclusion

Remediation is required as test case failures and defects exist in the current test suite. The report indicates outstanding execution issues that must be addressed before progression.
