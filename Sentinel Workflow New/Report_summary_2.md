# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 2 user stories.

These 2 user stories form the baseline for evaluation. The scope is restricted to unit test coverage, unit test execution records, and defect data directly mapped to these user stories.

Included in scope:
- Unit test cases linked to the identified user stories.
- Test execution results covering executed, not executed, passed, and failed outcomes.
- Defect data directly associated with these user stories.

Excluded from scope:
- Integration tests, system tests, and performance tests.
- User stories not mapped to test cases.
- External or unrelated defect logs.

The baseline reference for measuring coverage, execution success, and defect quality is limited to the mapped user stories: LZ-001 and BRZ-001.

## Test Coverage Summary

Total Use Cases: 2

Coverage Details:

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 1 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 1 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

Coverage Gap Details:

| User Story ID | AC ID | Acceptance Criteria | Impact Level | Coverage Status |
|---|---|---|---|---|
| BRZ-001 | AC2 | Raw Format Preservation: Given the ingestion process, when data is landed in ADLS Gen2, then it must be stored in its source format (e.g., Parquet or Avro). | NULL | Partially Covered |

Coverage Score:

| User Story ID | Coverage Score | Color |
|---|---:|---|
| BRZ-001 | 90.00% | 🟢 Green |

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

Total Test Cases Executed: 30

Total Test Cases Not Executed: 0

Total Test Cases Passed: 26

Total Test Cases Failed: 4

Execution Success Rate: 86.67%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---|---:|---:|---:|---:|---:|---:|---:|
| LZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |

Execution Success Rate = (Test Cases Passed / Test Cases Executed) × 100

Overall execution status is based on 30 executed test cases, with 26 passed and 4 failed. Failures are distributed across both user stories, with 2 failed test cases in LZ-001 and 2 failed test cases in BRZ-001. Execution records show full execution coverage with no unexecuted test cases.

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
| DEF_LZ-001_008 | UT_LZ-001_008 | LZ-001 | NULL | Dev-to-Prod network connection blocking did not behave as expected during execution. | network_segmentation | high | open |
| DEF_LZ-001_013 | UT_LZ-001_013 | LZ-001 | NULL | Deployment with Cost Center tag present but empty or null was not rejected as expected. | policy_enforcement | medium | open |
| DEF_BRZ-001_002 | UT_BRZ-001_002 | BRZ-001 | NULL | Pipeline behavior when Self-Hosted Integration Runtime was offline did not match expected failure and alerting behavior. | connectivity_runtime | high | open |
| DEF_BRZ-001_009 | UT_BRZ-001_009 | BRZ-001 | NULL | Persistent network failure handling beyond 3 retry attempts did not match expected termination and alert behavior. | retry_logic | high | open |

Defect patterns are concentrated in network segmentation, policy enforcement, connectivity runtime, and retry logic areas. Severity distribution includes 3 high defects and 1 medium defect. All recorded defects are in open status.

## Conclusion

Summary of Findings:

A total of 2 user stories were reviewed. Coverage distribution shows 1 fully covered user story, 1 partially covered user story, and 0 not covered user stories. The overall test coverage rate is 95.00%, execution success rate is 86.67%, and defect rate is 13.33%.

Final Outcome Statement:

The overall coverage rate is 95.00%, the overall execution stability is 86.67%, and the recorded defect severity profile includes 3 high defects and 1 medium defect. Based on these reported values, the unit test suite shows high coverage with execution failures and open defects present across both user stories.

Conclusion Statement:

The current unit test suite is not sufficient to proceed without remediation. Failed test cases and open defects require resolution before progression.
