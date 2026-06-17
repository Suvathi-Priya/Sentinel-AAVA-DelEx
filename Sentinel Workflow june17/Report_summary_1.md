<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 10 user stories. The scope is restricted to test plans and execution records mapped to these user stories. Analysis excludes non-unit test activities and unrelated defect categories.

**Total User Stories:** 10

The coverage boundary encompasses all acceptance criteria within the identified user stories, forming the baseline for unit test coverage evaluation. No unit test cases or execution records were available in the provided input data.

# Test Coverage Summary

## Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|-------------------|-----------------|
| 1848 | AC1 | No testcase explicitly validates automatic capture of data from Event Hub stream into ADLS Gen2.; No testcase explicitly validates capture in Avro/Parquet format. | Not Covered |
| 1848 | AC2 | No testcase explicitly validates partitioning by year/month/day/hour for performance. | Not Covered |
| 1848 | AC3 | No testcase explicitly validates incoming JSON payload against registered schema.; No testcase explicitly validates routing of non-matching payload to dead-letter folder for review. | Not Covered |
| 1848 | AC4 | No testcase explicitly validates message visibility in Bronze layer within 5 minutes. | Not Covered |
| 1848 | AC5 | No testcase explicitly validates Event Hub auto-scaling when throughput exceeds limits.; No testcase explicitly validates prevention of data loss. | Not Covered |
| 1856 | AC1 | No testcase explicitly validates granting permissions via Microsoft Entra ID groups. | Not Covered |
| 1856 | AC2 | No testcase explicitly validates masking of PII data when queried by non-authorized users. | Not Covered |
| 1856 | AC3 | No testcase explicitly validates that regional manager sees only data associated with their specific region. | Not Covered |
| 1856 | AC4 | No testcase explicitly validates retrieval of secrets from Azure Key Vault.; No testcase explicitly validates absence of hardcoded values. | Not Covered |
| 1856 | AC5 | No testcase explicitly validates logging of User ID.; No testcase explicitly validates logging of Timestamp.; No testcase explicitly validates logging of Query string. | Not Covered |
| 1846 | AC1 | No testcase explicitly validates creation of separate root container /bronze.; No testcase explicitly validates creation of separate root container /silver.; No testcase explicitly validates creation of separate root container /gold. | Not Covered |
| 1846 | AC2 | No testcase explicitly validates organization of data by domain folders. | Not Covered |
| 1846 | AC3 | No testcase explicitly validates files exceeding 90 days of age.; No testcase explicitly validates automatic movement to Cool storage via lifecycle policy. | Not Covered |
| 1846 | AC4 | No testcase explicitly validates encryption of data at rest using Microsoft-managed or Customer-managed keys. | Not Covered |
| 1846 | AC5 | No testcase explicitly validates denial of access to Gold container when user lacks specific permissions. | Not Covered |
| 1836 | AC1 | No testcase explicitly validates use of separate subscription for Dev.; No testcase explicitly validates use of separate subscription for QA.; No testcase explicitly validates use of separate subscription for Prod. | Not Covered |
| 1836 | AC2 | No testcase explicitly validates grouping of resources into Resource Groups based on environment. | Not Covered |
| 1836 | AC3 | No testcase explicitly validates following of defined enterprise naming standards.; No testcase explicitly validates blocking of resource creation by policy when naming standards not followed. | Not Covered |
| 1836 | AC4 | No testcase explicitly validates blocking of connection from Dev to Prod by default. | Not Covered |
| 1836 | AC5 | No testcase explicitly validates failure of deployment validation when Cost Center tag is missing. | Not Covered |
| 1854 | AC1 | No testcase explicitly validates structuring of data into Fact tables.; No testcase explicitly validates structuring of data into Dimension tables. | Not Covered |
| 1854 | AC2 | No testcase explicitly validates pre-calculation of standard KPIs. | Not Covered |
| 1854 | AC3 | No testcase explicitly validates provision of unified Customer 360 view. | Not Covered |
| 1854 | AC4 | No testcase explicitly validates partitioning of tables by Business Period for query optimization. | Not Covered |
| 1854 | AC5 | No testcase explicitly validates that data reflects all transactions up to previous midnight when queried at 8:00 AM. | Not Covered |
| 1858 | AC1 | No testcase explicitly validates moving of record to Quarantine folder when key columns are empty. | Not Covered |
| 1858 | AC2 | No testcase explicitly validates triggering of alert when values fall outside predefined logical ranges. | Not Covered |
| 1858 | AC3 | No testcase explicitly validates flagging of record as orphan when associated Master Key does not exist in reference table. | Not Covered |
| 1858 | AC4 | No testcase explicitly validates generation of summary report with Pass/Fail counts for dashboard. | Not Covered |
| 1858 | AC5 | No testcase explicitly validates error rate exceeding 5% records fail.; No testcase explicitly validates pipeline stopping.; No testcase explicitly validates notification of engineering team. | Not Covered |
| 1860 | AC1 | No testcase explicitly validates performing UPSERT (Merge) based on unique Business Key. | Not Covered |
| 1860 | AC2 | No testcase explicitly validates logical or physical deletion of corresponding record in Silver Delta table. | Not Covered |
| 1860 | AC3 | No testcase explicitly validates refreshing of UpdateTimestamp metadata column.; No testcase explicitly validates refreshing of SourceSystem metadata column. | Not Covered |
| 1860 | AC4 | No testcase explicitly validates logging of number of inserted rows in monitoring table.; No testcase explicitly validates logging of number of updated rows in monitoring table.; No testcase explicitly validates logging of number of deleted rows in monitoring table. | Not Covered |
| 1860 | AC5 | No testcase explicitly validates updating of high-watermark timestamp to ensure next run picks up only new data. | Not Covered |
| 1850 | AC1 | No testcase explicitly validates enabling of System-Assigned Managed Identity. | Not Covered |
| 1850 | AC2 | No testcase explicitly validates assignment of Storage Blob Data Contributor role. | Not Covered |
| 1850 | AC3 | No testcase explicitly validates selection of Managed Identity authentication method. | Not Covered |
| 1850 | AC4 | No testcase explicitly validates use of identity to fetch secret from Azure Key Vault. | Not Covered |
| 1850 | AC5 | No testcase explicitly validates logging of action in Azure Activity Log with Identity ID. | Not Covered |
| 1844 | AC1 | No testcase explicitly validates use of Self-Hosted Integration Runtime. | Not Covered |
| 1844 | AC2 | No testcase explicitly validates storage of data in source format. | Not Covered |
| 1844 | AC3 | No testcase explicitly validates appending of source system metadata.; No testcase explicitly validates appending of load timestamp metadata.; No testcase explicitly validates appending of file name metadata. | Not Covered |
| 1844 | AC4 | No testcase explicitly validates automatic retry 3 times.; No testcase explicitly validates triggering of alert after 3 retries. | Not Covered |
| 1844 | AC5 | No testcase explicitly validates that pipeline must not fail.; No testcase explicitly validates capture of new columns. | Not Covered |
| 1852 | AC1 | No testcase explicitly validates conversion of all date columns to ISO 8601 format (YYYY-MM-DD). | Not Covered |
| 1852 | AC2 | No testcase explicitly validates flagging of record when null value detected.; No testcase explicitly validates assignment of default Unknown value when null value detected. | Not Covered |
| 1852 | AC3 | No testcase explicitly validates retention of only latest record based on LoadTimestamp. | Not Covered |
| 1852 | AC4 | No testcase explicitly validates conversion of currency or measurements to enterprise standard. | Not Covered |
| 1852 | AC5 | No testcase explicitly validates that operation fails when incoming data schema does not match Silver table definition. | Not Covered |

# Consistency Analysis

## Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 0 |
| Total Test Logs | 0 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Consistency Status | No testcases or test execution logs available |

# Defect Details

No defects reported for this analysis.

# Conclusion

Remediation is required as all user stories are Not Covered and no unit test cases or execution records are available for validation.
