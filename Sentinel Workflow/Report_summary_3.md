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

The baseline reference for measuring coverage, execution success, and defect quality is limited to the following user stories: LZ-001, BRZ-001, and STG-001.

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
|----------------|-------|---------------------|--------------|-----------------|
| BRZ-001 | AC2 | Raw Format Preservation: Given the ingestion process, when data is landed in ADLS Gen2, then it must be stored in its source format (e.g., Parquet or Avro). | NULL | Partially Covered |
| STG-001 | AC1 | Zone Creation: Given a new Data Lake account, when initialized, then separate root containers for /bronze, /silver, and /gold must be created. | NULL | Partially Covered |

| User Story ID | Coverage Score | Color |
|---------------|----------------|-------|
| LZ-001 | 100.00% | 🟢 Green |
| BRZ-001 | 90.00% | 🟢 Green |
| STG-001 | 90.00% | 🟢 Green |

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

Total Test Cases Executed: 45

Total Test Cases Not Executed: 0

Total Test Cases Passed: 39

Total Test Cases Failed: 6

Execution Success Rate: 86.67%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---------------|------------------|----------|--------------|--------|--------|----------------|-----------|
| LZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| STG-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |

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
|-----------|--------------|---------------|--------------|--------------------|----------|----------|--------|
| DEF_LZ-001_008 | UT_LZ-001_008 | LZ-001 | NULL | Dev-to-Prod network connection blocking was not observed as expected during execution. | network_segmentation | high | open |
| DEF_LZ-001_013 | UT_LZ-001_013 | LZ-001 | NULL | Deployment with empty or null Cost Center tag value was not rejected as expected. | policy_enforcement | medium | open |
| DEF_BRZ-001_002 | UT_BRZ-001_002 | BRZ-001 | NULL | Expected failure handling for offline Self-Hosted Integration Runtime did not occur as designed. | connectivity_runtime | high | open |
| DEF_BRZ-001_009 | UT_BRZ-001_009 | BRZ-001 | NULL | Pipeline did not terminate and alert correctly after 3 retry attempts under persistent network failure. | retry_logic | high | open |
| DEF_STG-001_004 | UT_STG-001_004 | STG-001 | NULL | Missing domain folder handling did not auto-create or reject ingestion as expected. | folder_hierarchy | medium | open |
| DEF_STG-001_011 | UT_STG-001_011 | STG-001 | NULL | User with Bronze-only access was not denied Gold container access as expected. | access_control | critical | open |

## Conclusion

Summary of Findings

A total of 3 user stories were reviewed. Coverage distribution shows 1 fully covered user story, 2 partially covered user stories, and 0 not covered user stories. The overall test coverage rate is 93.30%, the execution success rate is 86.67%, and the defect rate is 13.33%.

Final Outcome Statement

The overall average coverage score is 93.30%, and the overall execution stability is 86.67%. Defect severity includes high, medium, and critical open defects. Based on these reported values, remediation is required before progression.

Conclusion Statement

The current unit test suite demonstrates broad mapped coverage across the evaluated user stories; however, open failed tests and recorded critical, high, and medium defects indicate that remediation is required before proceeding.
