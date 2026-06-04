# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

The baseline for evaluation consists of 2 user stories (PGI-001 and OMS-001) containing a total of 10 acceptance criteria. These user stories form the baseline reference for measuring coverage, execution success, and defect quality.

## Test Coverage Summary

**Total User Stories:** 2

### Coverage Details

| Metric | Count | Description |
|--------|-------|-------------|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 2 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 0 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| PGI-001 | AC1 | No testcase explicitly validates available balance check. | Partially Covered |
| PGI-001 | AC1 | No testcase explicitly validates merchant authorization. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that email confirmation contains amount. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that email confirmation contains date. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that email confirmation contains merchant name. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that email confirmation is sent within 2 minutes of successful payment. | Partially Covered |
| PGI-001 | AC3 | No testcase explicitly validates that payment transactions are logged. | Partially Covered |
| PGI-001 | AC4 | No testcase explicitly validates that retry uses exponential backoff. | Partially Covered |
| PGI-001 | AC5 | No testcase explicitly validates that refund requests are processed within 5 business days. | Partially Covered |
| OMS-001 | AC2 | No testcase explicitly validates that order status is updated to Cancelled lifecycle stage. | Partially Covered |
| OMS-001 | AC4 | No testcase explicitly validates that order events are logged. | Partially Covered |

### Coverage Score

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| PGI-001 | 0.00% | 🔴 Red |
| OMS-001 | 60.00% | 🔴 Red |

Green (90–100%) → High coverage (meets quality expectations)

Amber (70–89%) → Moderate coverage (requires attention)

Red (<70%) → Low coverage (critical gaps present)

Coverage Score (%) = (Fully Covered Acceptance Criteria for the User Story / Total Acceptance Criteria in the User Story) × 100

Coverage Score measures the extent to which the acceptance criteria of an individual user story are validated by corresponding test cases. It indicates how completely the requirements defined within that user story are covered through testing.

Covered Acceptance Criteria for the User Story: Number of acceptance criteria within the user story that have at least one mapped test case.

Total Acceptance Criteria in the User Story: Total number of acceptance criteria defined for that specific user story.

Coverage Score must be calculated separately for each user story using only the acceptance criteria belonging to that user story. Acceptance criteria from other user stories must not be included in the calculation.

## Test Execution Summary

**Total Test Cases Executed:** 30

**Total Test Cases Passed:** 22

**Total Test Cases Failed:** 8

### Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---------------|------------------|----------|--------|--------|
| PGI-001 | 15 | 15 | 11 | 4 |
| OMS-001 | 15 | 15 | 11 | 4 |

## Consistency Analysis

### Consistency Metrics Summary

| Metric | Count |
|--------|-------|
| Total Test Cases | 30 |
| Total Test Logs | 30 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Consistency Status | Consistent |

## Defect Details

**Defect Rate:** 26.67%

Defect Rate = (Total Defects / Total Test Cases) × 100

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Total Defects: Total number of defects identified during the test cycle

Total Test Cases: Total number of test cases executed

| Defect ID | Test Case ID | User Story ID | Defect Description |
|-----------|--------------|---------------|-------------------|
| DEF-PGI-001 | UT_PGI_003 | PGI-001 | Payment processing response exceeds 10 second SLA under concurrent load |
| DEF-PGI-002 | UT_PGI_005 | PGI-001 | Email confirmation template missing merchant name field |
| DEF-PGI-003 | UT_PGI_012 | PGI-001 | Alert notification service failed to dispatch operations team alert on final retry exhaustion |
| DEF-PGI-004 | UT_PGI_015 | PGI-001 | Refund status notification service did not trigger customer email on status change |
| DEF-OMS-001 | UT_OMS_003 | OMS-001 | Order confirmation service response exceeds 30 second SLA during concurrent order submissions |
| DEF-OMS-002 | UT_OMS_006 | OMS-001 | Notification event not fired for Dispatched status transition in order lifecycle service |
| DEF-OMS-003 | UT_OMS_014 | OMS-001 | Agent routing service failed to assign late cancellation request to customer service queue |

## Conclusion

Remediation is required as test case failures and defects exist in the unit test suite. The report indicates outstanding coverage and execution issues that must be addressed before progression.
