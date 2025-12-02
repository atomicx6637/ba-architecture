# SMV-03: Distributed Energy Resource (DER) Aggregation & Optimization - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the DER Aggregation & Optimization value stream
**Parent Value Stream:** SMV-03 Distributed Energy Resource (DER) Aggregation & Optimization
**Triggering Stakeholder:** Grid Operator / Market Operator / Portfolio Manager
**Receiving Stakeholder:** The Grid / DER Owners
**Value Proposition:** Enhanced grid reliability and resilience, reduced system costs, and new revenue streams from DER participation in wholesale markets or provision of ancillary services.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Distributed Energy Resource (DER) Aggregation & Optimization value stream (SMV-03). This modern and complex value stream describes how Quantum Energy enrolls, groups (aggregates), and controls a fleet of customer-sited and utility-sited DERs (like batteries, smart thermostats, and EV chargers) to act as a single "Virtual Power Plant" (VPP). This VPP can then be used to provide valuable services to the grid or to bid into wholesale energy markets.

---

## 1. Value Stream Context

**Value Stream ID:** SMV-03
**Name:** Distributed Energy Resource (DER) Aggregation & Optimization
**Description:** Aggregate, optimize, and manage a portfolio of regulated and non-regulated DERs to provide grid services and market opportunities.

**Entry Criteria:**
-   A portfolio of DERs (e.g., from customer programs or non-regulated sales) is available and contractually permitted for aggregation.
-   Grid service needs (e.g., peak shaving, frequency regulation) or wholesale market products for DERs are identified.
-   A DER Management System (DERMS) platform is in place.

**Exit Criteria:**
-   The aggregated DER portfolio (VPP) is effectively dispatched to provide a grid service or participate in the market.
-   Grid services are successfully delivered, or market revenues are captured.
-   Value (e.g., incentives, shared revenue) is shared back with DER owners as per their agreements.
-   The performance of the VPP is measured and verified.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **SMV-03.1** | **DER Enrollment & Onboarding** | Enroll customer-sited DERs into specific programs that allow for aggregation and dispatch. Onboard the physical devices onto the DERMS platform. | *   1.1 Customer Relationship Management | Customer DER program enrollment | Registered DER assets in DERMS, Customer consent | DER onboarding cycle time, Portfolio MW growth |
| **SMV-03.2** | **VPP Forecasting & Capability Assessment** | Forecast the available capacity and operational characteristics of the aggregated DER portfolio (the VPP) for a given timeframe, considering device status and customer constraints. | *   13.7 DER Management System (DERMS) Operations | DER asset data, Customer constraints, Weather data | VPP capacity forecast, Availability reports | VPP forecast accuracy (MW), Available vs. enrolled capacity |
| **SMV-03.3** | **Grid Service & Market Opportunity Analysis** | Identify opportunities to use the VPP to solve grid needs (e.g., defer a T&D investment, reduce peak load) or to bid the VPP into wholesale markets as a resource. | *   11.1 Load & Resource Forecasting | VPP capacity forecast, Grid needs, Market prices | Grid service use case, Market bid strategy | Value of identified opportunities ($), Bid-to-win ratio |
| **SMV-03.4** | **VPP Optimization & Bid/Offer Submission** | Run optimization algorithms to determine the most economic and reliable way to use the VPP to meet an opportunity. Submit bids/offers to the market or schedule the VPP for a grid service. | *   13.7 DER Management System (DERMS) Operations | VPP use case, VPP forecast | Optimal dispatch plan, Market bids/offers | Optimization speed, Bid value |
| **SMV-03.5** | **VPP Dispatch & Real-Time Control** | Upon market award or grid service trigger, send automated control signals to the fleet of individual DERs to perform the required action (e.g., charge, discharge, reduce load). | *   13.7 DER Management System (DERMS) Operations | Market award, Dispatch trigger | Real-time DER control signals, VPP telemetry | Dispatch accuracy (actual vs. scheduled), Signal latency |
| **SMV-03.6** | **Performance Measurement & Settlement** | Measure and verify the actual performance of the VPP against the dispatched schedule or market award. Settle transactions with the market operator and/or calculate performance for internal grid service value. | *   9.2 Meter Data Collection & Management | VPP telemetry, Market settlement data | VPP performance report, Settled market transactions | Performance accuracy factor, Settlement value |
| **SMV-03.7** | **Value Distribution & Reporting** | Distribute incentives or revenue shares to the DER owners based on their contribution and program agreements. Report on VPP performance and value created. | *   4.2 Bill Calculation | VPP performance data, Customer agreements | Customer incentives/payments, Performance dashboards | On-time customer payment, Report accuracy |

---

## 3. Cross-Value Stream Dependencies

*   This value stream is heavily dependent on **RCV-04 Regulated Customer Program Participation** and the various non-regulated value streams (**NCV-01, 02, 03**) to create the underlying portfolio of DER assets.
*   It acts as a new type of supply resource for **AOV-04 Electric Energy Delivery** and **AOV-06 System Reliability & Emergency Response**.
*   It represents a new form of market interaction, related to but distinct from traditional **SMV-01 Electric Energy Supply & Trading**.
*   The rules for DER participation in markets are often governed by regulations managed in **REV-02 Regulatory Compliance & Reporting**.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Grid Modernization Leadership, Energy Trading, Customer Programs, BA Working Group
**Approval:** Chief Technology Officer (CTO) / Chief Strategy Officer
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for SMV-03.

**Next Review:** Annually or upon significant changes in DER technology or market rules.

---

**End of Document**
