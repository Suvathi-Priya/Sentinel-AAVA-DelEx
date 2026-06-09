# UNIT TEST QUALITY & COVERAGE REPORT

## Scope
This report presents the unit test quality and coverage assessment for the provided user stories, test plan mappings, test execution logs, mapping consistency details, consistency summary, test execution summary, coverage analysis, and summary metrics.

The report content is generated directly from the provided input data and includes only the sections and values available in the input.

## Test Coverage Summary

| Metric | Count | Description |
|---|---:|---|
| total_user_stories | 5 | total_user_stories |
| total_Fully_covered_user_stories | 1 | total_Fully_covered_user_stories |
| total_Partially_covered_user_stories | 4 | total_Partially_covered_user_stories |
| total_Not_covered_user_stories | 0 | total_Not_covered_user_stories |
| total_acceptance_criterias_in_all_user_stories | 25 | total_acceptance_criterias_in_all_user_stories |
| fully_covered_acceptance_criterias_in_all_user_stories | 15 | fully_covered_acceptance_criterias_in_all_user_stories |
| partially_covered_acceptance_criterias_in_all_user_stories | 10 | partially_covered_acceptance_criterias_in_all_user_stories |
| not_covered_acceptance_criterias_in_all_user_stories | 0 | not_covered_acceptance_criterias_in_all_user_stories |
| overall_coverage_score_percentage | 60.0 | overall_coverage_score_percentage |

### Coverage Details

| Metric | Count | Description |
|---|---:|---|
| ORM-001 | 60.0 | Implement Order Refund Management Service |
| CNS-001 | 60.0 | Implement Customer Notification Service |
| CLP-001 | 80.0 | Implement Customer Loyalty Points Service |
| SCM-003 | 60.0 | Subscription Upgrade Request Processing |
| SCM-004 | 40.0 | Subscription Cancellation Workflow |

### Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---|---|---|---|
| ORM-001 | AC4 | Refund audit logs must capture customer ID, refund amount, and approval timestamp. | Partially Covered |
| ORM-001 | AC5 | High-value refunds above $1000 must require manager approval and fraud review. | Partially Covered |
| CNS-001 | AC4 | Notification logs must capture customer ID, notification type, and timestamp. | Partially Covered |
| CNS-001 | AC5 | Failed notifications must trigger retry attempts up to 3 times. | Partially Covered |
| CLP-001 | AC5 | Reward redemptions above 5000 points must require manager approval and fraud review. | Partially Covered |
| SCM-003 | AC2 | Upgrade confirmation notifications must be sent to customers including the new plan details, effective date, and revised billing amount. | Partially Covered |
| SCM-003 | AC4 | Upgrade audit logs must capture customer ID, subscription ID, previous plan, new plan, upgrade date, and timestamp. | Partially Covered |
| SCM-004 | AC2 | Cancellation confirmation notifications must be sent to customers including the effective cancellation date and any applicable refund details. | Partially Covered |
| SCM-004 | AC4 | Cancellation audit logs must capture customer ID, subscription ID, cancellation reason, effective date, refund amount, and timestamp. | Partially Covered |

### Coverage Score

| User Story ID | Coverage Score | Color |
|---|---:|---|
| ORM-001 | 60.0 | 🟠 Amber |
| CNS-001 | 60.0 | 🟠 Amber |
| CLP-001 | 80.0 | 🟢 Green |
| SCM-003 | 60.0 | 🟠 Amber |
| SCM-004 | 40.0 | 🔴 Red |

### Legend

| Color | Coverage Range | Interpretation |
|---|---|---|
| 🟢 Green | 80–100 | Fully Covered |
| 🟠 Amber | 50–79 | Partially Covered |
| 🔴 Red | 0–49 | Low Coverage |

### Formula Analysis for Coverage Score

#### Formula

```text
(fully_covered_acceptance_criterias / total_acceptance_criterias) × 100
```

#### Description
coverage_score_formula

#### Components

| Component | Description |
|---|---|
| fully_covered_acceptance_criterias | fully_covered_acceptance_criterias |
| total_acceptance_criterias | total_acceptance_criterias |

#### Calculation Scope:
Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story.

## Test Execution Summary

Test execution summary is based on the provided test_execution_summary data.

### Overall Test Execution Summary

total_test_cases_in_all_test_plan: 73

total_test_cases_in_all_test_logs: 15

total_passed_in_all_test_logs: 13

total_failed_in_all_test_logs: 2

total_defects_in_all_test_logs: 2

### Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| ORM-001 | 15 | 0 | 0 | 0 |
| CNS-001 | 15 | 0 | 0 | 0 |
| CLP-001 | 13 | 0 | 0 | 0 |
| SCM-003 | 15 | 15 | 13 | 2 |
| SCM-004 | 15 | 0 | 0 | 0 |

