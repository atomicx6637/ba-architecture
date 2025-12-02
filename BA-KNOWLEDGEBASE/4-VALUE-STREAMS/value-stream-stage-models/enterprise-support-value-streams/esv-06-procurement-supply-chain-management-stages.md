# ESV-06: Procurement & Supply Chain Management - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Procurement & Supply Chain Management value stream
**Parent Value Stream:** ESV-06 Procurement & Supply Chain Management
**Triggering Stakeholder:** Business Unit / Project Manager / Employee
**Receiving Stakeholder:** Business Unit / Project Manager / Employee
**Value Proposition:** Optimized costs, assured supply continuity, managed supplier risk, and efficient delivery of goods and services across the entire enterprise.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Procurement & Supply Chain Management value stream (ESV-06). Often called "Source-to-Pay," this value stream describes the end-to-end process of how Quantum Energy buys all goods and services needed to run the business. It covers everything from strategic sourcing and supplier selection to creating purchase orders, managing inventory, and paying supplier invoices.

---

## 1. Value Stream Context

**Value Stream ID:** ESV-06
**Name:** Procurement & Supply Chain Management
**Description:** Strategically source, procure, and manage suppliers, materials, and logistics to support all business operations, including regulated infrastructure maintenance and non-regulated product fulfillment.

**Entry Criteria:**
-   A need for goods or services is identified by a business unit or project.
-   A bill of materials for a capital project is finalized.
-   Inventory levels for a stocked item fall below a reorder point.

**Exit Criteria:**
-   The required goods or services are delivered to the business user on time and to specification.
-   The supplier's performance is managed effectively.
-   The supplier is paid accurately and on time.
-   The total cost of ownership is optimized and supply risk is managed.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **ESV-06.1** | **Spend Analysis & Sourcing Strategy** | Analyze enterprise-wide spend to identify opportunities for cost savings. Develop strategic sourcing plans for key commodity and service categories. | *   15.4 Sourcing & Procurement | Spend data, Business requirements | Spend analysis cube, Category sourcing plans | Spend under management (%), Identified savings opportunities ($) |
| **ESV-06.2** | **Supplier Identification & Qualification** | Identify, evaluate, and qualify potential suppliers based on their capabilities, financial stability, and risk profile. Manage the supplier master data. | *   15.4 Sourcing & Procurement | Sourcing plans, Supplier information | Qualified supplier list, Supplier risk scorecards | New qualified suppliers, Supplier diversity rate |
| **ESV-06.3** | **Strategic Sourcing & Contracting** | Execute strategic sourcing events (e.g., RFPs, auctions). Negotiate pricing, terms, and conditions, and put master agreements and contracts in place. | *   15.4 Sourcing & Procurement | RFP/RFQ, Supplier bids | Executed contracts, Negotiated savings | Realized savings vs. identified (%), Contract compliance |
| **ESV-06.4** | **Requisition & Purchase Order Processing (Procure-to-Pay)** | Process purchase requisitions from business users, convert them into purchase orders (POs), and send the POs to the selected suppliers. | *   15.4 Sourcing & Procurement | Purchase requisition | Approved purchase order | Requisition-to-PO cycle time, No-PO/No-Pay compliance |
| **ESV-06.5** | **Logistics & Inventory Management** | Manage the transportation and logistics for incoming materials. Receive goods into warehouses and manage inventory levels for key materials to ensure availability. | *   15.6 Logistics & Warehousing | Purchase order, Advance ship notice | Goods receipt, Updated inventory levels | Inventory turns, Stockout rate, On-time delivery |
| **ESV-06.6** | **Invoice Processing & Payment (Accounts Payable)** | Receive supplier invoices, match them against purchase orders and goods receipts (3-way match), resolve exceptions, and process payments to the supplier. | *   14.2 General Accounting & Reporting | Supplier invoice, Goods receipt | Paid invoice | Invoice processing cost, On-time payment percentage |
| **ESV-06.7** | **Supplier Performance & Relationship Management** | Monitor and manage supplier performance against contractual obligations. Conduct regular business reviews and build long-term, strategic relationships with key suppliers. | *   15.4 Sourcing & Procurement | Contract SLAs, Performance data | Supplier scorecards, Improvement plans | Supplier performance rating, Supplier satisfaction |

---

## 3. Cross-Value Stream Dependencies

*   **ESV-06** is a critical enabler for all value streams that consume goods and services, particularly asset-intensive streams like **AOV-02 Capital Project Delivery** and **AOV-03 Work & Outage Management**.
*   The "Pay" part of this process is a direct input to **ESV-03 Financial Management & Reporting** (Accounts Payable).
*   It works with **ESV-05 Enterprise Risk Management** to manage supply chain and third-party supplier risk.
*   For non-regulated value streams like **NCV-01**, this process is crucial for managing the cost of goods sold and ensuring product availability.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Procurement & Supply Chain Leadership, Finance, BA Working Group
**Approval:** Chief Procurement Officer (CPO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for ESV-06.

**Next Review:** Annually or upon a major change in supply chain strategy.

---

**End of Document**
