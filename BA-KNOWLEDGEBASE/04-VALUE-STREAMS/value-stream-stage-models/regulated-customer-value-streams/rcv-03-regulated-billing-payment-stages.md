# RCV-03: Regulated Billing & Payment - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Regulated Billing & Payment value stream
**Parent Value Stream:** RCV-03 Regulated Billing & Payment
**Triggering Stakeholder:** Quantum Energy (monthly billing cycle)
**Receiving Stakeholder:** Active Regulated Customer
**Value Proposition:** Accurate, understandable regulated utility bills with convenient payment options and fair collection practices.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Regulated Billing & Payment value stream (RCV-03). This is a core utility process that covers the end-to-end cycle from collecting meter data to calculating bills, receiving customer payments, and managing revenue. Its accuracy, timeliness, and transparency are fundamental to the company's financial health and the customer experience.

---

## 1. Value Stream Context

**Value Stream ID:** RCV-03
**Name:** Regulated Billing & Payment
**Description:** Calculate consumption-based charges, deliver bills, collect payments, and manage accounts receivable for core regulated utility services.

**Entry Criteria:**
-   A billing cycle is initiated for a group of regulated customer accounts.
-   Validated meter read or interval data is available for the billing period.
-   Approved regulated tariff rates are loaded and effective in the billing system.

**Exit Criteria:**
-   An accurate regulated utility bill is calculated and successfully delivered to the customer.
-   Customer payment is received and applied correctly to the account.
-   The account balance is reconciled.
-   Any necessary collections activities for the cycle are completed or initiated.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **RCV-03.1** | **Meter Data Acquisition & Validation** | Collect consumption data from meters (manual, AMR, AMI) and validate it for completeness and accuracy, estimating where necessary. | *   9.2 Meter Data Collection & Management | Meter read schedules, Raw meter data | Validated consumption data (VEE) | Meter Read Success Rate, Data estimation rate |
| | | | *   9.3 Meter Data Validation, Estimating & Editing (VEE) | | | |
| **RCV-03.2** | **Rate Application & Bill Calculation** | Apply the appropriate regulated tariff rates, riders, and taxes to the validated consumption data to calculate the total bill amount for each customer. | *   4.3 Rate & Tariff Management | Validated consumption data, Approved rates | Calculated bill charges | Bill calculation error rate, Rerate volume |
| | | | *   4.2 Bill Calculation | | | |
| **RCV-03.3** | **Bill Generation & Presentment** | Generate the final bill statement in the required format (print or electronic) and present it to the customer through their preferred delivery channel. | *   4.2 Bill Calculation | Calculated bill charges, Customer preferences | Rendered bill image, Delivered bill (mail/email) | On-time bill delivery, e-bill adoption rate |
| **RCV-03.4** | **Payment Processing** | Receive customer payments from all available channels (e.g., mail, web, auto-pay, third-party) and apply them accurately to the correct customer accounts. | *   4.4 Payment Processing & Management | Customer payments, Remittance information | Posted payments, Updated account balances | Payment processing time, Exception handling rate |
| **RCV-03.5** | **Account Reconciliation & Aging** | Reconcile payments against billed amounts, manage account balances, and age outstanding receivables to identify delinquent accounts. | *   4.5 Credit & Collections Management | Posted payments, Billed amounts | Aged receivables report, Reconciled accounts | Days Sales Outstanding (DSO), Bad debt expense |
| **RCV-03.6** | **Collections Management** | Manage delinquent accounts according to regulatory rules, including issuing notices, making payment arrangements, and initiating service disconnection if necessary. | *   4.5 Credit & Collections Management | Delinquent account list, Regulatory rules | Payment arrangements, Collection notices, Disconnection orders | Collection rate, Roll-rate to write-off |

---

## 3. Cross-Value Stream Dependencies

*   **RCV-03** is the primary source of inquiries for **RCV-02 Regulated Customer Service Delivery**.
*   It relies on accurate data from **AOV-04 Electric Energy Delivery** and **AOV-05 Natural Gas Delivery** via their shared **Metering & Measurement** capability.
*   Failure to collect payment may trigger **RCV-05 Regulated Service Disconnection & Reconnection**.
*   The rates and charges are determined by the outcomes of **REV-01 Rate Case & Cost Recovery**.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Finance Leadership, Customer Operations, Regulatory Affairs, BA Working Group
**Approval:** Chief Financial Officer (CFO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for RCV-03.

**Next Review:** Annually or upon major changes in billing systems or rate structures.

---

**End of Document**
