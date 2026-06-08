# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 5 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. These user stories form the baseline for evaluation, with unit test cases linked to the identified user stories and defect data directly associated with these user stories included in the assessment.

## Test Coverage Summary

| User Story ID | Title | Total Acceptance Criterias | Fully Covered Acceptance Criterias | Partially Covered Acceptance Criterias | Not Covered Acceptance Criterias | Coverage Score Percentage | Total Test Cases in Test Plan | Total Test Cases in Test Logs | Total Passed | Total Failed | Total Defects |
|---------------|-------|----------------------------|------------------------------------|----------------------------------------|----------------------------------|---------------------------|-------------------------------|-------------------------------|--------------|--------------|---------------|
| SCM-006 | Subscription Downgrade Management | 5 | 3 | 2 | 0 | 60.00 | 15 | 13 | 12 | 1 | 1 |
| SCM-003 | Subscription Upgrade Request Processing | 5 | 3 | 2 | 0 | 60.00 | 15 | 15 | 13 | 2 | 2 |
| CLP-001 | Implement Customer Loyalty Points Service | 5 | 4 | 1 | 0 | 80.00 | 13 | 13 | 10 | 3 | 3 |
| ORM-001 | Implement Order Refund Management Service | 5 | 3 | 2 | 0 | 60.00 | 15 | 0 | 0 | 0 | 0 |
| SCM-004 | Subscription Cancellation Workflow | 5 | 0 | 0 | 5 | 0.00 | 0 | 15 | 13 | 2 | 2 |

| Metric | Value |
|--------|-------|
| Total User Stories | 5 |
| Total Fully Covered User Stories | 0 |
| Total Partially Covered User Stories | 4 |
| Total Not Covered User Stories | 1 |
| Total Acceptance Criterias in All User Stories | 25 |
| Fully Covered Acceptance Criterias in All User Stories | 11 |
| Partially Covered Acceptance Criterias in All User Stories | 9 |
| Not Covered Acceptance Criterias in All User Stories | 5 |
| Overall Coverage Score Percentage | 44.00 |
| Overall Coverage Score Formula | (Fully Covered Acceptance Criteria in All User Stories / Total Acceptance Criteria in All User Stories) × 100 |
| Overall Coverage Score Calculation | (11 / 25) × 100 = 44.00 |
| Total Test Cases in All Test Plan | 58 |
| Total Test Cases in All Test Logs | 56 |
| Total Passed in All Test Logs | 50 |
| Total Failed in All Test Logs | 6 |
| Total Defects in All Test Logs | 6 |
| Overall Defect Rate Percentage | 10.34 |
| Overall Defect Rate Formula | (Total Defects / Total Test Cases) × 100 |
| Overall Defect Rate Calculation | (6 / 58) × 100 = 10.34 |

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-006 | AC2 | No testcase explicitly validates that adjusted billing amount is included in downgrade confirmation notification. | Partially Covered |
| SCM-006 | AC4 | No testcase explicitly validates that effective date is captured in downgrade audit log. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates that revised billing amount is included in upgrade confirmation notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that subscription ID is captured in upgrade audit log. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that upgrade date is captured in upgrade audit log. | Partially Covered |
| CLP-001 | AC5 | No testcase explicitly validates that fraud review is required for reward redemptions above 5000 points. | Partially Covered |
| ORM-001 | AC4 | No testcase explicitly validates that approval timestamp is captured in refund audit log. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the threshold of refunds above $1000. | Partially Covered |
| SCM-004 | AC1 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC1 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC1 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC2 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC2 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC2 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC3 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC3 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC3 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC4 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC5 | No testcase mapped to validate this requirement. | Not Covered |
| SCM-004 | AC5 | No testcase mapped to validate this requirement. | Not Covered |

## Test Execution Summary

