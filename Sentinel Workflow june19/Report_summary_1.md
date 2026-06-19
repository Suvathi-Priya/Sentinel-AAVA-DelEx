<div align="center"><strong><span style="font-size:24px;">UNIT TEST QUALITY & COVERAGE REPORT</span></strong></div>

# Scope

This report evaluates unit test coverage and quality across 7 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories.

# Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| 1846 | AC3 | No testcase explicitly validates viewing next billing cycle changes in the customer portal. | Partially Covered |
| 1852 | AC2 | No testcase explicitly validates that adjusted billing amount is included in downgrade confirmation notification. | Partially Covered |
| 1852 | AC4 | No testcase explicitly validates capture of previous plan in downgrade audit log.; No testcase explicitly validates capture of downgraded plan in downgrade audit log.; No testcase explicitly validates capture of effective date in downgrade audit log.; No testcase explicitly validates capture of credit issued in downgrade audit log.; No testcase explicitly validates capture of timestamp in downgrade audit log. | Partially Covered |
| 1852 | AC5 | No testcase explicitly validates that customer retention review is required before enterprise downgrade is processed. | Partially Covered |
| 1836 | AC5 | No testcase explicitly validates that fraud review is required for high-value refunds above $1000. | Partially Covered |
| 1850 | AC4 | No testcase explicitly validates capture of reminder date in renewal reminder logs.; No testcase explicitly validates capture of channel used in renewal reminder logs.; No testcase explicitly validates capture of delivery status in renewal reminder logs. | Partially Covered |
| 1850 | AC5 | No testcase explicitly validates identification of high-value subscriptions with annual value greater than $10,000.; No testcase explicitly validates sending reminders to the customer for high-value subscriptions.; No testcase explicitly validates sending reminders to the assigned account manager for high-value subscriptions. | Not Covered |
| 1854 | AC2 | No testcase explicitly validates that transfer details are included in transfer notification. | Partially Covered |
| 1854 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in the customer portal.; No testcase explicitly validates that incoming owner can view billing change summary in the customer portal. | Partially Covered |
| 1854 | AC4 | No testcase explicitly validates capture of subscription ID in transfer audit log.; No testcase explicitly validates capture of transfer date in transfer audit log.; No testcase explicitly validates capture of authorization reference in transfer audit log.; No testcase explicitly validates capture of timestamp in transfer audit log. | Partially Covered |
| 1854 | AC5 | No testcase explicitly validates identification of subscription transfers involving a change in billing entity.; No testcase explicitly validates identification of subscription transfers involving a change in tax jurisdiction. | Partially Covered |
| 1844 | AC2 | No testcase explicitly validates that resume date is included in pause confirmation notification. | Partially Covered |
| 1844 | AC3 | No testcase explicitly validates that scheduled resume date is viewable in the customer portal. | Partially Covered |
| 1844 | AC4 | No testcase explicitly validates capture of pause start date in pause audit log. | Partially Covered |

# Consistency Analysis

## Data Mapping Inconsistency Details

No mapping inconsistencies detected.

## Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 105 |
| Total Test Logs | 103 |
| Missing Test Cases | 0 |
| Missing Test Logs | 2 |
| Consistency Status | NULL |

# Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM3-101 | TP_SCM3_004 | 1846 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | 1846 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM6-101 | TP_SCM6_005 | 1852 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | 1852 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | 1852 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |
| DEF-SCM4-101 | TP_SCM4_004 | 1848 | Applicable refund details not included in cancellation confirmation notification |
| DEF-SCM4-102 | TP_SCM4_009 | 1848 | Finance team approval workflow fails for mixed currency outstanding balances |
| DEF-SCM1-002 | TP_SCM1_009 | 1836 | Refund workflow synchronization error |
| DEF-SCM5-101 | TP_SCM5_005 | 1850 | Renewal amount not populated in 30-day reminder notification for monthly billing plans |
| DEF-SCM5-104 | TP_SCM5_013 | 1850 | Boundary condition error: $10,000 subscription flagged as high-value instead of requiring value >$10,000 |
| DEF-SCM5-105 | TP_SCM5_015 | 1850 | Reminder log delivery status remains blank when notification channel fails |
| DEF-SCM7-101 | TP_SCM7_005 | 1854 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | 1854 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | 1854 | Audit log authorization reference field empty when transfer initiated via bulk admin API |
| DEF-SCM2-101 | TP_SCM2_008 | 1844 | Pause reason not captured consistently |
| DEF-SCM2-102 | TP_SCM2_009 | 1844 | Activation allowed without completed approval |

# Conclusion

Remediation is required as multiple test cases have failed and defects exist across all user stories. The report indicates outstanding coverage gaps and execution issues that must be addressed before progression.
