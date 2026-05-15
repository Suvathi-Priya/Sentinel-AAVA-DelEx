# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories.

The 3 user stories form the baseline for evaluation.

The scope is restricted to unit test plans and execution records mapped to these user stories.

Included within scope are unit test cases linked to the identified user stories, test execution results recorded as executed, not executed, passed, and failed, and defect data directly associated with these user stories.

Excluded from scope are integration tests, system tests, performance tests, user stories not mapped to test cases, and any external or unrelated defect logs.

The baseline reference for measuring coverage, execution success, and defect quality is limited to the following user stories: LZ-001, BRZ-001, and STG-001.

## Test Coverage Summary

Total Use Cases: 3

Coverage Details:

| Metric | Count | Description |
|---|---:|---|
| Fully Covered | 0 | User stories where all acceptance criteria are covered by test cases |
| Partially Covered | 3 | User stories containing a mix of covered and uncovered acceptance criteria |
| Not Covered | 0 | User stories where none of the acceptance criteria are covered by test cases |

Coverage Gap Details:

| User Story ID | AC ID | Acceptance Criteria | Impact Level | Coverage Status |
|---|---|---|---|---|
| LZ-001 | AC4 | Network connection attempts from Dev environment resources to Prod resources are blocked by default | high | Partially Covered |
| BRZ-001 | AC1 | ADF pipeline connecting to an on-premises SQL database uses a Self-Hosted Integration Runtime | high | Partially Covered |
| BRZ-001 | AC4 | Pipeline automatically retries multiple times after a transient network failure before triggering an alert | high | Partially Covered |
| STG-001 | AC2 | Data ingested into the /bronze container is organized under domain-specific sub-folders | medium | Partially Covered |
| STG-001 | AC5 | User with only /bronze access is denied when attempting to read from the /gold container | critical | Partially Covered |

| User Story ID | Coverage Score | Color |
|---|---:|---|
| LZ-001 | 90.00% | 🟢 Green |
| BRZ-001 | 80.00% | 🟠 Amber |
| STG-001 | 80.00% | 🟠 Amber |

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

Total Test Cases Passed: 36

Total Test Cases Failed: 4

Execution Success Rate: 80.00%

Test Execution Summary Details:

| User Story ID | Total Test Cases | Executed | Not Executed | Passed | Failed | Execution Rate | Pass Rate |
|---|---:|---:|---:|---:|---:|---:|---:|
| LZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| BRZ-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| STG-001 | 15 | 15 | 0 | 11 | 0 | 100.00% | 86.67% |

Execution Success Rate = (Test cases Passed / Test Cases Executed) × 100

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
| DEF_LZ-001_008 | UT_LZ-001_008 | LZ-001 | NULL | Dev-to-Prod network connection blocking did not behave as expected during execution, indicating default segmentation enforcement failure against AC4. | network_segmentation | high | open |
| DEF_LZ-001_013 | UT_LZ-001_013 | LZ-001 | NULL | Mandatory tag validation for empty or null tag value did not behave as expected, indicating incomplete enforcement of AC5 boundary validation. | policy_enforcement | medium | open |
| DEF_BRZ-001_002 | UT_BRZ-001_002 | BRZ-001 | NULL | Pipeline behavior under offline Self-Hosted Integration Runtime did not meet expected failure-handling behavior, including alerting and prevention of partial writes. | integration_runtime | high | open |
| DEF_BRZ-001_009 | UT_BRZ-001_009 | BRZ-001 | NULL | Pipeline did not correctly terminate and alert after retry exhaustion beyond 3 attempts as required by AC4. | retry_logic | high | open |
| DEF_STG-001_004 | UT_STG-001_004 | STG-001 | NULL | Missing-domain-folder ingestion behavior was not fully validated; expected auto-create or clean rejection behavior was not observed correctly. | folder_hierarchy | medium | open |
| DEF_STG-001_011 | UT_STG-001_011 | STG-001 | NULL | Bronze-only user denial to /gold container was not observed as expected, indicating possible ACL enforcement failure against AC5. | access_control | critical | open |

Results show that 6 defects were recorded across 45 executed test cases. Failures are concentrated in network segmentation, policy enforcement, integration runtime handling, retry logic, folder hierarchy behavior, and access control. Severity distribution includes medium, high, and critical defects.

## Conclusion

Summary of Findings:

The analysis reviewed 3 user stories. Coverage distribution shows 0 fully covered, 3 partially covered, and 0 not covered user stories. The overall test coverage rate is 83.30%, the execution success rate is 80.00%, and the defect rate is 13.33%.

Final Outcome Statement:

The final outcome is not_ready. This result is supported by the overall test coverage rate of 83.30%, overall execution success rate of 80.00%, and the presence of open high and critical severity defects.

Conclusion Statement:

The current unit test suite is not ready to proceed based on the reported coverage, execution, and defect results. Remediation is required before progression.
