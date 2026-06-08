# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user stories form the baseline reference for measuring coverage, execution success, and defect quality.

**Coverage Boundary:** The total number of user stories included in the analysis is 3, which form the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

**Inclusions:** Unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

**Exclusions:** Integration tests, system tests, performance tests, and user stories not mapped to test cases.

## Test Coverage Summary

**Total User Stories:** 3

### Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 1 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 2 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates inclusion of adjusted billing amount in downgrade confirmation notifications. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates capture of effective date in downgrade audit logs. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates inclusion of transfer details in transfer notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that incoming owner can view billing change summary in customer portal. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates compliance team approval requirement for transfers involving billing entity change. | Not Covered |
| SCM-007 | AC5 | No testcase explicitly validates compliance team approval requirement for transfers involving tax jurisdiction change. | Not Covered |

## Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 48

**Total Test Cases Passed:** 42

**Total Test Cases Failed:** 6

### Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-005 | 15 | 15 | 13 | 2 |
| SCM-006 | 15 | 13 | 12 | 1 |
| SCM-007 | 13 | 20 | 17 | 3 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| TP_SCM7_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_014 | SCM-007 | AC5 | High |
| TP_SCM7_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_015 | SCM-007 | AC5 | High |
| TP_SCM4_001 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_001 |  | AC1 | Critical |
| TP_SCM4_002 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_002 |  | AC1 | Critical |
| TP_SCM4_003 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_003 |  | AC1 | Critical |
| TP_SCM4_004 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_004 |  | AC2 | Critical |
| TP_SCM4_005 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_005 |  | AC2 | Critical |
| TP_SCM4_006 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_006 |  | AC2 | Critical |
| TP_SCM4_007 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_007 |  | AC3 | Critical |
| TP_SCM4_008 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_008 |  | AC3 | Critical |
| TP_SCM4_009 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_009 |  | AC3 | Critical |
| TP_SCM4_010 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_010 |  | AC4 | Critical |
| TP_SCM4_011 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_011 |  | AC4 | Critical |
| TP_SCM4_012 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_012 |  | AC4 | Critical |
| TP_SCM4_013 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_013 |  | AC5 | Critical |
| TP_SCM4_014 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_014 |  | AC5 | Critical |
| TP_SCM4_015 | missing_testcase_and_testlog | Both testcase definition and execution log are missing for testcase ID: TP_SCM4_015 |  | AC5 | Critical |

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 43 |
| Total Test Logs | 48 |
| Missing Test Cases | 2 |
| Missing Test Logs | 2 |
| Consistency Status | Mismatch Detected |

## Defect Details

**Defect Rate:** 13.95%

### Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|--------------------|
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-102 | TP_SCM5_015 | SCM-005 | Account manager reminder not sent when subscription value exceeds threshold but account manager assignment is pending |
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |

## Conclusion

The report indicates outstanding coverage and execution issues that require remediation before progression. Test case failures and identified defects necessitate resolution to ensure system quality and compliance with acceptance criteria.
