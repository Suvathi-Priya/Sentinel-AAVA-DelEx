# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 8 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The 8 user stories form the baseline for evaluation, covering unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| SCM-001 | AC5 | No testcase explicitly validates fraud review. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in the notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in the audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval occurs before pause activation. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates next billing cycle changes visibility in the customer portal. | Partially Covered |
| SCM-003 | AC5 | No testcase explicitly validates that manager approval occurs before upgrade activation. | Partially Covered |
| SCM-004 | AC5 | No testcase explicitly validates that finance team approval occurs before cancellation processing. | Partially Covered |
| SCM-005 | AC3 | No testcase explicitly validates renewal preferences visibility in the customer portal. | Partially Covered |
| SCM-005 | AC4 | No testcase explicitly validates reminder date capture in the reminder log.; No testcase explicitly validates channel used capture in the reminder log. | Partially Covered |
| SCM-005 | AC5 | No testcase explicitly validates reminder delivery to the assigned account manager for high-value subscriptions. | Partially Covered |
| SCM-006 | AC2 | No testcase explicitly validates adjusted billing amount in the downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates previous plan capture in the audit log.; No testcase explicitly validates downgraded plan capture in the audit log.; No testcase explicitly validates effective date capture in the audit log.; No testcase explicitly validates timestamp capture in the audit log. | Partially Covered |
| SCM-006 | AC5 | No testcase explicitly validates customer retention review. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates transfer details inclusion in the notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates billing change summary visibility in the customer portal. | Partially Covered |
| SCM-007 | AC4 | No testcase explicitly validates subscription ID capture in the audit log.; No testcase explicitly validates transfer date capture in the audit log.; No testcase explicitly validates timestamp capture in the audit log. | Partially Covered |
| SCM-008 | AC4 | No testcase explicitly validates transaction timestamp capture. | Partially Covered |
| SCM-008 | AC5 | No testcase explicitly validates fraud review. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |
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

### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 120 |
| Total Test Logs | 118 |
| Missing Test Cases | 15 |
| Missing Test Logs | 17 |
| Consistency Status | Mismatch Detected |

## Defect Details

### SCM-001 - Implement Order Refund Management Service

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-ORM-001 | UT_SCM1_005 | SCM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_SCM1_009 | SCM-001 | Refund workflow synchronization error |

### SCM-002 - Subscription Pause Management Service

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM-101 | TP_SCM_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_009 | SCM-002 | Activation allowed without completed approval |

### SCM-003 - Subscription Upgrade Request Processing

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM3-101 | TP_SCM3_004 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |

### SCM-004 - Subscription Cancellation Workflow

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM4-101 | TP_SCM4_004 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_009 | SCM-004 | Finance team approval workflow fails for mixed currency outstanding balances |

### SCM-005 - Subscription Renewal Reminder Service

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-103 | TP_SCM5_011 | SCM-005 | System sends reminder even when subscription expiry date is null |
| DEF-SCM5-104 | TP_SCM5_013 | SCM-005 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |
| DEF-SCM5-105 | TP_SCM5_015 | SCM-005 | Reminder log delivery status remains blank when notification channel fails |

### SCM-006 - Subscription Downgrade Management

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCM-006 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCM-006 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |

### SCM-007 - Subscription Transfer and Ownership Change

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-101 | TP_SCM7_015 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCM-007 | Audit log authorization reference field empty when transfer initiated via bulk admin API |

### SCM-008 - Implement Customer Loyalty Points Service

No defects reported for this User Story.

## Conclusion

Remediation is required. Multiple user stories have partial coverage gaps, failed test cases exist, and defects are present across 7 of 8 user stories requiring resolution before progression.
