# RCV-05: Regulated Service Disconnection & Reconnection - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Regulated Service Disconnection & Reconnection value stream
**Parent Value Stream:** RCV-05 Regulated Service Disconnection & Reconnection
**Triggering Stakeholder:** Quantum Energy (non-payment) or Regulated Customer (voluntary)
**Receiving Stakeholder:** Regulated Customer
**Value Proposition:** Fair collection practices with clear path to regulated service restoration, while protecting utility revenue and ensuring safety.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Regulated Service Disconnection & Reconnection value stream (RCV-05). This process handles the sensitive and highly regulated activities of stopping utility service, typically for non-payment, and subsequently restoring it. Executing this value stream requires strict adherence to regulatory rules, a focus on customer communication, and efficient field operations to ensure safety and fairness.

---

## 1. Value Stream Context

**Value Stream ID:** RCV-05
**Name:** Regulated Service Disconnection & Reconnection
**Description:** Manage service disconnection for non-payment or customer request, and restore core utility service when conditions are met, adhering to regulatory rules.

**Entry Criteria:**
-   A customer account meets the specific, regulated criteria for disconnection for non-payment (e.g., past due amount, time elapsed).
-   All legally required notices and waiting periods have been completed.
-   A customer submits a voluntary request to disconnect service.

**Exit Criteria:**
-   Regulated utility service is physically or remotely disconnected/reconnected.
-   The customer's account status is updated to reflect the change.
-   The customer is notified of the status change.
-   All required field work and regulatory reporting are completed.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **RCV-05.1** | **Disconnection Determination & Notification** | Identify accounts eligible for disconnection based on collections aging. Generate and send all legally mandated disconnection notices to the customer. | *   4.5 Credit & Collections Management | Aged receivables data, Regulatory rules | Disconnection candidate list, Sent notices | Notice accuracy, Number of eligible accounts |
| **RCV-05.2** | **Pre-Disconnection Mitigation** | Actively attempt to contact the customer before disconnection to offer payment arrangements or assistance, preventing unnecessary service interruptions. | *   1.2 Contact Center Management | Disconnection candidate list | Completed payment plans, Customer contacts | Disconnections avoided, Successful arrangements |
| | | | *   4.5 Credit & Collections Management | | | |
| **RCV-05.3** | **Field Disconnection Order & Execution** | If payment is not received, issue a service order and dispatch a field technician (or send a remote command) to safely disconnect the customer's service. | *   10.2 Field Service & Work Management | Disconnection order | Executed disconnection, Updated account status | On-time execution, Field safety incidents |
| | | | *   9.4 Remote Service Switching | | | |
| **RCV-05.4** | **Payment & Reconnection Request** | The customer makes the required payment or arrangement. The system receives this payment and automatically or manually triggers a reconnection request. | *   4.4 Payment Processing & Management | Customer payment, Account status | Reconnection request, Paid balance | Time from payment to request, Payment accuracy |
| **RCV-05.5** | **Field Reconnection Order & Execution** | Issue a service order and dispatch a field technician (or send a remote command) to safely restore the customer's service. | *   10.2 Field Service & Work Management | Reconnection order | Restored service, Updated account status | Time to reconnect, Reconnection success rate |
| | | | *   9.4 Remote Service Switching | | | |
| **RCV-05.6** | **Account Finalization & Reporting** | Update the customer's account to reflect the restored service, apply any relevant fees, and complete any required regulatory reporting on disconnection/reconnection activities. | *   4.2 Bill Calculation | Service restoration confirmation | Finalized account, Regulatory reports | Fee accuracy, Reporting timeliness |
| | | | *   14.6 Regulatory Strategy & Management | | | |

---

## 3. Cross-Value Stream Dependencies

*   **RCV-05** is the final stage of the collections process within **RCV-03 Regulated Billing & Payment**.
*   Interactions with the customer during this process are handled by **RCV-02 Regulated Customer Service Delivery**.
*   The physical work is performed as part of **AOV-03 Work & Outage Management**.
*   The entire process is heavily governed by rules defined in partnership with **REV-02 Regulatory Compliance & Reporting**.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Customer Operations, Finance, Regulatory Affairs, BA Working Group
**Approval:** Chief Customer Officer / Chief Financial Officer
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for RCV-05.

**Next Review:** Annually or upon changes to collections or disconnection regulations.

---

**End of Document**
