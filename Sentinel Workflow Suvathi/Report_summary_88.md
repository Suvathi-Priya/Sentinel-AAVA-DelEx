# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories. The baseline for evaluation consists of SCM-002 (Subscription Pause Management Service), SCM-003 (Subscription Upgrade Request Processing), and SCM-007 (Subscription Transfer and Ownership Change) user stories.

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| SCM-002 | AC2 | No testcase explicitly validates that resume date is included in the pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that customers can view scheduled resume date in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that pause start date is captured in the pause audit logs. | Partially Covered |
| SCM-003 | AC3 | No testcase explicitly validates that customers can view next billing cycle changes in the customer portal. | Partially Covered |
| SCM-007 | AC2 | No testcase explicitly validates that transfer details are included in the transfer notification. | Partially Covered |
| SCM-007 | AC3 | No testcase explicitly validates that outgoing owner can view billing change summary in the customer portal.; No testcase explicitly validates that incoming owner can view billing change summary in the customer portal. | Partially Covered |
| SCM-007 | AC4 | No testcase explicitly validates that subscription ID is captured in the transfer audit logs.; No testcase explicitly validates that transfer date is captured in the transfer audit logs.; No testcase explicitly validates that timestamp is captured in the transfer audit logs. | Partially Covered |
| SCM-007 | AC5 | No testcase explicitly validates that subscription transfers involving a change in billing entity require compliance team approval before the transfer is completed. | Partially Covered |

## Consistency Analysis

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|--------------|------------------|-------------|---------------|-------|--------------|
| TP_SCM_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_001 | SCM-002 | AC1 | Medium |
| TP_SCM_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_002 | SCM-002 | AC1 | Medium |
| TP_SCM_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_003 | SCM-002 | AC1 | Medium |
| TP_SCM_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_004 | SCM-002 | AC2 | Medium |
| TP_SCM_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_005 | SCM-002 | AC2 | Medium |
| TP_SCM_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_006 | SCM-002 | AC3 | Medium |
| TP_SCM_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_007 | SCM-002 | AC3 | Medium |
| TP_SCM_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_008 | SCM-002 | AC4 | Medium |
| TP_SCM_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_009 | SCM-002 | AC5 | Medium |
| TP_SCM_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_010 | SCM-002 | AC1 | Medium |
| TP_SCM_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_011 | SCM-002 | AC2 | Medium |
| TP_SCM_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_012 | SCM-002 | AC4 | Medium |
| TP_SCM_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_013 | SCM-002 | AC5 | Medium |
| TP_SCM_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_014 | SCM-002 | AC1 | Medium |
| TP_SCM_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM_015 | SCM-002 | AC5 | Medium |
| TP_SCM2_001 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_001 | SCM-002 | AC1 | High |
| TP_SCM2_002 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_002 | SCM-002 | AC1 | High |
| TP_SCM2_003 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_003 | SCM-002 | AC1 | High |
| TP_SCM2_004 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_004 | SCM-002 | AC2 | High |
| TP_SCM2_005 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_005 | SCM-002 | AC2 | High |
| TP_SCM2_006 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_006 | SCM-002 | AC3 | High |
| TP_SCM2_007 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_007 | SCM-002 | AC3 | High |
| TP_SCM2_008 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_008 | SCM-002 | AC4 | High |
| TP_SCM2_009 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_009 | SCM-002 | AC5 | High |
| TP_SCM2_010 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_010 | SCM-002 | AC1 | High |
| TP_SCM2_011 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_011 | SCM-002 | AC2 | High |
| TP_SCM2_012 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_012 | SCM-002 | AC4 | High |
| TP_SCM2_013 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_013 | SCM-002 | AC5 | High |
| TP_SCM2_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_014 | SCM-002 | AC1 | High |
| TP_SCM2_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: TP_SCM2_015 | SCM-002 | AC5 | High |
| TP_SCM3_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_014 | SCM-003 | AC1 | Medium |
| TP_SCM3_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM3_015 | SCM-003 | AC5 | Medium |

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 45 |
| Total Test Logs | 43 |
| Missing Test Cases | 15 |
| Missing Test Logs | 17 |
| Consistency Status | Mismatch Detected |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-SCM2-101 | TP_SCM2_008 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM2-102 | TP_SCM2_009 | SCM-002 | Activation allowed without completed approval |
| DEF-SCM3-101 | TP_SCM3_004 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_009 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-SCM7-101 | TP_SCM7_005 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |
| DEF-SCM7-102 | TP_SCM7_012 | SCM-007 | Compliance approval workflow not initiated for transfers involving tax jurisdiction change only without entity change |
| DEF-SCM7-103 | TP_SCM7_014 | SCM-007 | Audit log authorization reference field empty when transfer initiated via bulk admin API |
| DEF-SCM7-101 | TP_SCM7_015 | SCM-007 | New owner transfer notification not triggered when transfer is initiated via bulk admin API endpoint |

## Conclusion

Remediation is required as multiple user stories have coverage gaps and defects exist across all three user stories.