| Test Case ID | Status | Actual Result | Defects |
|--------------|--------|---------------|---------|
| TP_SCM6_001 | Pass | Downgrade request submitted successfully |  |
| TP_SCM6_002 | Pass | Effective date saved successfully |  |
| TP_SCM6_003 | Pass | Upgrade plan rejected in downgrade flow |  |
| TP_SCM6_004 | Pass | Downgrade confirmation notification sent |  |
| TP_SCM6_005 | Fail | Adjusted billing amount absent in downgrade notification | DEF-SCM6-101 |
| TP_SCM6_006 | Pass | Delivery log entry created |  |
| TP_SCM6_007 | Pass | Downgrade status displayed in portal |  |
| TP_SCM6_008 | Pass | Plan comparison displayed correctly |  |
| TP_SCM6_009 | Pass | Credit adjustment amount displayed |  |
| TP_SCM6_010 | Pass | Customer ID and subscription ID recorded |  |
| TP_SCM6_011 | Pass | Previous and downgraded plan recorded |  |
| TP_SCM6_012 | Pass | Credit issued and timestamp recorded |  |
| TP_SCM6_013 | Pass | Enterprise downgrade flagged correctly |  |
| TP_SCM3_001 | Pass | Upgrade request submitted successfully |  |
| TP_SCM3_002 | Pass | Preferred upgrade date captured successfully |  |
| TP_SCM3_003 | Pass | Invalid plan selection rejected with error |  |
| TP_SCM3_004 | Pass | Notification triggered after approval |  |
| TP_SCM3_005 | Fail | Revised billing amount missing in notification | DEF-SCM3-101 |
| TP_SCM3_006 | Pass | Delivery status recorded in system |  |
| TP_SCM3_007 | Pass | Upgrade request status displayed in portal |  |
| TP_SCM3_008 | Pass | Upgrade history list displayed correctly |  |
| TP_SCM3_009 | Pass | Next billing cycle change reflected in portal |  |
| TP_SCM3_010 | Pass | Customer ID recorded in audit log |  |
| TP_SCM3_011 | Pass | Previous and new plan recorded in audit log |  |
| TP_SCM3_012 | Pass | Timestamp recorded in audit log |  |
| TP_SCM3_013 | Pass | High-cost upgrade flagged by system |  |
| TP_SCM3_014 | Fail | Approval workflow not triggered for borderline 50% cases | DEF-SCM3-102 |
| TP_SCM3_015 | Pass | Manager notification generated |  |
| TP_SCM4_001 | Pass | Cancellation request submitted successfully |  |
| TP_SCM4_002 | Pass | Cancellation date saved successfully |  |
| TP_SCM4_003 | Pass | Empty reason rejected with validation error |  |
| TP_SCM4_004 | Pass | Cancellation confirmation notification sent |  |
| TP_SCM4_005 | Fail | Refund details missing from cancellation notification | DEF-SCM4-101 |
| TP_SCM4_006 | Pass | Delivery log entry created successfully |  |
| TP_SCM4_007 | Pass | Cancellation status displayed in portal |  |
| TP_SCM4_008 | Pass | Refund status displayed in portal |  |
| TP_SCM4_009 | Pass | Service end date displayed in portal |  |
| TP_SCM4_010 | Pass | Customer ID and subscription ID recorded |  |
| TP_SCM4_011 | Pass | Cancellation reason logged in audit |  |
| TP_SCM4_012 | Pass | Refund amount and timestamp recorded |  |
| TP_SCM4_013 | Pass | High balance cancellation flagged correctly |  |
| TP_SCM4_014 | Fail | Finance approval workflow not triggered consistently | DEF-SCM4-102 |
| TP_SCM4_015 | Pass | Cancellation held in pending state correctly |  |
| UT_CNS_001 | Pass | Email notification delivered |  |
| UT_CNS_002 | Pass | Email content generated |  |
| UT_CNS_003 | Pass | Delivery status recorded |  |
| UT_CNS_004 | Fail | SMS not delivered | DEF-CNS-001 |
| UT_CNS_005 | Pass | SMS content generated |  |
| UT_CNS_006 | Fail | Delivery status unavailable | DEF-CNS-002 |
| UT_CNS_007 | Pass | Enable preference saved |  |
| UT_CNS_008 | Pass | Disable preference saved |  |
| UT_CNS_009 | Fail | Push notification not dispatched | DEF-CNS-003 |
| UT_CNS_010 | Pass | Customer ID logged |  |
| UT_CNS_011 | Pass | Notification type logged |  |
| UT_CNS_012 | Pass | Log record created |  |
| UT_CNS_013 | Pass | Retry initiated |  |
| UT_CLP_001 | Passed | Points awarded successfully |  |
| UT_CLP_002 | Passed | Correct points calculated |  |
| UT_CLP_003 | Failed | Points posting delayed | DEF-CLP-001 |
| UT_CLP_004 | Passed | Reward redeemed successfully |  |
| UT_CLP_005 | Passed | Points deducted correctly |  |
| UT_CLP_006 | Passed | Reward issued successfully |  |
| UT_CLP_007 | Passed | Balance displayed correctly |  |
| UT_CLP_008 | Failed | Balance refresh issue observed | DEF-CLP-002 |
| UT_CLP_009 | Passed | Balance updated after redemption |  |
| UT_CLP_010 | Passed | Customer ID logged |  |
| UT_CLP_011 | Passed | Points value logged |  |
| UT_CLP_012 | Passed | Timestamp logged |  |
| UT_CLP_013 | Passed | Manager approval validated |  |
| UT_CLP_014 | Passed | Fraud review validated |  |
| UT_CLP_015 | Failed | High value workflow validation failed | DEF-CLP-003 |