## Consistency Analysis

Consistency analysis is based on the provided mapping_consistency_details and consistency_summary.

### Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_CNS_001 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_001 | CNS-001 | AC1 | Medium |
| UT_CNS_002 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_002 | CNS-001 | AC1 | Medium |
| UT_CNS_003 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_003 | CNS-001 | AC1 | Medium |
| UT_CNS_004 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_004 | CNS-001 | AC2 | Medium |
| UT_CNS_005 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_005 | CNS-001 | AC2 | Medium |
| UT_CNS_006 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_006 | CNS-001 | AC2 | Medium |
| UT_CNS_007 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_007 | CNS-001 | AC3 | Medium |
| UT_CNS_008 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_008 | CNS-001 | AC3 | Medium |
| UT_CNS_009 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_009 | CNS-001 | AC3 | Medium |
| UT_CNS_010 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_010 | CNS-001 | AC4 | Medium |
| UT_CNS_011 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_011 | CNS-001 | AC4 | Medium |
| UT_CNS_012 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_012 | CNS-001 | AC4 | Medium |
| UT_CNS_013 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_013 | CNS-001 | AC5 | Medium |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 | AC5 | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 | AC5 | Medium |
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
| UT_CLP_001 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_001 | CLP-001 | AC1 | Medium |
| UT_CLP_002 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_002 | CLP-001 | AC1 | Medium |
| UT_CLP_003 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_003 | CLP-001 | AC1 | Medium |
| UT_CLP_004 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_004 | CLP-001 | AC2 | Medium |
| UT_CLP_005 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_005 | CLP-001 | AC2 | Medium |
| UT_CLP_006 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_006 | CLP-001 | AC2 | Medium |
| UT_CLP_007 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_007 | CLP-001 | AC3 | Medium |
| UT_CLP_008 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_008 | CLP-001 | AC3 | Medium |
| UT_CLP_009 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_009 | CLP-001 | AC3 | Medium |
| UT_CLP_010 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_010 | CLP-001 | AC4 | Medium |
| UT_CLP_011 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_011 | CLP-001 | AC4 | Medium |
| UT_CLP_012 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_012 | CLP-001 | AC4 | Medium |
| UT_CLP_013 | missing_testlog | Execution log is missing for testcase ID: UT_CLP_013 | CLP-001 | AC5 | Medium |
| TP_SCM4_001 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_001 | SCM-004 | AC1 | Medium |
| TP_SCM4_002 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_002 | SCM-004 | AC1 | Medium |
| TP_SCM4_003 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_003 | SCM-004 | AC1 | Medium |
| TP_SCM4_004 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_004 | SCM-004 | AC2 | Medium |
| TP_SCM4_005 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_005 | SCM-004 | AC2 | Medium |
| TP_SCM4_006 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_006 | SCM-004 | AC2 | Medium |
| TP_SCM4_007 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_007 | SCM-004 | AC3 | Medium |
| TP_SCM4_008 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_008 | SCM-004 | AC3 | Medium |
| TP_SCM4_009 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_009 | SCM-004 | AC3 | Medium |
| TP_SCM4_010 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_010 | SCM-004 | AC4 | Medium |
| TP_SCM4_011 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_011 | SCM-004 | AC4 | Medium |
| TP_SCM4_012 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_012 | SCM-004 | AC4 | Medium |
| TP_SCM4_013 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_013 | SCM-004 | AC5 | Medium |
| TP_SCM4_014 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_014 | SCM-004 | AC5 | Medium |
| TP_SCM4_015 | missing_testlog | Execution log is missing for testcase ID: TP_SCM4_015 | SCM-004 | AC5 | Medium |

### Consistency Metrics Summary

| Metric | Count |
|---|---:|
| total_testcases | 73 |
| total_testlogs | 15 |
| consistency_status | Mismatch Detected |
| missing_testlogs | 58 |
| missing_testcases | 0 |

## Defect Details

Defect details are based on the provided test execution and coverage analysis input.

### Defect Rate

overall_defect_rate_percentage: 2.74

overall_defect_rate_formula: (total_defects_in_all_test_logs / total_test_cases_in_all_test_plan) × 100

overall_defect_rate_calculation: (2 / 73) × 100 = 2.74

### Formula Analysis for Defect Rate

#### Formula

```text
(total_defects_in_all_test_logs / total_test_cases_in_all_test_plan) × 100
```

#### Description
overall_defect_rate_formula

#### Components

| Component | Description |
|---|---|
| total_defects_in_all_test_logs | total_defects_in_all_test_logs |
| total_test_cases_in_all_test_plan | total_test_cases_in_all_test_plan |

### Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |

## Conclusion
Mismatch Detected