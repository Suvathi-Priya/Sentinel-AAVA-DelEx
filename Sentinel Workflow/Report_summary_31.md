<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 1 user story.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story CLP-001 forms the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to this user story.

# Test Coverage Summary

## Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---|---|---|---|
| CLP-001 | AC1 | System must award loyalty points for eligible purchases. | Not Covered |
| CLP-001 | AC2 | Customers must be able to redeem loyalty points for rewards. | Not Covered |
| CLP-001 | AC3 | Loyalty points balance must be viewable by customers in the portal. | Not Covered |
| CLP-001 | AC4 | Loyalty transaction logs must capture customer ID, points earned or redeemed, and transaction timestamp. | Not Covered |
| CLP-001 | AC5 | Reward redemptions above 5000 points must require manager approval and fraud review. | Not Covered |

# Test Execution Summary

**Total Test Cases Executed:** 13

**Total Test Cases Passed:** 10

**Total Test Cases Failed:** 3

## Overall Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| CLP-001 | 0 | 0 | 0 | 0 |
| ORM-001 | 15 | 0 | 0 | 0 |
| CNS-001 | 0 | 13 | 10 | 3 |

# Consistency Analysis

Mismatch Detected

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_ORM_001 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_001 | ORM-001 | AC1 | Medium |
| UT_ORM_002 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_002 | ORM-001 | AC1 | Medium |
| UT_ORM_003 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_003 | ORM-001 | AC1 | Medium |
| UT_ORM_004 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_004 | ORM-001 | AC2 | Medium |
| UT_ORM_005 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_005 | ORM-001 | AC2 | Medium |
| UT_ORM_006 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_006 | ORM-001 | AC2 | Medium |
| UT_ORM_007 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_007 | ORM-001 | AC3 | Medium |
| UT_ORM_008 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_008 | ORM-001 | AC3 | Medium |
| UT_ORM_009 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_009 | ORM-001 | AC3 | Medium |
| UT_ORM_010 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_010 | ORM-001 | AC4 | Medium |
| UT_ORM_011 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_011 | ORM-001 | AC4 | Medium |
| UT_ORM_012 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_012 | ORM-001 | AC4 | Medium |
| UT_ORM_013 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_013 | ORM-001 | AC5 | Medium |
| UT_ORM_014 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_014 | ORM-001 | AC5 | Medium |
| UT_ORM_015 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_015 | ORM-001 | AC5 | Medium |
| UT_CNS_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_001 | CNS-001 | AC1 | High |
| UT_CNS_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_002 | CNS-001 | AC1 | High |
| UT_CNS_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_003 | CNS-001 | AC1 | High |
| UT_CNS_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_004 | CNS-001 | AC2 | High |
| UT_CNS_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_005 | CNS-001 | AC2 | High |
| UT_CNS_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_006 | CNS-001 | AC2 | High |
| UT_CNS_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_007 | CNS-001 | AC3 | High |
| UT_CNS_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_008 | CNS-001 | AC3 | High |
| UT_CNS_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_009 | CNS-001 | AC3 | High |
| UT_CNS_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_010 | CNS-001 | AC4 | High |
| UT_CNS_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_011 | CNS-001 | AC4 | High |
| UT_CNS_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_012 | CNS-001 | AC4 | High |
| UT_CNS_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_013 | CNS-001 | AC5 | High |

## Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 13 |
| Missing Test Cases | 13 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

# Defect Details

No defect details are available for the analyzed user story CLP-001.

# Conclusion

Remediation is required as user story CLP-001 is Not Covered and test case failures exist with associated defects.