## Consistency Analysis

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM6_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_014 | SCM-006 | AC5 | Medium |
| TP_SCM6_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM6_015 | SCM-006 | AC5 | Medium |
| TP_SCM4_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_001 | SCM-004 | AC1 | High |
| TP_SCM4_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_002 | SCM-004 | AC1 | High |
| TP_SCM4_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_003 | SCM-004 | AC1 | High |
| TP_SCM4_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_004 | SCM-004 | AC2 | High |
| TP_SCM4_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_005 | SCM-004 | AC2 | High |
| TP_SCM4_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_006 | SCM-004 | AC2 | High |
| TP_SCM4_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_007 | SCM-004 | AC3 | High |
| TP_SCM4_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_008 | SCM-004 | AC3 | High |
| TP_SCM4_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_009 | SCM-004 | AC3 | High |
| TP_SCM4_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_010 | SCM-004 | AC4 | High |
| TP_SCM4_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_011 | SCM-004 | AC4 | High |
| TP_SCM4_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_012 | SCM-004 | AC4 | High |
| TP_SCM4_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_013 | SCM-004 | AC5 | High |
| TP_SCM4_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC5 | High |
| TP_SCM4_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 | AC5 | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 | AC5 | High |
| UT_ORM_001 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_001 | ORM-001 | AC1 | Medium |
| UT_ORM_002 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_002 | ORM-001 | AC1 | Medium |
| UT_ORM_003 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_003 | ORM-001 | AC1 | Medium |
| UT_ORM_004 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_004 | ORM-001 | AC2 | Medium |
| UT_ORM_005 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_005 | ORM-001 | AC2 | Medium |
| UT_ORM_006 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_006 | ORM-001 | AC2 | Medium |
| UT_ORM_007 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_007 | ORM-001 | AC3 | Medium |
| UT_ORM_008 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_008 | ORM-001 | AC3 | Medium |
| UT_ORM_009 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_009 | ORM-001 | AC3 | Medium |
| UT_ORM_010 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_010 | ORM-001 | AC4 | Medium |
| UT_ORM_011 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_011 | ORM-001 | AC4 | Medium |
| UT_ORM_012 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_012 | ORM-001 | AC4 | Medium |
| UT_ORM_013 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_013 | ORM-001 | AC5 | Medium |
| UT_ORM_014 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_014 | ORM-001 | AC5 | Medium |
| UT_ORM_015 | missing_testlog | Execution log is missing for testcase ID: UT_ORM_015 | ORM-001 | AC5 | Medium |

| Metric | Count |
|--------|-------|
| Total Test Cases | 73 |
| Total Test Logs | 71 |
| Missing Test Cases | 17 |
| Missing Test Logs | 17 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|--------------------|
| DEF-SCM6-101 | TP_SCM6_005 | SCM-006 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |

## Conclusion

Remediation is required as user story SCM-004 is Not Covered and multiple test case failures and defects exist across the evaluated user stories.
