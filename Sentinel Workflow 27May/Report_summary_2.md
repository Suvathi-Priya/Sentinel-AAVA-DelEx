# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories.

These user stories form the baseline reference for evaluating unit test coverage, test execution results, and defect quality.

The scope is restricted to unit test cases, execution records, and defect data mapped directly to the identified user stories.

Included in scope:

- Unit test cases linked to the identified user stories.
- Test execution results covering executed, passed, and failed outcomes.
- Defect records directly associated with these user stories.

Excluded from scope:

- Integration tests, system tests, and performance tests.
- User stories not mapped to test cases.
- External or unrelated defect logs.

## Test Coverage Summary

Total Use Cases: 3

Coverage Details:

| Metric | Count | Description |
|--------------------|-------|-----------------------------------------------------------------------------|
| Fully Covered | 1 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 2 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

Coverage Gap Details:

| User Story ID | AC ID | Acceptance Criteria | Impact Level | Coverage Status |
|---|---|---|---|---|
| BRZ-001 | AC2 | Raw Format Preservation: Given the ingestion process, when data is landed in ADLS Gen2, then it must be stored in its source format (e.g., Parquet or Avro). | Medium | Partially Covered |
| BRZ-001 | AC3 | Metadata Capture: Given a successful ingestion, when the record is saved, then metadata (source system, load timestamp, file name) must be appended. | Medium | Partially Covered |
| BRZ-001 | AC4 | Retry Logic: Given a transient network failure, when the ingestion fails, then the system must automatically retry 3 times before triggering an alert. | High | Partially Covered |
| SEC-001 | AC1 | Identity Creation: Given a new ADF instance, when deployed, then a System-Assigned Managed Identity must be enabled. | Critical | Not Covered |

| User Story ID | Coverage Score | Color |
|---|---:|---|
| BRZ-001 | 70.00% | 🟠 Amber |
| BRZ-002 | 100.00% | 🟢 Green |
| SEC-001 | 80.00% | 🟠 Amber |

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

Total Test Cases Passed: 36

Total Test Cases Failed: 6

Execution Success Rate = (Test Cases Passed / Test Cases Executed) × 100 = 85.71%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Total Executed | Passed | Failed |
|---|---:|---:|---:|---:|
| BRZ-001 | 15 | 15 | 13 | 2 |
| BRZ-002 | 15 | 15 | 13 | 2 |
| SEC-001 | 12 | 12 | 10 | 2 |

Data Mapping Inconsistency Details:

| Test Case ID | Consistency Type | Description | User Story ID | AC ID | Impact Level |
|---------------|------------------|-------------|----------------|-------|---------------|
| NULL | NULL | NULL | NULL | NULL | NULL |

Consistency Metrics Summary:

| Metric | Count |
|---------|-------|
| Total Test Cases | 42 |
| Total Test Logs | 42 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Extra Test Cases | 0 |
| Extra Test Logs | 0 |
| Consistency Status | Matched |

## Defect Details

Defect Rate: 14.29%

Defect Rate Analysis:

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:

- Total Defects: Total number of defects identified during the test cycle
- Total Test Cases: Total number of test cases executed

Defect Details:

| Defect ID | Test Case ID | User Story ID | Defect Title | Defect Description | Severity | Status |
|---|---|---|---|---|---|---|
| DEF_BRZ-001_002 | UT_BRZ-001_002 | BRZ-001 | NULL | Validate pipeline behavior when the Self-Hosted Integration Runtime is offline during a scheduled ingestion run. Defect raised for investigation and fix. | High | open |
| DEF_BRZ-001_009 | UT_BRZ-001_009 | BRZ-001 | NULL | Validate retry logic when network failure persists beyond 3 attempts. Defect raised for investigation and fix. | High | open |
| DEF_BRZ-002_008 | UT_BRZ-002_008 | BRZ-002 | NULL | Verify that a message entering Event Hub is visible in the Bronze layer within 5 minutes. Defect raised for investigation and fix. | High | open |
| DEF_BRZ-002_012 | UT_BRZ-002_012 | BRZ-002 | NULL | Validate auto-scaling behavior when throughput spike is brief and the volume returns to normal within minutes. Defect raised for investigation and fix. | Critical | open |
| DEF_SEC-001_004 | UT_SEC-001_002 | SEC-001 | NULL | Validate that the ADF identity with only Storage Blob Data Reader role cannot write data to ADLS Gen2. Defect raised for investigation and fix. | Critical | open |
| DEF_SEC-001_011 | UT_SEC-001_009 | SEC-001 | NULL | Validate that a failed access attempt by the ADF identity (e.g., insufficient permissions) is also logged in the Activity Log. Defect raised for investigation and fix. | Critical | open |

Defect pattern summary:

- High severity defects: 3
- Critical severity defects: 3
- Open defects: 6

## Conclusion

Summary of Findings:

A total of 3 user stories were reviewed. Coverage distribution shows 1 fully covered user story, 2 partially covered user stories, and 0 not covered user stories. The overall test coverage rate is 83.30%, the execution success rate is 85.71%, and the defect rate is 14.29%.

Final Outcome Statement:

Based on the overall coverage rate of 83.30%, execution success rate of 85.71%, and the presence of Critical and High severity defects, the current unit test results indicate incomplete coverage and unresolved quality risk within the evaluated baseline.

Conclusion Statement:

The current unit test suite is not sufficient to proceed without remediation. Coverage gaps and open defects require resolution before progression.
