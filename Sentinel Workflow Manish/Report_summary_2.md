<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 9 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories. The user stories form the baseline for measuring coverage, execution success, and defect quality.

# Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM8 | AC5 | No testcase explicitly validates fraud review requirement for redemptions above 5000 points. | Partially Covered |
| SCRUM-58 | AC2 | No testcase explicitly validates that transfer details are included in notification. | Partially Covered |
| SCRUM-58 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in customer portal.; No testcase explicitly validates that incoming owner can view billing change summary in customer portal. | Partially Covered |
| SCRUM-58 | AC4 | No testcase explicitly validates that subscription ID is captured in transfer audit log.; No testcase explicitly validates that transfer date is captured in transfer audit log.; No testcase explicitly validates that timestamp is captured in transfer audit log. | Partially Covered |
| SCRUM-58 | AC5 | No testcase explicitly validates that transfers involving change in billing entity require compliance team approval. | Partially Covered |
| SCRUM-56 | AC2 | No testcase explicitly validates that adjusted billing amount is included in downgrade confirmation notification. | Partially Covered |
| SCRUM-56 | AC4 | No testcase explicitly validates that previous plan is captured in downgrade audit log.; No testcase explicitly validates that downgraded plan is captured in downgrade audit log.; No testcase explicitly validates that effective date is captured in downgrade audit log.; No testcase explicitly validates that credit issued is captured in downgrade audit log.; No testcase explicitly validates that timestamp is captured in downgrade audit log. | Partially Covered |
| SCRUM-56 | AC5 | No testcase explicitly validates that downgrade requests from enterprise-tier plans require customer retention review. | Partially Covered |

# Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| UT_SCM8_001 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_001 but corresponding test plan uses TP_SCM8_001 for story SCM-008. | SCM8 | AC1 | High |
| UT_SCM8_002 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_002 but corresponding test plan uses TP_SCM8_002 for story SCM-008. | SCM8 | AC1 | High |
| UT_SCM8_003 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_003 but corresponding test plan uses TP_SCM8_003 for story SCM-008. | SCM8 | AC1 | High |
| UT_SCM8_004 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_004 but corresponding test plan uses TP_SCM8_004 for story SCM-008. | SCM8 | AC2 | High |
| UT_SCM8_005 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_005 but corresponding test plan uses TP_SCM8_005 for story SCM-008. | SCM8 | AC2 | High |
| UT_SCM8_006 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_006 but corresponding test plan uses TP_SCM8_006 for story SCM-008. | SCM8 | AC3 | High |
| UT_SCM8_007 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_007 but corresponding test plan uses TP_SCM8_007 for story SCM-008. | SCM8 | AC3 | High |
| UT_SCM8_008 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_008 but corresponding test plan uses TP_SCM8_008 for story SCM-008. | SCM8 | AC4 | High |
| UT_SCM8_009 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_009 but corresponding test plan uses TP_SCM8_009 for story SCM-008. | SCM8 | AC5 | High |
| UT_SCM8_010 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_010 but corresponding test plan uses TP_SCM8_010 for story SCM-008. | SCM8 | AC1 | High |
| UT_SCM8_011 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_011 but corresponding test plan uses TP_SCM8_011 for story SCM-008. | SCM8 | AC2 | High |
| UT_SCM8_012 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_012 but corresponding test plan uses TP_SCM8_012 for story SCM-008. | SCM8 | AC4 | High |
| UT_SCM8_013 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_013 but corresponding test plan uses TP_SCM8_013 for story SCM-008. | SCM8 | AC5 | High |
| UT_SCM8_014 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_014 but corresponding test plan uses TP_SCM8_014 for story SCM-008. | SCM8 | AC2 | High |
| UT_SCM8_015 | invalid_mapping | Test execution record uses testcase ID UT_SCM8_015 but corresponding test plan uses TP_SCM8_015 for story SCM-008. | SCM8 | AC5 | High |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCRUM-52 | AC2 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCRUM-52 | AC5 | Medium |
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCRUM-50 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCRUM-50 | AC5 | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 135 |
| Total Test Logs | 131 |
| Missing Test Cases | 15 |
| Missing Test Logs | 4 |
| Consistency Status | Mismatch Detected |

# Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM9-001 | UT_SCM9_004 | SCM9 | SMS gateway timeout prevents delivery |
| DEF-SCM9-002 | UT_SCM9_012 | SCM9 | Push notification service ignores user preference flag |
| DEF-SCM8-003 | TP_SCM8_009 | SCM8 | Redemption workflow synchronization issue |
| DEF-SCM7-101 | TP_SCM7_005 | SCRUM-58 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-101 | TP_SCM7_015 | SCRUM-58 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCRUM-58 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCRUM-58 | Audit log authorization reference field empty when transfer initiated via bulk admin API |
| DEF-SCM6-101 | TP_SCM6_005 | SCRUM-56 | Adjusted billing amount not included in downgrade confirmation notification to customer |
| DEF-SCM6-102 | TP_SCM6_012 | SCRUM-56 | Audit log not created when downgrade results in zero credit amount |
| DEF-SCM6-103 | TP_SCM6_015 | SCRUM-56 | Enterprise downgrade not held pending state; processed immediately bypassing approval workflow |

# Conclusion

Remediation is required as multiple user stories have partial coverage gaps and 10 defects exist across the test suite.
