# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 2

**Coverage Boundary:** The analysis encompasses 30 unit test cases linked to the identified user stories, forming the baseline for evaluation of coverage, execution success, and defect quality.

## Test Coverage Summary

**Total Use Cases:** 2

### Coverage Gap Details:

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-001 | AC5 | No testcase explicitly validates fraud review requirement for high-value refunds above $1000. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates that resume date is included in pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that customers can view scheduled resume date in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that pause start date is captured in pause audit logs. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval must be completed before the pause is activated. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details:

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| UT_SCM1_001 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_001 | SCM-001 | NULL | NULL |
| UT_SCM1_002 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_002 | SCM-001 | NULL | NULL |
| UT_SCM1_003 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_003 | SCM-001 | NULL | NULL |
| UT_SCM1_004 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_004 | SCM-001 | NULL | NULL |
| UT_SCM1_005 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_005 | SCM-001 | NULL | NULL |
| UT_SCM1_006 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_006 | SCM-001 | NULL | NULL |
| UT_SCM1_007 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_007 | SCM-001 | NULL | NULL |
| UT_SCM1_008 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_008 | SCM-001 | NULL | NULL |
| UT_SCM1_009 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_009 | SCM-001 | NULL | NULL |
| UT_SCM1_010 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_010 | SCM-001 | NULL | NULL |
| UT_SCM1_011 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_011 | SCM-001 | NULL | NULL |
| UT_SCM1_012 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_012 | SCM-001 | NULL | NULL |
| UT_SCM1_013 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_013 | SCM-001 | NULL | NULL |
| UT_SCM1_014 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_014 | SCM-001 | NULL | NULL |
| UT_SCM1_015 | missing_testlog | Execution log is missing for testcase ID: UT_SCM1_015 | SCM-001 | NULL | NULL |
| TP_SCM1_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_001 | SCM-001 | NULL | NULL |
| TP_SCM1_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_002 | SCM-001 | NULL | NULL |
| TP_SCM1_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_003 | SCM-001 | NULL | NULL |
| TP_SCM1_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_004 | SCM-001 | NULL | NULL |
| TP_SCM1_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_005 | SCM-001 | NULL | NULL |
| TP_SCM1_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_006 | SCM-001 | NULL | NULL |
| TP_SCM1_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_007 | SCM-001 | NULL | NULL |
| TP_SCM1_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_008 | SCM-001 | NULL | NULL |
| TP_SCM1_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM1_009 | SCM-001 | NULL | NULL |

### Consistency Metrics Summary:

| Metric | Count |
|--------|-------|
| Total Test Cases | 30 |
| Total Test Logs | 30 |
| Missing Test Cases | 9 |
| Missing Test Logs | 15 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM1-001 | TP_SCM1_005 | SCM-001 | Notification template rendering issue |
| DEF-SCM1-002 | TP_SCM1_009 | SCM-001 | Refund workflow synchronization error |
| DEF-SCM2-101 | TP_SCM2_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM2-102 | TP_SCM2_009 | SCM-002 | Activation allowed without completed approval |

## Conclusion

Remediation is required as coverage gaps exist in both user stories and defects have been identified in the test execution results.
