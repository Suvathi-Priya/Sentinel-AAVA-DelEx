# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 1 user story. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories. The user story SCM-007 forms the baseline for evaluation, with unit test coverage and execution records mapped to this user story serving as the foundation for this assessment.

## Test Coverage Summary

| User Story ID | Title | Total Acceptance Criteria | Fully Covered Acceptance Criteria | Partially Covered Acceptance Criteria | Not Covered Acceptance Criteria | Coverage Score Percentage |
|---|---|---:|---:|---:|---:|---:|
| SCM-007 | Subscription Transfer and Ownership Change | 5 | 2 | 2 | 1 | 40.00 |

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| SCM-007 | AC2 | No testcase explicitly validates that transfer details are included in the notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that incoming owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that transfers involving change in billing entity require compliance team approval. | Not Covered |
| SCM-007 | AC5 | No testcase explicitly validates that transfers involving change in tax jurisdiction require compliance team approval. | Not Covered |
| SCM-007 | AC5 | No testcase explicitly validates that compliance team approval is required before the transfer is completed. | Not Covered |

Coverage color indicators with icons:
- 🟢 Fully Covered
- 🟡 Partially Covered
- 🔴 Not Covered

## Test Execution Summary

| Test Case ID | Acceptance Criteria ID | Status | Actual Result | Defect ID & Description |
|---|---|---|---|---|
| TP_SCM7_001 | AC1 | Pass | Transfer request created successfully | NaN |
| TP_SCM7_002 | AC1 | Pass | Transfer effective date saved | NaN |
| TP_SCM7_003 | AC1 | Pass | Invalid new owner rejected by system | NaN |
| TP_SCM7_004 | AC2 | Pass | Current owner notified of transfer | NaN |
| TP_SCM7_005 | AC2 | Fail | New owner notification not sent in all transfer scenarios | DEF-SCM7-101 - New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| TP_SCM7_006 | AC2 | Pass | Effective date and billing detail present in notification | NaN |
| TP_SCM7_007 | AC3 | Pass | Transfer status visible to outgoing owner | NaN |
| TP_SCM7_008 | AC3 | Pass | Transfer status visible to incoming owner | NaN |
| TP_SCM7_009 | AC3 | Pass | Ownership history displayed in portal | NaN |
| TP_SCM7_010 | AC4 | Pass | Current and new owner IDs recorded | NaN |
| TP_SCM7_011 | AC4 | Pass | Subscription ID and transfer date recorded | NaN |
| TP_SCM7_012 | AC4 | Pass | Authorization reference and timestamp recorded | NaN |
| TP_SCM7_013 | AC5 | Pass | Compliance-sensitive transfer flagged correctly | NaN |
| TP_SCM7_014 | AC5 | Fail | Compliance team approval workflow not triggered for tax jurisdiction changes | DEF-SCM7-102 - Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| TP_SCM7_015 | AC5 | Pass | Transfer correctly held in pending state | NaN |

## Consistency Analysis

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| TP_SCM7_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_014 | SCM-007 | AC5 | High |
| TP_SCM7_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM7_015 | SCM-007 | AC5 | High |

| Metric | Count |
|---|---|
| Total Test Cases | 13 |
| Total Test Logs | 15 |
| Missing Test Cases | 2 |
| Missing Test Logs | 0 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_014 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |

## Conclusion

Remediation is required as user story SCM-007 contains acceptance criteria AC5 that is Not Covered, and defects exist in the test execution results. The unit test suite requires additional test cases to address coverage gaps and defect resolution before progression.
