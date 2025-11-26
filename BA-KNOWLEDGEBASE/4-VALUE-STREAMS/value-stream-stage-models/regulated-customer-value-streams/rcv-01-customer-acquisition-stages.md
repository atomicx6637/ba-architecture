# RCV-01: Regulated Customer Acquisition - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Detailed stages for the Regulated Customer Acquisition value stream
**Parent Value Stream:** RCV-01 Regulated Customer Acquisition
**Triggering Stakeholder:** Prospective Regulated Customer
**Receiving Stakeholder:** New Regulated Customer
**Value Proposition:** Seamless transition to reliable electric or natural gas service with clear pricing, terms, and service expectations.
**Related Documents:**
*   [Enterprise Value Streams Catalog (ent-value-streams-catalog.md)](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Regulated Customer Acquisition value stream (RCV-01) for Quantum Energy. This value stream outlines the end-to-end process of attracting, onboarding, and activating new customers for core regulated utility services (electric or gas). Understanding these stages is critical for optimizing customer experience, ensuring compliance, and streamlining operational efficiency.

---

## 1. Value Stream Context

**Value Stream ID:** RCV-01
**Name:** Regulated Customer Acquisition
**Description:** The process by which Quantum Energy identifies, qualifies, enrolls, and connects new customers to its regulated electric or natural gas services. It encompasses the customer's initial inquiry through to the point of active service and first billing.

**Entry Criteria:**
-   Customer expresses interest in regulated electric or gas service.
-   Premise is within Quantum Energy's regulated service territory.
-   Customer contact information is available.

**Exit Criteria:**
-   Customer account is established and active in billing system.
-   Electric or gas service is connected at the premise.
-   Customer receives initial welcome communication.
-   First bill is successfully generated.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **RCV-01.1** | **Customer Inquiry & Qualification** | Customer contacts Quantum Energy to inquire about new service. Information is gathered to determine eligibility and service needs. | *   10.1 Customer Contact & Interaction Management | Customer contact info, Service address | Service eligibility confirmed, Service options presented | Call abandon rate, Digital inquiry rate |
| | | | *   10.2 Customer Account Management | | | First Contact Resolution |
| | | | *   12.1 Market Research & Analysis (if segment specific) | | | |
| **RCV-01.2** | **Credit Assessment & Account Setup** | Quantum Energy assesses customer creditworthiness and establishes a new account in the billing system, including deposit determination if necessary. | *   14.2 General Accounting & Reporting (Credit) | Customer personal data, Service details | Credit decision, Account ID, Deposit requirement | Deposit collection rate, Account setup accuracy |
| | | | *   10.2 Customer Account Management | | | |
| | | | *   18.1 Legal Advisory & Counsel (Privacy) | | | |
| **RCV-01.3** | **Service Connection Planning** | Schedule the physical connection of service and coordinate necessary field activities (e.g., meter set, turn-on). | *   8.3 Service Connections & Installations (Reg) | Account details, Service address, Service type | Work order created, Appointment scheduled | Appointment adherence, Work order creation time |
| | | | *   9.3 Service Connections & Installations (Reg) | | | |
| | | | *   13.5 Switching & Clearance Coordination (for electric) | | | |
| **RCV-01.4** | **Physical Service Installation/Turn-On** | Field crews perform the necessary physical work to connect or turn on electric or natural gas service at the customer's premise. | *   8.3 Service Connections & Installations (Reg) | Work order, Equipment, Safety protocols | Service physically connected/turned on, Field notes | Installation completion rate, Safety incidents |
| | | | *   9.3 Service Connections & Installations (Reg) | | | |
| | | | *   15.5 Compensation & Benefits (Field Staff) | | | |
| **RCV-01.5** | **Meter Installation & Activation** | Install and activate the appropriate electric or gas meter, ensuring it is properly provisioned and begins recording consumption data. | *   Metering and Measurement (L1) | Service connected confirmation, Meter asset info | Meter active, Data flow initiated | Meter read accuracy, Activation time |
| | | | *   9.1 Metering Infrastructure Management (L2) | | | |
| | | | *   9.2 Meter Data Collection & Management (L2) | | | |
| **RCV-01.6** | **Account Activation & Welcome** | Finalize account activation, send welcome communications, and provide customer with essential information about their new service. | *   10.2 Customer Account Management | Active meter data, Account details | Welcome package sent, Digital account enabled | First bill accuracy, Customer welcome survey |
| | | | *   10.6 Customer Communications & Notifications | | | |
| | | | *   4.1 Corporate Communications (Brand) | | | |
| **RCV-01.7** | **First Bill Delivery** | Generate and deliver the customer's first bill, ensuring accuracy and clarity for their initial charges. | *   Financial Management (L1) | Meter data, Account info, Tariff rates | First bill generated and delivered | First bill accuracy, Inquiry rate on first bill |
| | | | *   14.2 General Accounting & Reporting (L2) | | | |
| | | | *   10.6 Customer Communications & Notifications | | | |

---

## 3. Cross-Value Stream Dependencies

*   **RCV-01 Regulated Customer Acquisition** is a prerequisite for **RCV-02 Regulated Customer Service Delivery** and **RCV-03 Regulated Billing & Payment**.
*   It feeds into **RCV-04 Regulated Customer Program Participation** by establishing the customer base.
*   It is indirectly influenced by **REV-02 Regulatory Compliance & Reporting** (e.g., customer protection rules).
*   It can be a precursor to **NCV-01 Smart Home Solution Delivery** if a new utility customer is also a target for non-regulated offerings.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Customer Experience Leadership, Regulated Operations Leadership, BA Working Group
**Approval:** Chief Customer Officer (CCO)
**Version History:**
- v1.0 (2025-11-25): Initial detailed stage model for RCV-01 Regulated Customer Acquisition.

**Next Review:** Annually or upon significant changes to customer onboarding processes/regulations

---

**End of Document**
