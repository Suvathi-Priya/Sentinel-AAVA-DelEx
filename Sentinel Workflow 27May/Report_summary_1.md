# UNIT TEST QUALITY & COVERAGE REPORT

## Scope

This report evaluates unit test coverage and quality across 3 user stories. These user stories form the baseline for evaluation.

The scope is restricted to unit test plans and execution records mapped to these user stories. The analysis includes unit test cases linked to the identified user stories, test execution results (executed, not executed, passed, failed), and defect data directly associated with these user stories.

The analysis excludes integration tests, system tests, performance tests, user stories not mapped to test cases, and any external or unrelated defect logs.

The baseline reference for measuring coverage, execution success, and defect quality is limited to the following user stories: SLV-003, GLD-001, and SEC-002.

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
| GLD-001 | AC4 | Performance Partitioning Given large datasets in Gold, when stored in Synapse/Fabric, then tables must be partitioned by 'Business Period' (e.g., Fiscal Year) for query optimization. | Medium | Partially Covered |
| SEC-002 | AC4 | Key Vault Secret Rotation Given application secrets, when accessed by the reporting layer, then they must be retrieved from Azure Key Vault with no hardcoded values. | High | Partially Covered |

Coverage Score:

| User Story ID | Coverage Score | Color |
|---|---:|---|
| GLD-001 | 90.00% | 🟢 Green |
| SEC-002 | 90.00% | 🟢 Green |

Legend:

- 🟢 Green (90–100%) → High coverage (meets quality expectations)
- 🟠 Amber (70–89%) → Moderate coverage (requires attention)
- 🔴 Red (<70%) → Low coverage (critical gaps present)

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
| SLV-003 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| GLD-001 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |
| SEC-002 | 15 | 15 | 0 | 13 | 2 | 100.00% | 86.67% |

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
| DEF_SLV-003_007 | UT_SLV-003_007 | SLV-003 | NULL | Validate referential integrity check when the reference table is temporarily unavailable during the Silver load. Defect raised for investigation and fix. | Functional | High | open |
| DEF_SLV-003_012 | UT_SLV-003_012 | SLV-003 | NULL | Validate stop-on-failure threshold behavior when the error rate is exactly 5.0%. Defect raised for investigation and fix. | Functional | High | open |
| DEF_GLD-001_005 | UT_GLD-001_005 | GLD-001 | NULL | Validate KPI pre-calculation when source Silver data contains null values in fields used for KPI computation. Defect raised for investigation and fix. | Functional | Medium | open |
| DEF_GLD-001_014 | UT_GLD-001_014 | GLD-001 | NULL | Validate Star Schema foreign key relationships when a Dimension table record is deleted that is still referenced by the Fact table. Defect raised for investigation and fix. | Functional | High | open |
| DEF_SEC-002_002 | UT_SEC-002_002 | SEC-002 | NULL | Validate RBAC group assignment when a user is removed from an Entra ID group and their access to Gold resources is revoked. Defect raised for investigation and fix. | Security | Critical | open |
| DEF_SEC-002_007 | UT_SEC-002_007 | SEC-002 | NULL | Validate RLS behavior when a user is not assigned to any region in the security configuration. Defect raised for investigation and fix. | Security | High | open |

Defect pattern summary: 6 defects were recorded across 3 user stories. Severity distribution includes 1 Critical, 4 High, and 1 Medium defect. Category distribution includes Functional and Security defects. Affected areas include referential integrity, stop-on-failure threshold handling, KPI computation with null values, Star Schema relationship handling, RBAC access revocation, and RLS behavior.

## Conclusion

Summary of Findings:

A total of 3 user stories were reviewed. Coverage distribution shows 1 fully covered user story, 2 partially covered user stories, and 0 not covered user stories. The overall test coverage rate is 93.30%, the execution success rate is 86.70%, and the defect rate is 13.33%.

Final Outcome Statement:

Based on the reported overall test coverage rate of 93.30%, overall execution success rate of 86.70%, and the presence of Critical, High, and Medium severity defects, the current unit test results indicate that remediation is required for failed scenarios and open defects.

Conclusion Statement:

The unit test suite demonstrates broad coverage and full execution across the evaluated baseline. Remediation is required before progression due to open defects and failed test results.
