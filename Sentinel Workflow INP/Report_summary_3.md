<div align="center"><strong><span style="font-size:28px;">UNIT TEST QUALITY & COVERAGE REPORT</span></strong></div>

# Scope

This report evaluates unit test coverage and quality across 5 user stories.

The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

# Test Coverage Summary

**Total User Stories:** 5

## Coverage Details

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 5 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

## Coverage Gap Details

| User Story ID | AC ID | Acceptance Criteria | Coverage Status |
|---|---|---|---|
| SCM-002 | AC2 | No testcase explicitly validates that resume date is included in the pause confirmation notification. | Partially Covered |
| SCM-002 | AC3 | No testcase explicitly validates that customers can view the scheduled resume date in the customer portal. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that pause start date is captured in pause audit logs. | Partially Covered |
| SCM-002 | AC4 | No testcase explicitly validates that timestamp is captured in pause audit logs. | Partially Covered |
| SCM-002 | AC5 | No testcase explicitly validates that manager approval is required before the pause is activated. | Partially Covered |
| ORM-001 | AC4 | No testcase explicitly validates that approval timestamp is captured in refund audit logs. | Partially Covered |
| ORM-001 | AC5 | No testcase explicitly validates the threshold of $1000 for high-value refunds. | Partially Covered |
| CLP-001 | AC5 | No testcase explicitly validates that fraud review is required for reward redemptions above 5000 points. | Partially Covered |
| SCM-003 | AC2 | No testcase explicitly validates that revised billing amount is included in the upgrade confirmation notification. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that subscription ID is captured in upgrade audit logs. | Partially Covered |
| SCM-003 | AC4 | No testcase explicitly validates that upgrade date is captured in upgrade audit logs. | Partially Covered |
| SCM-003 | AC5 | No testcase explicitly validates that manager approval is required before the upgrade is activated. | Partially Covered |
| CNS-001 | AC4 | No testcase explicitly validates that timestamp is captured in notification logs. | Partially Covered |
| CNS-001 | AC5 | No testcase explicitly validates that retry attempts are limited to 3 times. | Partially Covered |

## Coverage Score

| User Story ID | Coverage Score | Color |
|---|---|---|
| SCM-002 | 20.00% | 🔴 Red |
| ORM-001 | 60.00% | 🟠 Amber |
| CLP-001 | 80.00% | 🟠 Amber |
| SCM-003 | 40.00% | 🔴 Red |
| CNS-001 | 40.00% | 🔴 Red |

## Legend

| Color | Coverage Range | Interpretation |
|---|---|---|
| 🔴 Red | <70% | Low coverage (critical gaps present) |
| 🟠 Amber | 70–89% | Moderate coverage (requires attention) |
| Green | 90–100% | High coverage (meets quality expectations) |

## Formula Analysis for Coverage Score

#### Formula

```text
(fully_covered_acceptance_criterias / total_acceptance_criterias) × 100
```

#### Description

Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

#### Components

| Component | Description |
|---|---|
| fully_covered_acceptance_criterias | Number of acceptance criteria within the user story that are Fully Covered |
| total_acceptance_criterias | Total number of acceptance criteria defined for that specific user story |

#### Calculation Scope:

Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

# Test Execution Summary

### Overall Test Execution Summary

**Total Test Cases Executed:** 73

**Total Test Cases Passed:** 57

**Total Test Cases Failed:** 16

## Test Execution Summary Details

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| SCM-002 | 15 | 15 | 13 | 2 |
| ORM-001 | 15 | 15 | 12 | 3 |
| CLP-001 | 13 | 15 | 12 | 3 |
| CNS-001 | 15 | 13 | 10 | 3 |
| SCM-003 | 15 | 15 | 13 | 2 |

# Consistency Analysis

Mismatch Detected

## Data Mapping Inconsistency Details

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---|---|---|---|---|---|
| UT_CLP_014 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_014 | CLP-001 |  | High |
| UT_CLP_015 | missing_testcase | Mapped testcase definition is missing for testcase ID: UT_CLP_015 | CLP-001 |  | High |
| UT_CNS_014 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_014 | CNS-001 |  | Medium |
| UT_CNS_015 | missing_testlog | Execution log is missing for testcase ID: UT_CNS_015 | CNS-001 |  | Medium |

## Consistency Metrics Summary

| Metric | Count |
|---|---|
| total_testcases | 73 |
| total_testlogs | 73 |
| consistency_status | Mismatch Detected |
| missing_testlogs | 2 |
| missing_testcases | 2 |

# Defect Details

**Defect Rate:** 21.92%

## Formula Analysis for Defect Rate

#### Formula

```text
(total_defects_in_all_test_logs / total_test_cases_in_all_test_plan) × 100
```

#### Description

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

#### Components

| Component | Description |
|---|---|
| total_defects_in_all_test_logs | Total number of defects identified during the test cycle |
| total_test_cases_in_all_test_plan | Total number of test cases executed |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-SCM-101 | TP_SCM_012 | SCM-002 | Pause reason not captured consistently |
| DEF-SCM-102 | TP_SCM_015 | SCM-002 | Activation allowed without completed approval |
| DEF-ORM-001 | UT_ORM_005 | ORM-001 | Notification template rendering issue |
| DEF-ORM-002 | UT_ORM_009 | ORM-001 | Status history service timeout |
| DEF-ORM-003 | UT_ORM_015 | ORM-001 | Refund workflow synchronization error |
| DEF-CLP-001 | UT_CLP_003 | CLP-001 | Points posting service delay |
| DEF-CLP-002 | UT_CLP_008 | CLP-001 | Balance refresh cache issue |
| DEF-CLP-003 | UT_CLP_015 | CLP-001 | Redemption workflow synchronization issue |
| DEF-SCM3-101 | TP_SCM3_005 | SCM-003 | Revised billing amount not included in upgrade confirmation notification |
| DEF-SCM3-102 | TP_SCM3_014 | SCM-003 | Manager approval workflow not initiated when price increase equals exactly 50% |
| DEF-CNS-001 | UT_CNS_004 | CNS-001 | SMS gateway timeout prevents delivery |
| DEF-CNS-002 | UT_CNS_006 | CNS-001 | SMS tracking service failed to update status |
| DEF-CNS-003 | UT_CNS_009 | CNS-001 | Push notification service unavailable |

# Conclusion

The report indicates outstanding coverage and execution issues based on the provided data. With 16 test case failures and 16 defects identified across all user stories, remediation is required before progression.
