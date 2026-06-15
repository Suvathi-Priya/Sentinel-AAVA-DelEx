<div align="center"><strong><span style="font-size:28px;">UNIT TEST QUALITY & COVERAGE REPORT</span></strong></div>

# Scope

This report evaluates unit test coverage and quality across 9 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

The 9 user stories form the baseline for evaluation, covering unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

# Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-001 | AC4 | No testcase explicitly validates approval timestamp capture. | Partially Covered |
| SCM-001 | AC5 | No testcase explicitly validates fraud review requirement. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates inclusion of resume date in the notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date visibility in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in the audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval occurs before pause activation. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates next billing cycle changes visibility in the customer portal. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates upgrade date capture in the audit log. | Partially Covered |
| SCM-003 | AC5 | No testcase explicitly validates that manager approval occurs before upgrade activation. | Partially Covered |
| SCM-004 | AC4 | No testcase explicitly validates cancellation reason capture in the audit log. | Partially Covered |
| SCM-004 | AC5 | No testcase explicitly validates that finance approval occurs before cancellation processing. | Partially Covered |
| SCM-005 | AC4 | No testcase explicitly validates reminder date capture in the reminder log.; No testcase explicitly validates channel used capture in the reminder log. | Partially Covered |
| SCM-005 | AC5 | No testcase explicitly validates reminders for subscriptions with annual value greater than $10,000.; No testcase explicitly validates sending reminders to the assigned account manager for high-value subscriptions. | Partially Covered |
| SCM-006 | AC2 | No testcase explicitly validates adjusted billing amount in the downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates previous plan capture in the audit log.; No testcase explicitly validates downgraded plan capture in the audit log.; No testcase explicitly validates effective date capture in the audit log.; No testcase explicitly validates timestamp capture in the audit log. | Partially Covered |
| SCM-006 | AC5 | No testcase explicitly validates customer retention review requirement. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates inclusion of transfer details in the notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates billing change summary visibility in the customer portal. | Partially Covered |
| SCM-007 | AC4 | No testcase explicitly validates subscription ID capture in the audit log.; No testcase explicitly validates transfer date capture in the audit log.; No testcase explicitly validates timestamp capture in the audit log. | Partially Covered |
| SCM-008 | AC4 | No testcase explicitly validates transaction timestamp capture in the loyalty transaction log. | Partially Covered |
| SCM-008 | AC5 | No testcase explicitly validates fraud review requirement. | Partially Covered |

# Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | NULL | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | NULL | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | NULL | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | NULL | Medium |
| TP_SCM8_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM8_014 | SCM-008 | NULL | High |
| TP_SCM8_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM8_015 | SCM-008 | NULL | High |
| UT_SCM9_014 | missing_testlog | Execution log is missing for testcase ID: UT_SCM9_014 | SCM-009 | NULL | Medium |
| UT_SCM9_015 | missing_testlog | Execution log is missing for testcase ID: UT_SCM9_015 | SCM-009 | NULL | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 135 |
| Total Test Logs | 131 |
| Missing Test Cases | 2 |
| Missing Test Logs | 6 |
| Consistency Status | Mismatch Detected |

# Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-ORM-001 | UT_SCM1_005 | SCM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_SCM1_009 | SCM-001 | Refund workflow synchronization error |
| DEF-SCM-101 | TP_SCM_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_009 | SCM-002 | Activation allowed without completed approval |
| DEF-SCM3-101 | TP_SCM3_004 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM4-101 | TP_SCM4_004 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_009 | SCM-004 | Finance team approval workflow fails for mixed currency outstanding balances |
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-103 | TP_SCM5_011 | SCM-005 | System sends reminder even when subscription expiry date is null |
| DEF-SCM5-104 | TP_SCM5_013 | SCM-005 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |
| DEF-SCM5-105 | TP_SCM5_015 | SCM-005 | Reminder log delivery status remains blank when notification channel fails |
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCM-006 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCM-006 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCM-007 | Audit log authorization reference field empty when transfer initiated via bulk admin API |
| DEF-SCM7-101 | TP_SCM7_015 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-CLP-001 | TP_SCM8_003 | SCM-008 | Points posting service delay |
| DEF-CLP-002 | TP_SCM8_007 | SCM-008 | Balance refresh cache issue |
| DEF-CLP-003 | TP_SCM8_009 | SCM-008 | Redemption workflow synchronization issue |
| DEF-CNS-001 | UT_SCM9_004 | SCM-009 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_SCM9_012 | SCM-009 | Push notification service ignores user preference flag |

# Conclusion

Remediation is required. Multiple user stories have partial coverage gaps and 24 defects exist across the test suite that require resolution before progression.
