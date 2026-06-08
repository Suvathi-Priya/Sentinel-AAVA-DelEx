# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 6 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user stories form the baseline reference for measuring coverage, execution success, and defect quality.

## Test Coverage Summary

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates that adjusted billing amount is included in downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that effective date is captured in downgrade audit logs. | Partially Covered |
| CLP-001 | AC5 | No testcase explicitly validates that fraud review is required for reward redemptions above 5000 points. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates that revised billing amount is included in upgrade confirmation notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that subscription ID is captured in upgrade audit logs. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that upgrade date is captured in upgrade audit logs. | Partially Covered |
| ORM-001 | AC4 | No testcase explicitly validates that approval timestamp is captured in refund audit logs. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold for high-value refunds. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates that timestamp is captured in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates that retry attempts are limited to 3 times. | Partially Covered |
| SCM-004 | AC1 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC1 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC1 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC2 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC2 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC2 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC3 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC3 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC3 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC5 | No testcase is mapped to validate this requirement. | Not Covered |
| SCM-004 | AC5 | No testcase is mapped to validate this requirement. | Not Covered |

## Test Execution Summary

| Metric | Value |
|--------|-------|
| Total Test Cases in All Test Logs | 56 |
| Total Passed in All Test Logs | 51 |
| Total Failed in All Test Logs | 5 |
| Total Defects in All Test Logs | 8 |
| Overall Defect Rate Percentage | 13.79 |
| Overall Defect Rate Formula | (Total Defects / Total Test Cases) × 100 |
| Overall Defect Rate Calculation | (8 / 58) × 100 = 13.79 |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |
| TP_SCM4_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_001 | SCM-004 | AC1 | High |
| TP_SCM4_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_002 | SCM-004 | AC1 | High |
| TP_SCM4_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_003 | SCM-004 | AC1 | High |
| TP_SCM4_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_004 | SCM-004 | AC2 | High |
| TP_SCM4_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_005 | SCM-004 | AC2 | High |
| TP_SCM4_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_006 | SCM-004 | AC2 | High |
| TP_SCM4_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_007 | SCM-004 | AC3 | High |
| TP_SCM4_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_008 | SCM-004 | AC3 | High |
| TP_SCM4_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_009 | SCM-004 | AC3 | High |
| TP_SCM4_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_010 | SCM-004 | AC4 | High |
| TP_SCM4_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_011 | SCM-004 | AC4 | High |
| TP_SCM4_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_012 | SCM-004 | AC4 | High |
| TP_SCM4_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_013 | SCM-004 | AC5 | High |
| TP_SCM4_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC5 | High |
| TP_SCM4_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | High |

### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 73 |
| Total Test Logs | 71 |
| Missing Test Cases | 17 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Title | Defect Description |
|-----------|--------------|---------------|--------------|-------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | NULL | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | NULL | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | NULL | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | NULL | Redemption workflow synchronization issue |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | NULL | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | NULL | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | NULL | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | NULL | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | NULL | Push notification service unavailable |

## Conclusion

Remediation is required as user story SCM-004 is Not Covered and multiple test case failures and defects exist across the analyzed user stories.
