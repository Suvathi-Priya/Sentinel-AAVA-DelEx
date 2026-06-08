# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories. The scope is restricted to test plans and execution records mapped to these user stories. The baseline for evaluation consists of SCM-006 (Subscription Downgrade Management), SCM-007 (Subscription Transfer and Ownership Change), and CNS-001 (Implement Customer Notification Service), which form the reference for measuring coverage, execution success, and defect quality. Analysis excludes non-unit test activities and unrelated defect categories.

## Test Coverage Summary

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates that the adjusted billing amount is detailed in the downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that the effective date is captured in the downgrade audit log. | Partially Covered |
| SCM-007 | AC1 | No testcase explicitly validates that administrators can initiate a subscription transfer by specifying the current owner. | Not Covered |
| SCM-007 | AC1 | No testcase explicitly validates that administrators can initiate a subscription transfer by specifying the new owner. | Not Covered |
| SCM-007 | AC1 | No testcase explicitly validates that administrators can initiate a subscription transfer by specifying the transfer effective date. | Not Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer notification is sent to the current owner. | Not Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer notification is sent to the new owner. | Not Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer details are included in the transfer notification. | Not Covered |
| SCM-007 | AC2 | No testcase explicitly validates that effective date is included in the transfer notification. | Not Covered |
| SCM-007 | AC2 | No testcase explicitly validates that new billing responsibility is included in the transfer notification. | Not Covered |
| SCM-007 | AC3 | No testcase explicitly validates that the outgoing owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that the incoming owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that subscription transfers involving a change in billing entity require compliance team approval before the transfer is completed. | Not Covered |
| SCM-007 | AC5 | No testcase explicitly validates that subscription transfers involving a change in tax jurisdiction require compliance team approval before the transfer is completed. | Not Covered |
| CNS-001 | AC1 | No testcase explicitly validates that the system sends email notifications for all completed transactions. | Not Covered |
| CNS-001 | AC2 | No testcase explicitly validates that SMS notifications are sent for high-priority alerts. | Not Covered |
| CNS-001 | AC3 | No testcase explicitly validates that push notifications are configurable per user preference. | Not Covered |
| CNS-001 | AC4 | No testcase explicitly validates that timestamp is captured in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates that failed notifications trigger retry attempts up to 3 times. | Not Covered |

## Test Execution Summary

| Test Case ID | Status | Actual Result | Defects |
|--------------|--------|---------------|---------|
| TP_SCM6_001 | Pass | Downgrade request submitted successfully | None |
| TP_SCM6_002 | Pass | Effective date saved successfully | None |
| TP_SCM6_003 | Pass | Upgrade plan rejected in downgrade flow | None |
| TP_SCM6_004 | Pass | Downgrade confirmation notification sent | None |
| TP_SCM6_005 | Fail | Adjusted billing amount absent in downgrade notification | DEF-SCM6-101 |
| TP_SCM6_006 | Pass | Delivery log entry created | None |
| TP_SCM6_007 | Pass | Downgrade status displayed in portal | None |
| TP_SCM6_008 | Pass | Plan comparison displayed correctly | None |
| TP_SCM6_009 | Pass | Credit adjustment amount displayed | None |
| TP_SCM6_010 | Pass | Customer ID and subscription ID recorded | None |
| TP_SCM6_011 | Pass | Previous and downgraded plan recorded | None |
| TP_SCM6_012 | Pass | Credit issued and timestamp recorded | None |
| TP_SCM6_013 | Pass | Enterprise downgrade flagged correctly | None |
| TP_SCM7_001 | Pass | Transfer request created successfully | None |
| TP_SCM7_002 | Pass | Transfer effective date saved | None |
| TP_SCM7_003 | Pass | Invalid new owner rejected by system | None |
| TP_SCM7_004 | Pass | Current owner notified of transfer | None |
| TP_SCM7_005 | Fail | New owner notification not sent in all transfer scenarios | DEF-SCM7-101 |
| TP_SCM7_006 | Pass | Effective date and billing detail present in notification | None |
| TP_SCM7_007 | Pass | Transfer status visible to outgoing owner | None |
| TP_SCM7_008 | Pass | Transfer status visible to incoming owner | None |
| TP_SCM7_009 | Pass | Ownership history displayed in portal | None |
| TP_SCM7_010 | Pass | Current and new owner IDs recorded | None |
| TP_SCM7_011 | Pass | Subscription ID and transfer date recorded | None |
| TP_SCM7_012 | Pass | Authorization reference and timestamp recorded | None |
| TP_SCM7_013 | Pass | Compliance-sensitive transfer flagged correctly | None |
| TP_SCM7_014 | Fail | Compliance team approval workflow not triggered for tax jurisdiction changes | DEF-SCM7-102 |
| TP_SCM7_015 | Pass | Transfer correctly held in pending state | None |
| UT_CNS_001 | Pass | Email notification delivered | None |
| UT_CNS_002 | Pass | Email content generated | None |
| UT_CNS_003 | Pass | Delivery status recorded | None |
| UT_CNS_004 | Fail | SMS not delivered | DEF-CNS-001 |
| UT_CNS_005 | Pass | SMS content generated | None |
| UT_CNS_006 | Fail | Delivery status unavailable | DEF-CNS-002 |
| UT_CNS_007 | Pass | Enable preference saved | None |
| UT_CNS_008 | Pass | Disable preference saved | None |
| UT_CNS_009 | Fail | Push notification not dispatched | DEF-CNS-003 |
| UT_CNS_010 | Pass | Customer ID logged | None |
| UT_CNS_011 | Pass | Notification type logged | None |
| UT_CNS_012 | Pass | Log record created | None |
| UT_CNS_013 | Pass | Retry initiated | None |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| TP_SCM7_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_001 | SCM-007 | AC1 | High |
| TP_SCM7_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_002 | SCM-007 | AC1 | High |
| TP_SCM7_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_003 | SCM-007 | AC1 | High |
| TP_SCM7_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_004 | SCM-007 | AC2 | High |
| TP_SCM7_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_005 | SCM-007 | AC2 | High |
| TP_SCM7_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_006 | SCM-007 | AC2 | High |
| TP_SCM7_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_014 | SCM-007 | AC5 | High |
| TP_SCM7_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_015 | SCM-007 | AC5 | High |
| UT_CNS_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_001 | CNS-001 | AC1 | High |
| UT_CNS_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_002 | CNS-001 | AC1 | High |
| UT_CNS_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_003 | CNS-001 | AC1 | High |
| UT_CNS_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_004 | CNS-001 | AC2 | High |
| UT_CNS_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_005 | CNS-001 | AC2 | High |
| UT_CNS_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_006 | CNS-001 | AC2 | High |
| UT_CNS_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_007 | CNS-001 | AC3 | High |
| UT_CNS_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CNS_008 | CNS-001 | AC3 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 29 |
| Total Test Logs | 41 |
| Missing Test Cases | 16 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Title | Defect Description |
|-----------|--------------|---------------|--------------|--------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | NULL | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | NULL | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | NULL | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | NULL | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | NULL | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | NULL | Push notification service unavailable |

## Conclusion

Remediation is required as multiple user stories are Not Covered and defects exist in the test execution results.
