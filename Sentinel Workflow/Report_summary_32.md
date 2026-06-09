# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story ORM-001 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

## Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---|---|---|---|
| ORM-001 | AC1 | System must create refund requests for eligible orders. | Not Covered |
| ORM-001 | AC2 | Refund approval notifications must be sent to customers. | Not Covered |
| ORM-001 | AC3 | Refund status must be viewable by customers in the portal. | Not Covered |
| ORM-001 | AC4 | Refund audit logs must capture customer ID, refund amount, and approval timestamp. | Not Covered |
| ORM-001 | AC5 | High-value refunds above $1000 must require manager approval and fraud review. | Not Covered |

## Test Execution Summary

**Total Test Cases Executed:** 15

**Total Test Cases Passed:** 12

**Total Test Cases Failed:** 3

## Overall Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| ORM-001 | 0 | 0 | 0 | 0 |

## Consistency Analysis

Mismatch Detected

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_CNS_001 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_001 | CNS-001 | AC1 | Medium |
| UT_CNS_002 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_002 | CNS-001 | AC1 | Medium |
| UT_CNS_003 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_003 | CNS-001 | AC1 | Medium |
| UT_CNS_004 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_004 | CNS-001 | AC2 | Medium |
| UT_CNS_005 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_005 | CNS-001 | AC2 | Medium |
| UT_CNS_006 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_006 | CNS-001 | AC2 | Medium |
| UT_CNS_007 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_007 | CNS-001 | AC3 | Medium |
| UT_CNS_008 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_008 | CNS-001 | AC3 | Medium |
| UT_CNS_009 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_009 | CNS-001 | AC3 | Medium |
| UT_CNS_010 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_010 | CNS-001 | AC4 | Medium |
| UT_CNS_011 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_011 | CNS-001 | AC4 | Medium |
| UT_CNS_012 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_012 | CNS-001 | AC4 | Medium |
| UT_CNS_013 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_013 | CNS-001 | AC5 | Medium |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |
| UT_CLP_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_001 | CLP-001 | AC1 | High |
| UT_CLP_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_002 | CLP-001 | AC1 | High |
| UT_CLP_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_003 | CLP-001 | AC1 | High |
| UT_CLP_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_004 | CLP-001 | AC2 | High |
| UT_CLP_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_005 | CLP-001 | AC2 | High |
| UT_CLP_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_006 | CLP-001 | AC2 | High |
| UT_CLP_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_007 | CLP-001 | AC3 | High |
| UT_CLP_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_008 | CLP-001 | AC3 | High |
| UT_CLP_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_009 | CLP-001 | AC3 | High |
| UT_CLP_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_010 | CLP-001 | AC4 | High |
| UT_CLP_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_011 | CLP-001 | AC4 | High |
| UT_CLP_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_012 | CLP-001 | AC4 | High |
| UT_CLP_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_013 | CLP-001 | AC5 | High |
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |

## Consistency Metrics Summary

| Metric | Count |
|---|---|
| total_testcases | 15 |
| total_testlogs | 15 |
| consistency_status | Mismatch Detected |
| missing_testlogs | 15 |
| missing_testcases | 15 |

## Defect Details

No defects reported for this User Story.

## Conclusion

Remediation is required as user story ORM-001 is Not Covered. The unit test suite requires comprehensive test case development to address all acceptance criteria before progression.
