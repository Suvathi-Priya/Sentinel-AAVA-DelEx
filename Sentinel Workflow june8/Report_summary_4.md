# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

Total User Stories: 2

The user stories form the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to these user stories.

## Test Coverage Summary

Coverage Details:

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 2 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

Coverage Gap Details:

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates that adjusted billing amount is included in the downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that effective date is captured in the downgrade audit log. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer details are included in the transfer notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that billing change summary is viewable in the customer portal. | Partially Covered |

## Test Execution Summary

Overall Test Execution Summary:

Total Test Cases Executed: 26

Total Test Cases Passed: 24

Total Test Cases Failed: 2

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| SCM-006 | 15 | 13 | 12 | 1 |
| SCM-007 | 13 | 13 | 12 | 2 |

## Consistency Analysis

Data Mapping Inconsistency Details:

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |

Consistency Metrics Summary:

| Metric | Count |
|--------|-------|
| Total Test Cases | 28 |
| Total Test Logs | 26 |
| Missing Test Cases | 0 |
| Missing Test Logs | 2 |
| Consistency Status | Mismatch Detected |

## Defect Details

Defect Rate: 10.71%

Defect Rate Analysis:

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:
Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:
- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

Defect Details:

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |

## Conclusion

Remediation is required as test case failures and defects exist in the current test suite.
