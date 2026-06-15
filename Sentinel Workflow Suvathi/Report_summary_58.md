# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 5 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories. The baseline consists of 5 user stories with 25 acceptance criteria, forming the reference for measuring coverage, execution success, and defect quality.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-001 | AC5 | No testcase explicitly validates fraud review requirement for high-value refunds. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates next billing cycle changes visibility in customer portal. | Partially Covered |
| SCM-005 | AC4 | No testcase explicitly validates reminder date capture in renewal reminder log.; No testcase explicitly validates channel used capture in renewal reminder log. | Partially Covered |

## Consistency Analysis

**Data Mapping Inconsistency Details:**

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | NULL | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | NULL | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | NULL | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | NULL | Medium |

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | NULL | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | NULL | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | NULL | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | NULL | Medium |

## Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 75 |
| Total Test Logs | 71 |
| Missing Test Cases | 0 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

**SCM-001:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-ORM-001 | UT_SCM1_005 | SCM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_SCM1_009 | SCM-001 | Refund workflow synchronization error |

**SCM-002:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM-101 | TP_SCM_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_009 | SCM-002 | Activation allowed without completed approval |

**SCM-003:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM3-101 | TP_SCM3_004 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |

**SCM-004:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM4-101 | TP_SCM4_004 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_009 | SCM-004 | Finance team approval workflow fails for mixed currency outstanding balances |

**SCM-005:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-103 | TP_SCM5_011 | SCM-005 | System sends reminder even when subscription expiry date is null |
| DEF-SCM5-104 | TP_SCM5_013 | SCM-005 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |
| DEF-SCM5-105 | TP_SCM5_015 | SCM-005 | Reminder log delivery status remains blank when notification channel fails |

## Conclusion

Remediation is required as multiple defects exist across all user stories and coverage gaps are present in 4 out of 5 user stories.