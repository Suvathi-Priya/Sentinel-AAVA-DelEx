# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories.

These user stories form the baseline for evaluation. The scope is restricted to unit test plans and execution records mapped to these user stories.

Included in scope:

- Unit test cases linked to the identified user stories.
- Test execution results covering executed, not executed, passed, and failed outcomes.
- Defect data directly associated with these user stories.

Excluded from scope:

- Integration tests, system tests, and performance tests.
- User stories not mapped to test cases.
- External or unrelated defect logs.

The baseline reference for measuring coverage, execution success, and defect quality is limited to the following user stories: STG-001, BRZ-002, and SEC-001.

Data integrity validation status: Matched.

| Metric | Count | Description |
|---|---:|---|
| Total Test Cases | 42 | Total unit test cases identified in the input |
| Total Test Logs | 42 | Total unit test execution records identified in the input |
| Missing Test Logs | 0 | Test cases without corresponding execution records |
| Missing Test Cases | 0 | Execution records without corresponding test cases |
| Extra Test Cases | 0 | Additional test cases not aligned to the validated baseline |
| Extra Test Logs | 0 | Additional execution records not aligned to the validated baseline |

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
| STG-001 | AC1 | Zone Creation: Given a new Data Lake account, when initialized, then separate root containers for /bronze, /silver, and /gold must be created. | Medium | Partially Covered |
| STG-001 | AC2 | Domain Organization: Given the /bronze container, when data is ingested, then it must be organized by domain folders (e.g., /sales, /finance). | Medium | Partially Covered |
| STG-001 | AC4 | Encryption Validation: Given data landing in any zone, when stored at rest, then it must be encrypted using Microsoft-managed and Customer-managed keys. | High | Partially Covered |
| SEC-001 | AC1 | Identity Creation: Given a new ADF instance, when deployed, then a System-Assigned Managed Identity must be enabled. | High | Not Covered |

| User Story ID | Coverage Score | Color |
|---|---:|---|
| STG-001 | 70.00% | 🟠 Amber |
| SEC-001 | 80.00% | 🟠 Amber |
| BRZ-002 | 100.0% | 🟢 Green |

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

## Test Execution Summary

Total Test Cases Executed: 42

Total Test Cases Not Executed: 0

Total Test Cases Passed: 36

Total Test Cases Failed: 6

Execution Success Rate: 85.7%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---|---:|---:|---:|---:|---:|---:|---:|
| STG-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-002 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| SEC-001 | 12 | 12 | 0 | 10 | 2 | 100.00% | 83.33% |

Execution success rate is 85.7%, based on 36 passed test cases out of 42 executed test cases.

Failures are distributed across all 3 user stories. STG-001 recorded 2 failed test cases, BRZ-002 recorded 2 failed test cases, and SEC-001 recorded 2 failed test cases.

All identified test cases were executed. No not-executed test cases were reported in the input.

## Defect Details

Defect Rate: 14.29%

Defect Rate Analysis:

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:

- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

| Defect ID | Test Case ID | User Story ID | Defect Description | Category | Severity | Status |
|---|---|---|---|---|---|---|
| DEF_STG-001_004 | UT_STG-001_004 | STG-001 | Validate ingestion behavior when the target domain folder within /bronze does no. Defect raised for investigation and fix. | Functional | High | open |
| DEF_STG-001_011 | UT_STG-001_011 | STG-001 | Verify that a user with only /bronze access is denied when attempting to read fr. Defect raised for investigation and fix. | Security | Critical | open |
| DEF_BRZ-002_008 | UT_BRZ-002_008 | BRZ-002 | Verify that a message entering Event Hub is visible in the Bronze layer within 5. Defect raised for investigation and fix. | SLA | High | open |
| DEF_BRZ-002_012 | UT_BRZ-002_012 | BRZ-002 | Validate auto-scaling behavior when throughput spike is brief and the volume ret. Defect raised for investigation and fix. | Scalability | Medium | open |
| DEF_SEC-001_004 | UT_SEC-001_002 | SEC-001 | Validate that the ADF identity with only Storage Blob Data Reader role cannot wr. Defect raised for investigation and fix. | Security | Critical | open |
| DEF_SEC-001_011 | UT_SEC-001_009 | SEC-001 | Validate that a failed access attempt by the ADF identity (e.g., insufficient pe. Defect raised for investigation and fix. | Audit | High | open |

## Conclusion

Summary of Findings:

A total of 3 user stories were reviewed. Coverage distribution shows 1 fully covered user story, 2 partially covered user stories, and 0 not covered user stories. Execution success rate is 85.7%, and defect rate is 14.29%.

Final Outcome Statement:

The overall test coverage rate is 83.3%, and the overall execution success rate is 85.7%. The defect profile includes 2 Critical defects, 3 High defects, and 1 Medium defect. Based on these reported values, the current unit test baseline shows Moderate coverage with open high-severity and critical-severity defects.

Conclusion Statement:

The current unit test suite is not sufficient to proceed without remediation. Coverage gaps and open critical and high-severity defects require resolution before progression.
