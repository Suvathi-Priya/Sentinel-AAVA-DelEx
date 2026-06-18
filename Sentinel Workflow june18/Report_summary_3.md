<div align="center">

# **UNIT TEST QUALITY & COVERAGE REPORT**

</div>

# Scope

This report evaluates unit test coverage and quality across 7 user stories. The scope is restricted to test plans and execution records mapped to these user stories.

Analysis excludes non-unit test activities and unrelated defect categories. The user stories form the baseline for evaluation, and the scope is limited to unit test coverage and execution records mapped to these user stories.

# Coverage Gap Details

| User Story ID | AC ID | Coverage Gap Reason | Coverage Status |
|---------------|-------|---------------------|-----------------|
| 1836 | AC1 | No testcase explicitly validates creation of refund requests for eligible orders. | Not Covered |
| 1836 | AC2 | No testcase explicitly validates sending refund approval notifications to customers. | Not Covered |
| 1836 | AC3 | No testcase explicitly validates refund status viewability by customers in the portal. | Not Covered |
| 1836 | AC4 | No testcase explicitly validates capture of customer ID in refund audit logs.; No testcase explicitly validates capture of refund amount in refund audit logs.; No testcase explicitly validates capture of approval timestamp in refund audit logs. | Not Covered |
| 1836 | AC5 | No testcase explicitly validates refunds above $1000 threshold.; No testcase explicitly validates manager approval requirement for high-value refunds.; No testcase explicitly validates fraud review requirement for high-value refunds. | Not Covered |
| 1844 | AC1 | No testcase explicitly validates customers submitting subscription pause requests.; No testcase explicitly validates inclusion of pause start date in pause requests.; No testcase explicitly validates inclusion of pause reason in pause requests. | Not Covered |
| 1844 | AC2 | No testcase explicitly validates sending pause confirmation notifications to customers.; No testcase explicitly validates inclusion of pause start date in pause confirmation notifications.; No testcase explicitly validates inclusion of resume date in pause confirmation notifications. | Not Covered |
| 1844 | AC3 | No testcase explicitly validates viewing pause status in the customer portal.; No testcase explicitly validates viewing pause history in the customer portal.; No testcase explicitly validates viewing scheduled resume date in the customer portal. | Not Covered |
| 1844 | AC4 | No testcase explicitly validates capture of customer ID in pause audit logs.; No testcase explicitly validates capture of subscription ID in pause audit logs.; No testcase explicitly validates capture of pause reason in pause audit logs.; No testcase explicitly validates capture of pause start date in pause audit logs.; No testcase explicitly validates capture of timestamp in pause audit logs. | Not Covered |
| 1844 | AC5 | No testcase explicitly validates pause requests exceeding 90 days threshold.; No testcase explicitly validates manager approval requirement before pause activation for requests exceeding 90 days. | Not Covered |
| 1858 | AC1 | No testcase explicitly validates sending email notifications for all completed transactions. | Not Covered |
| 1858 | AC2 | No testcase explicitly validates sending SMS notifications for high-priority alerts. | Not Covered |
| 1858 | AC3 | No testcase explicitly validates push notifications being configurable per user preference. | Not Covered |
| 1858 | AC4 | No testcase explicitly validates capture of customer ID in notification logs.; No testcase explicitly validates capture of notification type in notification logs.; No testcase explicitly validates capture of timestamp in notification logs. | Not Covered |
| 1858 | AC5 | No testcase explicitly validates failed notifications triggering retry attempts.; No testcase explicitly validates retry attempts up to 3 times threshold. | Not Covered |
| 1860 | AC1 | No testcase explicitly validates performing UPSERT (Merge) based on the unique Business Key. | Not Covered |
| 1860 | AC2 | No testcase explicitly validates deletion of corresponding record in the Silver Delta table when record is deleted in source system. | Not Covered |
| 1860 | AC3 | No testcase explicitly validates refreshing UpdateTimestamp metadata column during Merge.; No testcase explicitly validates refreshing SourceSystem metadata column during Merge. | Not Covered |
| 1860 | AC4 | No testcase explicitly validates logging number of inserted rows in the monitoring table.; No testcase explicitly validates logging number of updated rows in the monitoring table.; No testcase explicitly validates logging number of deleted rows in the monitoring table. | Not Covered |
| 1860 | AC5 | No testcase explicitly validates updating high-watermark timestamp to ensure next run only picks up new data. | Not Covered |
| 1852 | AC1 | No testcase explicitly validates customers submitting downgrade request.; No testcase explicitly validates selecting target lower plan in downgrade request.; No testcase explicitly validates selecting desired effective date in downgrade request. | Not Covered |
| 1852 | AC2 | No testcase explicitly validates sending downgrade confirmation notifications to customers.; No testcase explicitly validates detailing new plan features in downgrade confirmation notifications.; No testcase explicitly validates detailing effective date in downgrade confirmation notifications.; No testcase explicitly validates detailing adjusted billing amount in downgrade confirmation notifications. | Not Covered |
| 1852 | AC3 | No testcase explicitly validates viewing downgrade request status in the customer portal.; No testcase explicitly validates viewing plan comparison in the customer portal.; No testcase explicitly validates viewing credit adjustments in the customer portal. | Not Covered |
| 1852 | AC4 | No testcase explicitly validates capture of customer ID in downgrade audit logs.; No testcase explicitly validates capture of subscription ID in downgrade audit logs.; No testcase explicitly validates capture of previous plan in downgrade audit logs.; No testcase explicitly validates capture of downgraded plan in downgrade audit logs.; No testcase explicitly validates capture of effective date in downgrade audit logs.; No testcase explicitly validates capture of credit issued in downgrade audit logs.; No testcase explicitly validates capture of timestamp in downgrade audit logs. | Not Covered |
| 1852 | AC5 | No testcase explicitly validates downgrade requests from enterprise-tier plans.; No testcase explicitly validates account manager approval requirement for enterprise-tier downgrade requests.; No testcase explicitly validates customer retention review requirement before processing enterprise-tier downgrade requests. | Not Covered |
| 1848 | AC1 | No testcase explicitly validates customers submitting cancellation request.; No testcase explicitly validates specifying cancellation reason in cancellation request.; No testcase explicitly validates specifying preferred cancellation date in cancellation request. | Not Covered |
| 1848 | AC2 | No testcase explicitly validates sending cancellation confirmation notifications to customers.; No testcase explicitly validates including effective cancellation date in cancellation confirmation notifications.; No testcase explicitly validates including applicable refund details in cancellation confirmation notifications. | Not Covered |
| 1848 | AC3 | No testcase explicitly validates viewing cancellation request status in the customer portal.; No testcase explicitly validates viewing refund status in the customer portal.; No testcase explicitly validates viewing service end date in the customer portal. | Not Covered |
| 1848 | AC4 | No testcase explicitly validates capture of customer ID in cancellation audit logs.; No testcase explicitly validates capture of subscription ID in cancellation audit logs.; No testcase explicitly validates capture of cancellation reason in cancellation audit logs.; No testcase explicitly validates capture of effective date in cancellation audit logs.; No testcase explicitly validates capture of refund amount in cancellation audit logs.; No testcase explicitly validates capture of timestamp in cancellation audit logs. | Not Covered |
| 1848 | AC5 | No testcase explicitly validates cancellation requests with outstanding balances greater than $500 threshold.; No testcase explicitly validates finance team approval requirement before cancellation processing for requests with outstanding balances greater than $500. | Not Covered |
| 1856 | AC1 | No testcase explicitly validates awarding loyalty points for eligible purchases. | Not Covered |
| 1856 | AC2 | No testcase explicitly validates customers redeeming loyalty points for rewards. | Not Covered |
| 1856 | AC3 | No testcase explicitly validates loyalty points balance viewability by customers in the portal. | Not Covered |
| 1856 | AC4 | No testcase explicitly validates capture of customer ID in loyalty transaction logs.; No testcase explicitly validates capture of points earned or redeemed in loyalty transaction logs.; No testcase explicitly validates capture of transaction timestamp in loyalty transaction logs. | Not Covered |
| 1856 | AC5 | No testcase explicitly validates reward redemptions above 5000 points threshold.; No testcase explicitly validates manager approval requirement for reward redemptions above 5000 points.; No testcase explicitly validates fraud review requirement for reward redemptions above 5000 points. | Not Covered |

# Consistency Analysis

### Data Mapping Inconsistency Details


### Consistency Metrics Summary

| Metric | Count |
|---------|-------|
| Total Test Cases | 0 |
| Total Test Logs | 0 |
| Missing Test Cases | 0 |
| Missing Test Logs | 0 |
| Consistency Status | No testcases or test execution logs available |

# Defect Details

No defects reported for User Story 1836.

No defects reported for User Story 1844.

No defects reported for User Story 1858.

No defects reported for User Story 1860.

No defects reported for User Story 1852.

No defects reported for User Story 1848.

No defects reported for User Story 1856.

### Defect Details


# Conclusion

Remediation is required as all user stories are Not Covered.
