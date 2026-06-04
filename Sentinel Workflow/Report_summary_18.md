# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 2

The 2 user stories form the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

**Inclusions:**
- Unit test cases linked to the identified user stories
- Test execution results (executed, passed, failed)
- Defect data directly associated with these user stories

**Exclusions:**
- Integration tests, system tests, or performance tests
- User stories not mapped to test cases

## Test Coverage Summary

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| PGI-001 | AC1 | No testcase explicitly validates available balance check. | Partially Covered |
| PGI-001 | AC1 | No testcase explicitly validates merchant authorization. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that amount is present in email confirmation. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that date is present in email confirmation. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates that merchant name is present in email confirmation. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates the 2 minute time threshold for email delivery. | Partially Covered |
| PGI-001 | AC3 | No testcase explicitly validates that payment transactions are logged. | Partially Covered |
| PGI-001 | AC4 | No testcase explicitly validates exponential backoff retry strategy. | Partially Covered |
| PGI-001 | AC5 | No testcase explicitly validates the 5 business day processing time threshold. | Partially Covered |
| OMS-001 | AC2 | No testcase explicitly validates order status transition to Cancelled. | Partially Covered |
| OMS-001 | AC4 | No testcase explicitly validates that order events are logged. | Partially Covered |

### Coverage Score

| User Story ID | Coverage Score | Color Indicator |
|---|---:|---|
| PGI-001 | 0.00% | 🔴 Red |
| OMS-001 | 60.00% | 🔴 Red |

## Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| PGI-001 | 15 | 15 | 11 | 4 |
| OMS-001 | 15 | 15 | 11 | 4 |

## Consistency Analysis

### Data Mapping Inconsistency Details

No inconsistency details provided.

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 30 |
| Total Test Logs | 30 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Consistency Status | Consistent |

## Defect Details

| Defect ID | Test Case ID | User Story ID | Defect Description |
|---|---|---|---|
| DEF-PGI-001 | UT_PGI_003 | PGI-001 | Payment processing response exceeds 10 second SLA under concurrent load |
| DEF-PGI-002 | UT_PGI_005 | PGI-001 | Email confirmation template missing merchant name field |
| DEF-PGI-003 | UT_PGI_012 | PGI-001 | Alert notification service failed to dispatch operations team alert on final retry exhaustion |
| DEF-PGI-004 | UT_PGI_015 | PGI-001 | Refund status notification service did not trigger customer email on status change |
| DEF-OMS-001 | UT_OMS_003 | OMS-001 | Order confirmation service response exceeds 30 second SLA during concurrent order submissions |
| DEF-OMS-002 | UT_OMS_006 | OMS-001 | Notification event not fired for Dispatched status transition in order lifecycle service |
| DEF-OMS-003 | UT_OMS_014 | OMS-001 | Agent routing service failed to assign late cancellation request to customer service queue |

## Conclusion

Remediation is required as test case failures and defects exist in the unit test suite. The report indicates outstanding coverage and execution issues that must be addressed before progression.
