# AVS-05: Natural Gas Delivery - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Natural Gas Delivery operational value stream
**Parent Value Stream:** AVS-05 Natural Gas Delivery
**Triggering Stakeholder:** Gas Customer (gas consumption)
**Receiving Stakeholder:** Gas Customer
**Value Proposition:** Continuous, safe natural gas delivery at required pressure with odorization and quality specifications met.
**Related Documents:**
*   [Enterprise Value Streams Catalog (ent-value-streams-catalog.md)](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Natural Gas Delivery value stream (AVS-05) for Quantum Energy. This value stream describes the end-to-end process of transporting natural gas from supply points through the transmission and distribution systems to customer meters, ensuring reliable pressure, safety, and gas quality. A clear understanding of these stages is crucial for maintaining system integrity, ensuring public safety, and providing reliable service to all gas customers.

---

## 1. Value Stream Context

**Value Stream ID:** AVS-05
**Name:** Natural Gas Delivery
**Description:** The complete cycle of delivering natural gas from city gate stations through the high-pressure transmission and lower-pressure distribution pipeline systems to the end-use customer's meter. This includes managing system pressure, ensuring gas quality and odorization, and balancing supply with real-time demand.

**Entry Criteria:**
-   Gas customer is connected and actively consuming gas.
-   Natural gas supply is procured and available at city gate stations.
-   The gas transmission and distribution pipeline systems are operational and safe.

**Exit Criteria:**
-   Natural gas is delivered to the customer's meter at the correct pressure.
-   System integrity and safety are maintained without interruption.
-   Gas pressure and quality specifications are continuously met.
-   Revenue metering accurately records gas volume consumed.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **AVS-05.1** | **Demand Forecasting & Supply Planning** | Forecast daily and intra-day gas demand based on weather and customer usage patterns. Plan supply nominations to meet this demand. | *   3.2 Gas Demand Forecasting | Weather forecasts, Historical consumption data | Gas demand forecast, Supply nomination plan | Forecast accuracy, Supply plan accuracy |
| | | | *   3.1 Gas Supply & Capacity Planning | | | |
| **AVS-05.2** | **Supply Scheduling & Balancing** | Schedule the flow of gas from suppliers and pipelines into the local distribution system. Balance nominations with actual receipts to ensure supply matches demand. | *   3.3 Gas Scheduling & Nominations | Supply contracts, Demand forecast | Daily gas schedules, Balanced supply portfolio | Balancing penalties, Schedule accuracy |
| | | | *   13.4 Gas System Balancing | | | |
| **AVS-05.3** | **Transmission System Operation** | Manage the flow and pressure of gas within the high-pressure transmission pipelines that act as the backbone of the delivery system. | *   6.1 Gas Transmission System Operations | System pressure data, Supply receipts | Stable transmission pressure, Gas flow to distribution | Transmission pressure variance, Throughput |
| | | | *   13.5 Switching & Clearance Coordination | | | |
| **AVS-05.4** | **Distribution System Pressure Management** | Operate and regulate pressure from the transmission system into the lower-pressure distribution network that directly serves neighborhoods and customers. | *   10.1 Gas Distribution System Operations & Control | Distribution pressure sensor data, Demand changes | Regulated distribution pressure, Safe operating conditions | Pressure compliance, Leak detection rate |
| | | | *   10.3 Gas Leak Survey & Repair | | | |
| **AVS-05.5** | **Real-Time Monitoring & Control** | Continuously monitor system pressures, flow rates, and equipment status via SCADA. Make control adjustments to maintain system integrity and respond to events. | *   13.2 Real-Time System Monitoring & Analysis | SCADA data, Alarm notifications | Real-time system view, Control commands | System availability, Alarm response time |
| | | | *   13.4 Gas System Balancing | | | |
| **AVS-05.6** | **Odorization & Quality Control** | Inject odorant into the gas stream for safety and public awareness. Monitor gas composition and quality to ensure it meets tariff specifications. | *   10.1 Gas Distribution System Operations & Control | Odorant levels, Gas samples | Odorized gas, Gas quality reports | Odorant concentration, BTU content |
| | | | *   10.4 Gas Quality & Odorization | | | |
| **AVS-05.7** | **Volume Accounting & Settlement** | Measure and record gas volumes at city gates and customer meters. Reconcile transported volumes and provide corrected data for billing. | *   Metering and Measurement (L1) | Meter data (volume), Temperature/pressure data | Corrected volume data, Settlement reports | Unaccounted-for gas (UAG), Meter accuracy |
| | | | *   9.2 Meter Data Collection & Management (L2) | | | |
| | | | *   14.2 General Accounting & Reporting (L2) | | | |

---

## 3. Cross-Value Stream Dependencies

*   **AVS-05 Natural Gas Delivery** is directly enabled by **SVS-02 Natural Gas Supply** for procuring the necessary commodity.
*   It is fundamental for **RCV-02 Regulated Customer Service Delivery** and **RCV-03 Regulated Billing & Payment** for gas customers.
*   System safety and reliability are enhanced by **AVS-06 System Reliability & Emergency Response**.
*   This value stream is crucial for providing the foundational service that supports non-regulated offerings that may use natural gas.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Regulated Operations Leadership, Gas Control Leadership, BA Working Group
**Approval:** Chief Operations Officer (COO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for AVS-05 Natural Gas Delivery.

**Next Review:** Annually or upon significant changes to gas system operations.

---

**End of Document**
