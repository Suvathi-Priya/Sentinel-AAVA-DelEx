<div align="center"><strong><span style="font-size:24px;">UNIT TEST QUALITY & COVERAGE REPORT</span></strong></div>

# Scope

This report evaluates unit test coverage and quality across 6 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

The baseline for evaluation consists of:
- SCM-006: Subscription Downgrade Management
- SCM-005: Subscription Renewal Reminder Service  
- SCM-004: Subscription Cancellation Workflow
- SCM-003: Subscription Upgrade Request Processing
- SCM-002: Subscription Pause Management Service
- SCM-001: Implement Order Refund Management Service

# Test Coverage Summary

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates that adjusted billing amount is included in downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that previous plan is captured in downgrade audit log.; No testcase explicitly validates that downgraded plan is captured in downgrade audit log.; No testcase explicitly validates that effective date is captured in downgrade audit log.; No testcase explicitly validates that timestamp is captured in downgrade audit log. | Partially Covered |
| SCM-006 | AC5 | No testcase explicitly validates that customer retention review is required for enterprise-tier plan downgrades. | Partially Covered |
| SCM-005 | AC4 | No testcase explicitly validates that reminder date is captured in renewal reminder log.; No testcase explicitly validates that channel used is captured in renewal reminder log. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates that next billing cycle changes are viewable in the customer portal. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates that resume date is included in pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that scheduled resume date is viewable in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that pause start date is captured in pause audit log. | Partially Covered |
| SCM-001 | AC5 | No testcase explicitly validates that fraud review is required for high-value refunds above $1000. | Partially Covered |

# Consistency Analysis

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC2 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | Medium |
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |
| TP_SCM2_004 | invalid_mapping | Acceptance criterion AC2 requires pause start date and resume date in notification, but available planned and executed coverage only explicitly validates pause start date; resume date coverage is not explicitly traceable. | SCM-002 | AC2 | Medium |
| TP_SCM2_008 | invalid_mapping | Acceptance criterion AC4 requires audit log to capture customer ID, subscription ID, pause reason, pause start date, and timestamp, but testcase TP_SCM2_008 only explicitly references customer ID, subscription ID, pause reason, and timestamp; pause start date is not explicitly traceable in the testcase description. | SCM-002 | AC4 | Low |
| TP_SCM1_009 | invalid_mapping | Acceptance criterion AC5 requires both manager approval and fraud review for high-value refunds above $1000, but mapped testcase coverage explicitly validates manager approval workflow only; fraud review traceability is not explicit. | SCM-001 | AC5 | Medium |

## Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 90 |
| Total Test Logs | 86 |
| Missing Test Cases | 0 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

# Defect Details

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCM-006 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCM-006 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |
| DEF-SCM5-103 | TP_SCM5_011 | SCM-005 | System sends reminder even when subscription expiry date is null |
| DEF-SCM5-101 | TP_SCM5_005 | SCM-005 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-105 | TP_SCM5_015 | SCM-005 | Reminder log delivery status remains blank when notification channel fails |
| DEF-SCM5-104 | TP_SCM5_013 | SCM-005 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |
| DEF-SCM4-101 | TP_SCM4_004 | SCM-004 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_009 | SCM-004 | Finance team approval workflow fails for mixed currency outstanding balances |
| DEF-SCM3-101 | TP_SCM3_004 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM2-101 | TP_SCM2_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM2-102 | TP_SCM2_009 | SCM-002 | Activation allowed without completed approval |
| DEF-SCM1-001 | TP_SCM1_005 | SCM-001 | Notification template rendering issue |
| DEF-SCM1-002 | TP_SCM1_009 | SCM-001 | Refund workflow synchronization error |

# Conclusion

Remediation is required as multiple user stories have coverage gaps, test case failures, and defects present. The report identifies 9 coverage gaps across 5 user stories, 4 missing test logs, and 15 defects requiring resolution before progression.
