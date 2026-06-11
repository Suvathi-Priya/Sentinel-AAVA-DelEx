<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 6 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 6, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

# Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-001 | AC5 | No testcase explicitly validates the $1000 threshold condition for high-value refunds. | Partially Covered |
| SCM-002 | AC2 | No testcase explicitly validates that resume date is included in the pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that scheduled resume date is viewable in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that pause start date is captured in the audit log. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates the 90-day threshold condition for pause requests. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates that revised billing amount is included in the upgrade confirmation notification. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates that next billing cycle changes are viewable in the customer portal. | Partially Covered |
| SCM-003 | AC5 | No testcase explicitly validates the price increase greater than 50% threshold condition.; No testcase explicitly validates that manager approval is required before upgrade activation for price increases greater than 50%. | Not Covered |
| SCM-004 | AC5 | No testcase explicitly validates the outstanding balance greater than $500 threshold condition.; No testcase explicitly validates that finance team approval is required before cancellation processing for outstanding balances greater than $500. | Not Covered |
| SCM-005 | AC5 | No testcase explicitly validates the $10,000 threshold condition for high-value subscriptions. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that customer ID is captured in the downgrade audit log.; No testcase explicitly validates that subscription ID is captured in the downgrade audit log.; No testcase explicitly validates that previous plan is captured in the downgrade audit log.; No testcase explicitly validates that downgraded plan is captured in the downgrade audit log.; No testcase explicitly validates that effective date is captured in the downgrade audit log.; No testcase explicitly validates that credit issued is captured in the downgrade audit log.; No testcase explicitly validates that timestamp is captured in the downgrade audit log. | Not Covered |
| SCM-006 | AC5 | No testcase explicitly validates that customer retention review is required before processing enterprise-tier downgrades. | Partially Covered |

# Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | NULL | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | NULL | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 90 |
| Total Test Logs | 88 |
| Missing Test Cases | 0 |
| Missing Test Logs | 2 |
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

# Conclusion

Remediation is required as multiple user stories have coverage gaps and 15 defects exist across the test suite.
