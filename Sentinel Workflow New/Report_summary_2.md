# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories.

The 3 user stories form the baseline for evaluation. The scope is restricted to unit test plans and execution records mapped to these user stories.

Included in scope are unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

Excluded from scope are integration tests, system tests, performance tests, user stories not mapped to test cases, and external or unrelated defect logs.

The baseline reference for measuring coverage, execution success, and defect quality is limited to the following user stories: LZ-001, BRZ-001, and STG-001.

## Test Coverage Summary

Total Use Cases: 3

Coverage Details:

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 3 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 0 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

Coverage Gap Details:

| User Story ID | AC ID | Acceptance Criteria | Impact Level | Coverage Status |
|---|---|---|---|---|
| NULL | NULL | NULL | NULL | NULL |

| User Story ID | Coverage Score | Color |
|---|---:|---|
| LZ-001 | 100.00% | 🟢 Green |
| BRZ-001 | 100.00% | 🟢 Green |
| STG-001 | 100.00% | 🟢 Green |

Legend:

🟢 Green (90–100%) → High coverage (meets quality expectations)

🟠 Amber (70–89%) → Moderate coverage (requires attention)

🔴 Red (<70%) → Low coverage (critical gaps present)

Coverage Score Analysis:

Coverage % = (Covered Acceptance Criteria / Total Acceptance Criteria) × 100

Description:

Coverage Percentage measures the extent to which acceptance criteria are validated by corresponding test cases. It indicates how completely the defined requirements are covered through testing.

Components:

Covered Acceptance Criteria: Number of acceptance criteria that have at least one mapped test case

Total Acceptance Criteria: Total number of acceptance criteria defined across user stories

## Test Execution Summary

Total Test Cases Executed: 45

Total Test Cases Not Executed: 0

Total Test Cases Passed: 39

Total Test Cases Failed: 6

Execution Success Rate: 86.67%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---|---:|---:|---:|---:|---:|---:|---:|
| LZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| STG-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |

Results show that all 45 test cases were executed, with an overall execution success rate of 86.67%.

Failures are concentrated equally across LZ-001, BRZ-001, and STG-001, with 2 failed test cases in each user story. The execution rate is 100.00% for all user stories, while the pass rate is 86.67% for each user story.

The execution success rate reflects complete execution coverage with observed failures remaining open through associated defects.

## Defect Details

Defect Rate: 13.33%

Defect Rate Analysis:

Defect Rate = (Total Defects / Total Test Cases) × 100

Description:

Defect Rate measures the proportion of defects identified during testing relative to the total number of test cases executed. It is a key quality metric used to evaluate system stability and testing effectiveness.

Components:

Total Defects: Total number of defects identified during the test cycle

Total Test Cases: Total number of test cases executed

Defect Details:

| Defect ID | Test Case ID | User Story ID | Defect Title | Defect Description | Category | Severity | Status |
|---|---|---|---|---|---|---|---|
| DEF_LZ-001_008 | UT_LZ-001_008 | LZ-001 | NULL | Dev-to-Prod network connection blocking did not behave as expected during execution. | network_segmentation | high | open |
| DEF_LZ-001_013 | UT_LZ-001_013 | LZ-001 | NULL | Mandatory tag validation for empty or null tag value did not behave as expected during execution. | policy_enforcement | medium | open |
| DEF_BRZ-001_002 | UT_BRZ-001_002 | BRZ-001 | NULL | Pipeline behavior when Self-Hosted Integration Runtime is offline did not meet expected failure and alerting behavior. | integration_runtime | high | open |
| DEF_BRZ-001_009 | UT_BRZ-001_009 | BRZ-001 | NULL | Pipeline retry termination and alerting after persistent network failure beyond 3 attempts did not behave as expected. | retry_alerting | high | open |
| DEF_STG-001_004 | UT_STG-001_004 | STG-001 | NULL | Behavior for ingestion into a missing domain folder within /bronze did not meet expected auto-create or controlled rejection behavior. | folder_hierarchy | medium | open |
| DEF_STG-001_011 | UT_STG-001_011 | STG-001 | NULL | A user with only /bronze access was not reliably denied from reading the /gold container during execution. | access_control | critical | open |

Results show that 6 defects were identified across 45 executed test cases, resulting in a defect rate of 13.33%.

Defects are distributed across network segmentation, policy enforcement, integration runtime, retry alerting, folder hierarchy, and access control categories. Severity distribution includes 1 critical, 3 high, and 2 medium defects.

The analysis indicates that all recorded defects remain in open status.

## Conclusion

Summary of Findings:

The analysis reviewed 3 user stories. Coverage distribution shows 3 fully covered, 0 partially covered, and 0 not covered user stories.

Execution results show 45 executed test cases, 39 passed, and 6 failed, with an execution success rate of 86.67%. Defect results show 6 defects, producing a defect rate of 13.33%.

Final Outcome Statement:

The overall coverage rate is 100.00%, and the overall execution success rate is 86.70% based on the provided metrics. Defect severity includes medium, high, and critical defects, with one critical defect recorded.

Conclusion Statement:

The current unit test suite demonstrates complete mapped coverage across the evaluated user stories; however, remediation is required before progression due to 6 failed tests and the presence of open medium, high, and critical defects.