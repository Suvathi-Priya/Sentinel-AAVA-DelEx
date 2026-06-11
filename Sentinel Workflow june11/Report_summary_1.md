# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 6 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-002 | AC2 | No testcase explicitly validates resume date inclusion in pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates scheduled resume date viewing in customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates pause start date capture in audit log. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates next billing cycle changes viewing in customer portal. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates customer ID capture in upgrade audit log.; No testcase explicitly validates subscription ID capture in upgrade audit log.; No testcase explicitly validates previous plan capture in upgrade audit log.; No testcase explicitly validates new plan capture in upgrade audit log.; No testcase explicitly validates upgrade date capture in upgrade audit log.; No testcase explicitly validates timestamp capture in upgrade audit log. | Not Covered |
| SCM-003 | AC5 | No testcase explicitly validates upgrade requests with price increase greater than 50%.; No testcase explicitly validates manager approval requirement before upgrade activation for price increase greater than 50%. | Not Covered |
| SCM-004 | AC4 | No testcase explicitly validates customer ID capture in cancellation audit log.; No testcase explicitly validates subscription ID capture in cancellation audit log.; No testcase explicitly validates cancellation reason capture in cancellation audit log.; No testcase explicitly validates effective date capture in cancellation audit log.; No testcase explicitly validates refund amount capture in cancellation audit log.; No testcase explicitly validates timestamp capture in cancellation audit log. | Not Covered |
| SCM-004 | AC5 | No testcase explicitly validates cancellation requests with outstanding balances greater than $500.; No testcase explicitly validates finance team approval requirement before cancellation processing for outstanding balances greater than $500. | Not Covered |
| SCM-006 | AC4 | No testcase explicitly validates customer ID capture in downgrade audit log.; No testcase explicitly validates subscription ID capture in downgrade audit log.; No testcase explicitly validates previous plan capture in downgrade audit log.; No testcase explicitly validates downgraded plan capture in downgrade audit log.; No testcase explicitly validates effective date capture in downgrade audit log.; No testcase explicitly validates credit issued capture in downgrade audit log.; No testcase explicitly validates timestamp capture in downgrade audit log. | Not Covered |
| SCM-006 | AC5 | No testcase explicitly validates customer retention review requirement before processing enterprise-tier downgrades. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | NULL | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | NULL | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | NULL | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | NULL | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 90 |
| Total Test Logs | 86 |
| Missing Test Cases | 0 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

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

## Conclusion

Remediation is required as multiple user stories have coverage gaps and 17 defects exist across the test execution results.
