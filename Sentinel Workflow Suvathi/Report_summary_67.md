# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 9 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 9, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

**Inclusions:** Unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

**Exclusions:** Integration tests, system tests, performance tests, and user stories not mapped to test cases.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| SCM-001 | AC5 | No testcase explicitly validates fraud review requirement for high-value refunds. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval is required before pause activation. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates resume date inclusion in upgrade confirmation notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates upgrade date capture in audit log. | Partially Covered |
| SCM-004 | AC4 | No testcase explicitly validates effective date capture in cancellation audit log. | Partially Covered |
| SCM-005 | AC4 | No testcase explicitly validates reminder date and channel used capture in renewal reminder logs. | Partially Covered |
| SCM-005 | AC5 | No testcase explicitly validates account manager notification for high-value subscriptions. | Partially Covered |
| SCM-006 | AC2 | No testcase explicitly validates adjusted billing amount inclusion in downgrade confirmation notification. | Partially Covered |
| SCM-007 | AC4 | No testcase explicitly validates transfer date and authorization reference capture in transfer audit logs. | Partially Covered |
| SCM-008 | AC1 | No testcase is mapped to this acceptance criterion. | Not Covered |
| SCM-008 | AC2 | No testcase is mapped to this acceptance criterion. | Not Covered |
| SCM-008 | AC3 | No testcase is mapped to this acceptance criterion. | Not Covered |
| SCM-008 | AC4 | No testcase is mapped to this acceptance criterion. | Not Covered |
| SCM-008 | AC5 | No testcase is mapped to this acceptance criterion. | Not Covered |
| SCM-009 | AC2 | No testcase explicitly validates SMS content generation for high-priority alerts. | Partially Covered |

## Consistency Analysis

**Data Mapping Inconsistency Details:**

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC2 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | Medium |
| TP_SCM8_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_001 | SCM-008 | AC1 | Medium |
| TP_SCM8_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_002 | SCM-008 | AC1 | Medium |
| TP_SCM8_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_003 | SCM-008 | AC1 | Medium |
| TP_SCM8_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_004 | SCM-008 | AC2 | Medium |
| TP_SCM8_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_005 | SCM-008 | AC2 | Medium |
| TP_SCM8_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_006 | SCM-008 | AC3 | Medium |
| TP_SCM8_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_007 | SCM-008 | AC3 | Medium |
| TP_SCM8_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_008 | SCM-008 | AC4 | Medium |
| TP_SCM8_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_009 | SCM-008 | AC5 | Medium |
| TP_SCM8_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_010 | SCM-008 | AC1 | Medium |
| TP_SCM8_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_011 | SCM-008 | AC2 | Medium |
| TP_SCM8_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_012 | SCM-008 | AC4 | Medium |
| TP_SCM8_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_013 | SCM-008 | AC5 | Medium |
| TP_SCM8_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_014 | SCM-008 | AC2 | Medium |
| TP_SCM8_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_015 | SCM-008 | AC5 | Medium |
| UT_SCM_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_001 | SCM-008 | AC1 | High |
| UT_SCM_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_002 | SCM-008 | AC1 | High |
| UT_SCM_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_003 | SCM-008 | AC1 | High |
| UT_SCM_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_004 | SCM-008 | AC2 | High |
| UT_SCM_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_005 | SCM-008 | AC2 | High |
| UT_SCM_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_006 | SCM-008 | AC3 | High |
| UT_SCM_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_007 | SCM-008 | AC3 | High |
| UT_SCM_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_008 | SCM-008 | AC4 | High |
| UT_SCM_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_009 | SCM-008 | AC5 | High |
| UT_SCM_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_010 | SCM-008 | AC1 | High |
| UT_SCM_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_011 | SCM-008 | AC2 | High |
| UT_SCM_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_012 | SCM-008 | AC4 | High |
| UT_SCM_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_013 | SCM-008 | AC5 | High |
| UT_SCM_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_014 | SCM-008 | AC2 | High |
| UT_SCM_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_015 | SCM-008 | AC5 | High |
| UT_SCM9_014 | missing_testlog | Execution log is missing for testcase ID: UT_SCM9_014 | SCM-009 | AC2 | Medium |
| UT_SCM9_015 | missing_testlog | Execution log is missing for testcase ID: UT_SCM9_015 | SCM-009 | AC5 | Medium |

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC2 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | Medium |
| TP_SCM8_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_001 | SCM-008 | AC1 | Medium |
| TP_SCM8_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_002 | SCM-008 | AC1 | Medium |
| TP_SCM8_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_003 | SCM-008 | AC1 | Medium |
| TP_SCM8_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_004 | SCM-008 | AC2 | Medium |
| TP_SCM8_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_005 | SCM-008 | AC2 | Medium |
| TP_SCM8_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_006 | SCM-008 | AC3 | Medium |
| TP_SCM8_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_007 | SCM-008 | AC3 | Medium |
| TP_SCM8_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_008 | SCM-008 | AC4 | Medium |
| TP_SCM8_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_009 | SCM-008 | AC5 | Medium |
| TP_SCM8_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_010 | SCM-008 | AC1 | Medium |
| TP_SCM8_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_011 | SCM-008 | AC2 | Medium |
| TP_SCM8_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_012 | SCM-008 | AC4 | Medium |
| TP_SCM8_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_013 | SCM-008 | AC5 | Medium |
| TP_SCM8_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_014 | SCM-008 | AC2 | Medium |
| TP_SCM8_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM8_015 | SCM-008 | AC5 | Medium |
| UT_SCM_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_001 | SCM-008 | AC1 | High |
| UT_SCM_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_002 | SCM-008 | AC1 | High |
| UT_SCM_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_003 | SCM-008 | AC1 | High |
| UT_SCM_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_004 | SCM-008 | AC2 | High |
| UT_SCM_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_005 | SCM-008 | AC2 | High |
| UT_SCM_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_006 | SCM-008 | AC3 | High |
| UT_SCM_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_007 | SCM-008 | AC3 | High |
| UT_SCM_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_008 | SCM-008 | AC4 | High |
| UT_SCM_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_009 | SCM-008 | AC5 | High |
| UT_SCM_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_010 | SCM-008 | AC1 | High |
| UT_SCM_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_011 | SCM-008 | AC2 | High |
| UT_SCM_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_012 | SCM-008 | AC4 | High |
| UT_SCM_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_013 | SCM-008 | AC5 | High |
| UT_SCM_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_014 | SCM-008 | AC2 | High |
| UT_SCM_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_SCM_015 | SCM-008 | AC5 | High |
| UT_SCM9_014 | missing_testlog | Execution log is missing for testcase ID: UT_SCM9_014 | SCM-009 | AC2 | Medium |
| UT_SCM9_015 | missing_testlog | Execution log is missing for testcase ID: UT_SCM9_015 | SCM-009 | AC5 | Medium |

## Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 135 |
| Total Test Logs | 133 |
| Missing Test Cases | 15 |
| Missing Test Logs | 21 |
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

**SCM-006:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCM-006 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCM-006 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |

**SCM-007:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCM-007 | Audit log authorization reference field empty when transfer initiated via bulk admin API |

**SCM-008:**

No defects reported for this User Story.

**SCM-009:**

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-CNS-001 | UT_SCM9_004 | SCM-009 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_SCM9_012 | SCM-009 | Push notification service ignores user preference flag |

## Conclusion

The report indicates outstanding coverage and execution issues that require remediation before progression. SCM-008 is not covered and multiple user stories have failed test cases and defects present.
