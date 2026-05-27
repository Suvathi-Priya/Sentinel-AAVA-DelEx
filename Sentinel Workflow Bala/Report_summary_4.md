# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories.

The 3 user stories form the baseline for evaluation.

The scope is restricted to unit test plans and execution records mapped to these user stories.

Included within scope:

- Unit test cases linked to the identified user stories.
- Test execution results covering executed, not executed, passed, and failed outcomes.
- Defect data directly associated with these user stories.

Excluded from scope:

- Integration tests, system tests, and performance tests.
- User stories not mapped to test cases.
- External or unrelated defect logs.

The user stories are the baseline reference for measuring coverage, execution success, and defect quality.

## Test Coverage Summary

Total Use Cases: 3

Coverage Details:

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 1 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 2 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

Coverage Gap Details:

| User Story ID | AC ID | Acceptance Criteria | Impact Level | Coverage Status |
|---|---|---|---|---|
| BRZ-002 | AC4 | Latency SLA: Given the streaming ingestion, when a message enters Event Hub, then it must be visible in the Bronze layer within 5 minutes. | Medium | Partially Covered |
| SEC-001 | AC5 | Audit Trail: Given an access attempt, when the ADF identity requests a resource, then the action must be logged in the Azure Activity Log with the Identity ID. | Critical | Partially Covered |

| User Story ID | Coverage Score | Color |
|---|---:|---|
| BRZ-002 | 90.00% | 🟢 Green |
| SEC-001 | 90.00% | 🟢 Green |

Legend:

- 🟢 Green (90–100%) → High coverage (meets quality expectations)
- 🟠 Amber (70–89%) → Moderate coverage (requires attention)
- 🔴 Red (<70%) → Low coverage (critical gaps present)

Coverage Score Analysis:

Coverage % = (Covered Acceptance Criteria / Total Acceptance Criteria) × 100

Description:

Coverage Percentage measures the extent to which acceptance criteria are validated by corresponding test cases. It indicates how completely the defined requirements are covered through testing.

Components:

- Covered Acceptance Criteria: Number of acceptance criteria that have at least one mapped test case
- Total Acceptance Criteria: Total number of acceptance criteria defined across user stories

Per User Story Coverage Summary:

| User Story ID | Total Acceptance Criteria | Fully Covered Acceptance Criteria | Partially Covered Acceptance Criteria | Coverage Status | Coverage Percentage |
|---|---:|---:|---:|---|---:|
| STG-001 | 5 | 5 | 0 | Fully Covered | 100.00% |
| BRZ-002 | 5 | 4 | 1 | Partially Covered | 90.00% |
| SEC-001 | 5 | 4 | 1 | Partially Covered | 90.00% |

## Test Execution Summary

Total Test Cases Executed: 45

Total Test Cases Not Executed: 0

Total Test Cases Passed: 39

Total Test Cases Failed: 6

Execution Success Rate: 86.67%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---|---:|---:|---:|---:|---:|---:|---:|
| STG-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-002 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| SEC-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |

Execution Success Rate Formula:

Execution Success Rate = (Test Cases Passed / Test Cases Executed) × 100

## Defect Details

Defect Rate: 13.33%

Defect Rate Analysis:

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:

- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

Defect Details:

| Defect ID | Test Case ID | User Story ID | Defect Title | Defect Description | Category | Severity | Status |
|---|---|---|---|---|---|---|---|
| DEF_STG-001_004 | UT_STG-001_004 | STG-001 | NULL | Validate ingestion behavior when the target domain folder within /bronze does no. Defect raised for investigation and fix. | functional | Medium | open |
| DEF_STG-001_011 | UT_STG-001_011 | STG-001 | NULL | Verify that a user with only /bronze access is denied when attempting to read fr. Defect raised for investigation and fix. | policy_enforcement | High | open |
| DEF_BRZ-002_008 | UT_BRZ-002_008 | BRZ-002 | NULL | Verify that a message entering Event Hub is visible in the Bronze layer within 5. Defect raised for investigation and fix. | functional | Medium | open |
| DEF_BRZ-002_012 | UT_BRZ-002_012 | BRZ-002 | NULL | Validate auto-scaling behavior when throughput spike is brief and the volume ret. Defect raised for investigation and fix. | functional | Medium | open |
| DEF_SEC-001_004 | UT_SEC-001_004 | SEC-001 | NULL | Validate that the ADF identity with only Storage Blob Data Reader role cannot wr. Defect raised for investigation and fix. | policy_enforcement | High | open |
| DEF_SEC-001_011 | UT_SEC-001_011 | SEC-001 | NULL | Validate that a failed access attempt by the ADF identity (e.g., insufficient pe. Defect raised for investigation and fix. | security | Critical | open |

## Conclusion

Summary of Findings:

A total of 3 user stories were reviewed.

Coverage distribution shows 1 fully covered user story, 2 partially covered user stories, and 0 not covered user stories.

The overall unit test coverage rate is 93.30%, the execution success rate is 86.67%, and the defect rate is 13.33%.

Final Outcome Statement:

Based on the overall coverage rate of 93.30%, overall execution success rate of 86.70%, and the presence of Medium, High, and Critical severity defects, the current unit test results indicate that remediation is required before progression.

Conclusion Statement:

The current unit test suite demonstrates high overall coverage, but execution results and open defects include unresolved failures and Critical severity impact. Remediation is required before progression.
