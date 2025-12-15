# RCV-02: Regulated Customer Service Delivery - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Regulated Customer Service Delivery value stream
**Parent Value Stream:** RCV-02 Regulated Customer Service Delivery
**Triggering Stakeholder:** Active Regulated Customer
**Receiving Stakeholder:** Active Regulated Customer
**Value Proposition:** Timely, accurate, and helpful resolution of regulated utility service needs through convenient and compliant channels.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Regulated Customer Service Delivery value stream (RCV-02). This process covers how Quantum Energy responds to and resolves all forms of inbound customer inquiries, requests, and issues related to their core regulated utility service. Efficiently executing this value stream is critical for customer satisfaction, regulatory compliance, and operational efficiency.

---

## 1. Value Stream Context

**Value Stream ID:** RCV-02
**Name:** Regulated Customer Service Delivery
**Description:** Respond to customer inquiries, requests, and issues regarding core utility services (electric or gas) across all touchpoints.

**Entry Criteria:**
-   An active regulated customer initiates contact (e.g., call, email, web form, in-person).
-   The customer has an active regulated account or a specific service-related need.

**Exit Criteria:**
-   The customer's inquiry is fully resolved or their request has been fulfilled.
-   Customer satisfaction with the resolution is confirmed.
-   The interaction and any resulting transactions are documented in the customer information system.
-   Any required follow-up actions are completed or scheduled.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **RCV-02.1** | **Contact Initiation & Authentication** | Receive the customer contact through any channel (phone, web, etc.) and securely authenticate their identity to protect account information. | *   1.1 Customer Relationship Management | Customer contact, Account identifiers | Authenticated customer session, Service request type | Average Handle Time, Channel-specific volume |
| **RCV-02.2** | **Inquiry Triage & Routing** | Understand and classify the nature of the customer's inquiry or request and route it to the appropriate agent, specialist team, or self-service module. | *   1.2 Contact Center Management | Authenticated session, Request type | Routed inquiry, Case created | First Contact Resolution Rate, Transfer Rate |
| **RCV-02.3** | **Information Gathering & Analysis** | Access relevant customer, billing, and operational data to diagnose the issue or understand the context of the request. | *   1.1 Customer Relationship Management | Case details, Customer account data | Diagnosed issue, Contextual data summary | Agent data access time, Information accuracy |
| | | | *   9.2 Meter Data Collection & Management | | | |
| **RCV-02.4** | **Resolution & Fulfillment** | Provide the answer, execute the required transaction (e.g., payment plan), or dispatch a field resource to resolve the customer's need. | *   1.3 Customer Service Fulfillment | Diagnosed issue, Resolution options | Executed transaction, Service order, Customer answer | Resolution time, Service order accuracy |
| | | | *   10.2 Field Service & Work Management | | | |
| **RCV-02.5** | **Confirmation & Closure** | Clearly communicate the resolution to the customer, confirm their understanding and satisfaction, and formally close the inquiry or request. | *   1.1 Customer Relationship Management | Resolution details | Customer confirmation, Closed case | Customer Satisfaction (CSAT), Net Promoter Score (NPS) |
| **RCV-02.6** | **Documentation & Follow-up** | Record all interaction details, transactions, and outcomes in the system of record. Initiate any necessary follow-up actions or communications. | *   1.1 Customer Relationship Management | Closed case details | Documented interaction, Follow-up tasks | Documentation compliance, Follow-up completion rate |

---

## 3. Cross-Value Stream Dependencies

*   **RCV-02** is the primary interaction point for issues arising from **RCV-03 Regulated Billing & Payment**.
*   It often triggers work in **AOV-03 Work & Outage Management** (e.g., service calls).
*   Relies on data from **AOV-04 Electric Energy Delivery** and **AOV-05 Natural Gas Delivery** to diagnose service issues.
*   Poor performance in this value stream can lead to escalations that trigger **REV-02 Regulatory Compliance & Reporting** (e.g., official complaints).

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Customer Operations Leadership, Regulatory Affairs, BA Working Group
**Approval:** Chief Customer Officer
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for RCV-02.

**Next Review:** Annually or upon significant changes to customer service processes.

---

**End of Document**
