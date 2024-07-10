---
description: >-
  This section will highlight important requirements or describe any additional
  cross-cutting requirements that apply to this Building Block.
---

# Cross-Cutting Requirements

## Personal Data Privacy (REQUIRED)

Personal data must be kept private and never shared with any parties, except where specific authorization has been granted. The Consent Building Block shall follow the privacy principles as laid out in the Beckn-Onix architecture and security recommendations.

## All transactions must be Audit Logged  (RECOMMENDED)

Logs should be kept in a database of all created, updated, or deleted records. Logs must include timestamps and identify the user and affiliation that performed the transaction.

All audit logs shall be integrity-protected against tampering. The Consent Building Block shall follow the data policy and audit logging requirements as laid out in the Beckn-Onix 

## Rollback capability (RECOMMENDED)

The Building Block must perform various activities starting from initiation of purchase request/expression of interest to completion of order with feedback etc. In case of any non-compliance (due to both technical and functional reasons), it should be able to roll back to the initial state to safeguard the integrity of the application.

## Performance Monitoring (RECOMMENDED)

The Building Block must implement comprehensive performance monitoring activities, starting from the initiation of service requests to the completion of transactions. It should continuously track key performance metrics such as response times, resource utilization, and throughput across all stages of the process. In case of any performance degradation or anomalies (due to both technical and operational reasons), the system should trigger alerts and automatically initiate corrective actions to maintain optimal performance levels. This proactive approach ensures the stability and reliability of the application, safeguarding the user experience and system integrity.
