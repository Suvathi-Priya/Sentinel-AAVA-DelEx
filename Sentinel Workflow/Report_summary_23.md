<div align="center"><strong><span style="font-size:28px;">UNIT TEST QUALITY & COVERAGE REPORT</span></strong></div>

# Scope

This report evaluates unit test coverage and quality across 6 user stories.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The 6 user stories form the baseline for evaluation, covering unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

# Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---|---|---|---|
| CLP-001 | AC5 | No testcase explicitly validates fraud review requirement. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates timestamp capture. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates the retry limit of 3 times. | Partially Covered |
| ORM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the $1000 threshold. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates revised billing amount inclusion in notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates subscription ID capture. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates upgrade date capture. | Partially Covered |
| SCM-004 | AC2 | No testcase explicitly validates applicable refund details inclusion in notification. | Partially Covered |
| SCM-004 | AC4 | No testcase explicitly validates effective date capture in audit log. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date viewing in customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates timestamp capture in audit log. | Partially Covered |

# Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 73

**Total Test Cases Passed:** 59

**Total Test Cases Failed:** 14

# Overall Test Execution Summary

**Total Test Cases Executed:** 73

**Total Test Cases Passed:** 59

**Total Test Cases Failed:** 14

# Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| CLP-001 | 13 | 15 | 11 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |
| ORM-001 | 15 | 15 | 12 | 3 |
| SCM-003 | 15 | 15 | 13 | 2 |
| SCM-004 | 15 | 15 | 13 | 2 |
| SCM-002 | 15 | 15 | 13 | 2 |

# Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | NULL | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | NULL | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | NULL | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | NULL | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 73 |
| Total Test Logs | 73 |
| Missing Test Cases | 2 |
| Missing Test Logs | 2 |
| Consistency Status | Mismatch Detected |

# Defect Details

### Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM4-101 | TP_SCM4_005 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_014 | SCM-004 | Finance team approval workflow fails to initiate for accounts with mixed currency outstanding balances |
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |

# Conclusion

Remediation is required as multiple user stories have coverage gaps and test case failures with associated defects exist across all user stories.
