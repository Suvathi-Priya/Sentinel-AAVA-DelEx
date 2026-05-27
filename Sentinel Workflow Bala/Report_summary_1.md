# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories.

These 3 user stories form the baseline for evaluation.

The scope is restricted to unit test cases, unit test execution records, and defect data mapped directly to these user stories.

Included in scope:

- Unit test cases linked to the identified user stories.
- Test execution results covering executed, not executed, passed, and failed outcomes.
- Defect data directly associated with these user stories.

Excluded from scope:

- Integration tests, system tests, and performance tests.
- User stories not mapped to test cases.
- External or unrelated defect logs.

The baseline reference for measuring coverage, execution success, and defect quality is limited to the mapped user stories: LZ-001, BRZ-001, and STG-001.

Data integrity validation result: Matched.

| Validation Metric | Count | Description |
|-------------------|-------|-------------|
| Total Test Cases | 45 | Total test cases present in mapped test plan data |
| Total Test Logs | 45 | Total execution records present in mapped test execution data |
| Missing Test Logs | 0 | Test cases without corresponding execution records |
| Missing Test Cases | 0 | Execution records without corresponding mapped test cases |
| Extra Test Cases | 0 | Additional unmapped test cases identified in source data |
| Extra Test Logs | 0 | Additional unmapped execution records identified in source data |

## Test Coverage Summary

Total Use Cases: 3

Coverage Details:

| Metric | Count | Description |
|--------------------|-------|-----------------------------------------------------------------------------|
| Fully Covered | 0 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 3 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

| User Story ID | AC ID | Acceptance Criteria | Impact Level | Coverage Status |
|---------------|-------|---------------------|--------------|-----------------|
| LZ-001 | AC1 | Subscription Separation: Given the landing zone setup, when environments are created, then separate subscriptions must be used for Dev, QA, and Prod. | Medium | Partially Covered |
| LZ-001 | AC5 | Cost Center Tagging: Given any resource deployment, when the "Cost Center" tag is missing, then the deployment must fail validation. | High | Partially Covered |
| BRZ-001 | AC2 | Raw Format Preservation: Given the ingestion process, when data is landed in ADLS Gen2, then it must be stored in its source format (e.g., Parquet or Avro). | Medium | Partially Covered |
| BRZ-001 | AC3 | Metadata Capture: Given a successful ingestion, when the record is saved, then metadata (source system, load timestamp, file name) must be appended. | Medium | Partially Covered |
| BRZ-001 | AC4 | Retry Logic: Given a transient network failure, when the ingestion fails, then the system must automatically retry 3 times before triggering an alert. | Medium | Partially Covered |
| STG-001 | AC1 | Zone Creation: Given a new Data Lake account, when initialized, then separate root containers for /bronze, /silver, and /gold must be created. | Medium | Partially Covered |
| STG-001 | AC2 | Domain Organization: Given the /bronze container, when data is ingested, then it must be organized by domain folders (e.g., /sales, /finance). | Medium | Partially Covered |
| STG-001 | AC3 | Tiered Storage Policy: Given files in the /bronze layer, when they exceed 90 days of age, then they must automatically move to Cool storage via lifecycle policy. | Medium | Partially Covered |
| STG-001 | AC4 | Encryption Validation: Given data landing in any zone, when stored at rest, then it must be encrypted using Microsoft-managed and Customer-managed keys. | Critical | Partially Covered |

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| LZ-001 | 80.00% | 🟠 Amber |
| BRZ-001 | 70.00% | 🟠 Amber |
| STG-001 | 60.00% | 🔴 Red |

Legend:

- 🟢 Green (90–100%)
- 🟠 Amber (70–89%)
- 🔴 Red (<70%)

## Test Execution Summary

Execution Success Rate: 86.67%

Total Test Cases Executed: 45

Total Test Cases Not Executed: 0

Total Test Cases Passed: 39

Total Test Cases Failed: 6

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---------------|------------------|----------|--------------|--------|--------|----------------|-----------|
| LZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| STG-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |

All 45 mapped unit test cases were executed, resulting in an execution rate of 100.00% and an execution success rate of 86.67%.

Failures were distributed across all 3 user stories, with 2 failed test cases recorded in each user story.

Overall execution stability from input: 86.70%.

## Defect Details

Defect Rate: 13.33%

| Defect ID | Test Case ID | User Story ID | Defect Description | Category | Severity | Status |
|-----------|--------------|---------------|--------------------|----------|----------|--------|
| DEF_LZ-001_008 | UT_LZ-001_008 | LZ-001 | Network connection from Dev to Prod was not blocked by default, violating network segmentation policy. | policy_enforcement | high | open |
| DEF_LZ-001_013 | UT_LZ-001_013 | LZ-001 | Deployment with an empty 'Cost Center' tag value was not rejected, violating the mandatory tagging policy. | policy_enforcement | high | open |
| DEF_BRZ-001_002 | UT_BRZ-001_002 | BRZ-001 | Pipeline did not fail correctly with an IR connectivity error when the Self-Hosted Integration Runtime was offline. | connectivity | high | open |
| DEF_BRZ-001_009 | UT_BRZ-001_009 | BRZ-001 | Pipeline did not retry the specified 3 times upon persistent network failure before terminating. | functional_behavior | medium | open |
| DEF_STG-001_004 | UT_STG-001_004 | STG-001 | Ingestion pipeline did not auto-create a missing domain folder, leading to data being placed in an incorrect location. | functional_behavior | medium | open |
| DEF_STG-001_011 | UT_STG-001_011 | STG-001 | A user with only Bronze-level permissions was able to access data in the Gold container, violating ACL policy. | security | critical | open |

## Conclusion

A total of 3 user stories were reviewed.

Coverage distribution shows 0 fully covered, 3 partially covered, and 0 not covered user stories.

The overall test coverage rate is 70.00%, the execution success rate is 86.67%, and the defect rate is 13.33%.

Based on the reported overall coverage rate of 70.00%, overall execution stability of 86.70%, and the presence of open defects including critical severity, the current unit test baseline remains in a partially covered state with unresolved quality issues.

The current unit test suite is not sufficient to proceed without remediation. Coverage gaps and open defects, including critical severity findings, require resolution before progression.
