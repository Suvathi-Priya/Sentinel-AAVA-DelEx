# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 3

The user stories SCM-005, SCM-006, and SCM-007 form the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

**Total Use Cases:** 3

### Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 1 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 2 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates CSV formatting validation. | Partially Covered |
| SCM-007 | AC1 | No testcase explicitly validates that the endpoint accepts quantity parameter. | Partially Covered |
| SCM-007 | AC1 | No testcase explicitly validates that the endpoint accepts reservation timeout parameter. | Partially Covered |

## Test Execution Summary

**Total Test Cases Executed:** 48

**Total Test Cases Passed:** 40

**Total Test Cases Failed:** 5

### Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-005 | 15 | 15 | 14 | 1 |
| SCM-006 | 13 | 12 | 11 | 1 |
| SCM-007 | 12 | 13 | 10 | 3 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_013 | SCM-006 | AC5 | Medium |
| TP_SCM7_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_013 | SCM-007 | AC5 | High |

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 48 |
| Total Test Logs | 48 |
| Missing Test Cases | 1 |
| Missing Test Logs | 1 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 8.33%

### Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-902 | TP_SCM5_009 | SCM-005 | Saving renewal preferences in the customer portal results in a server error. |
| DEF-903 | TP_SCM6_008 | SCM-006 | Processing a CSV with a non-existent SKU results in an unhandled exception instead of a logged failure. |
| DEF-904 | TP_SCM7_006 | SCM-007 | Inventory reservation does not correctly decrement the available stock count. |
| DEF-905 | TP_SCM7_013 | SCM-007 | Race condition allows reservation request to be accepted even when stock is zero, but no reservation is created. |

## Conclusion

Remediation is required as test case failures and defects exist in the current test suite.
