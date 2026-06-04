# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Coverage Boundary:** The total number of user stories included in the analysis is 2, forming the baseline for evaluation. The scope is limited to unit test coverage and execution records mapped to these user stories.

**Inclusions:**

- Unit test cases linked to the identified user stories
- Test execution results (executed, not executed, passed, failed)
- Defect data directly associated with these user stories

**Exclusions:**

- Integration tests, system tests, or performance tests
- User stories not mapped to test cases

**Baseline Definition:** The user stories serve as the baseline reference for measuring coverage, execution success, and defect quality.

## Test Coverage Summary

**Total User Stories:** 2

### Coverage Details

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 0 | User stories where all acceptance criteria are Fully Covered |
| Partially Covered | 1 | User stories containing one or more Partially Covered acceptance criteria |
| Not Covered | 1 | User stories where all acceptance criteria are Not Covered |

### Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---|---|---|---|
| PGI-001 | AC1 | No testcase explicitly validates available balance check. | Partially Covered |
| PGI-001 | AC1 | No testcase explicitly validates merchant authorization. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates amount in email confirmation. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates date in email confirmation. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates merchant name in email confirmation. | Partially Covered |
| PGI-001 | AC2 | No testcase explicitly validates 2 minute delivery time threshold. | Partially Covered |
| PGI-001 | AC3 | No testcase explicitly validates that payment transactions are logged. | Partially Covered |
| PGI-001 | AC4 | No testcase explicitly validates exponential backoff retry strategy. | Partially Covered |
| PGI-001 | AC5 | No testcase explicitly validates 5 business day processing time threshold. | Partially Covered |
| OMS-001 | AC1 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC1 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC1 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC1 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC1 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC1 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC2 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC2 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC2 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC2 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC2 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC2 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC3 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC3 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC4 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC5 | No testcase mapped to this acceptance criterion. | Not Covered |
| OMS-001 | AC5 | No testcase mapped to this acceptance criterion. | Not Covered |

### Coverage Score

| User Story ID | Coverage Score | Color |
|---|---:|---|
| PGI-001 | 0.00% | 🔴 Red |
| OMS-001 | 0.00% | 🔴 Red |

## Test Execution Summary

### Test Execution Summary

| User Story ID | Total Test Cases | Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| PGI-001 | 15 | 15 | 11 | 4 |
| OMS-001 | 0 | 0 | 0 | 0 |

## Consistency Analysis

### Data Mapping Inconsistency Details

No data.

### Consistency Metrics Summary

| Metric | Count |
|---|---|
| Total Test Cases | 15 |
| Total Test Logs | 15 |
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

## Conclusion

Remediation is required as user story OMS-001 is Not Covered and defects exist in the test execution results.
