# SMV-02: Natural Gas Supply & Trading - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Natural Gas Supply & Trading value stream
**Parent Value Stream:** SMV-02 Natural Gas Supply & Trading
**Triggering Stakeholder:** Gas Supply Manager / Portfolio Manager
**Receiving Stakeholder:** The Gas System / Gas Customers
**Value Proposition:** Reliable, cost-effective gas supply with seasonal flexibility and risk mitigation, optimizing market returns within risk parameters.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Natural Gas Supply & Trading value stream (SMV-02). This process describes how Quantum Energy ensures a reliable and cost-effective supply of natural gas for its customers. It involves forecasting demand, buying gas from producers, contracting for pipeline transportation and storage, and managing the associated price risks.

---

## 1. Value Stream Context

**Value Stream ID:** SMV-02
**Name:** Natural Gas Supply & Trading
**Description:** Procure natural gas supply through commodity purchases, transportation contracts, and storage management to meet system and customer requirements, optimizing wholesale market exposure.

**Entry Criteria:**
-   A gas demand forecast for the planning horizon (daily, monthly, seasonal) is available.
-   The gas supply portfolio strategy and hedging policy are defined.
-   Quantum Energy has established credit and contracts to purchase gas and transport it on interstate pipelines.

**Exit Criteria:**
-   Sufficient physical gas supply is secured and scheduled to meet customer demand for the planning horizon.
-   The all-in cost of gas (commodity, transport, storage) is optimized and prudent.
-   Price risk is managed within approved tolerance levels.
-   All transactions are settled, and costs are tracked for regulatory recovery.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **SMV-02.1** | **Demand Forecasting & Supply Strategy** | Develop short and long-term forecasts for gas demand, considering weather and economic factors. Define the strategy for procuring supply (e.g., baseload vs. spot purchases). | *   3.2 Gas Demand Forecasting | Weather forecasts, Historical demand | Gas demand forecast, Supply plan | Forecast accuracy (e.g., BCF vs. actual) |
| **SMV-02.2** | **Commodity Procurement & Trading** | Purchase physical gas from producers or on trading hubs for various timeframes (next-day, monthly). Execute financial hedges (e.g., futures, swaps) to manage price risk. | *   11.2 Energy Trading & Hedging | Supply plan, Market prices | Executed gas purchases, Hedges | Weighted Average Cost of Gas (WACOG), Hedge effectiveness |
| **SMV-02.3** | **Transportation & Storage Contracting** | Contract for firm and interruptible transportation capacity on interstate pipelines to move gas from supply basins to the city gate. Contract for storage capacity to manage seasonal demand swings. | *   3.1 Gas Supply & Capacity Planning | Supply plan, Pipeline tariffs | Executed transport/storage contracts | Pipeline/storage capacity utilization, Cost per MMBtu transported |
| **SMV-02.4** | **Pipeline Scheduling & Nomination** | On a daily basis, nominate the volume of gas to be transported on each pipeline from specific receipt points to specific delivery points (city gates). | *   3.3 Gas Scheduling & Nominations | Daily demand forecast, Purchased volumes, Pipeline contracts | Daily gas nominations | Nomination accuracy, Imbalance penalties |
| **SMV-02.5** | **Intra-day Balancing & Optimization** | Monitor real-time system demand versus scheduled supply. Make intra-day adjustments by buying/selling on spot markets or utilizing storage to keep the system in balance. | *   13.4 Gas System Balancing | Real-time demand, Scheduled supply | Intra-day trades, Balancing actions | Daily imbalance volume/cost |
| **SMV-02.6** | **Transaction Settlement & Reconciliation** | Validate and settle all commodity, transport, and storage invoices. Resolve any discrepancies and ensure accurate financial accounting for all costs. | *   11.4 Contract & Transaction Management | Supplier invoices, Pipeline statements | Settled transactions, Paid invoices | Settlement dispute rate, On-time payment |
| **SMV-02.7** | **Purchased Gas Adjustment (PGA) Filing** | Aggregate all prudent gas supply costs and prepare regulatory filings (e.g., PGA) to pass these costs through to customers via regulated rates. | *   14.6 Regulatory Strategy & Management | Settled gas costs | Regulatory filings (PGA), Prudence reviews | Recovered cost percentage, True-up amounts |

---

## 3. Cross-Value Stream Dependencies

*   **SMV-02** provides the gas commodity that is delivered to customers via **AOV-05 Natural Gas Delivery**.
*   The costs incurred are recovered through customer bills in **RCV-03 Regulated Billing & Payment**.
*   The pass-through mechanism (PGA) is a specific type of filing related to the broader **REV-01 Rate Case & Cost Recovery** value stream.
*   This process must align with **ESV-05 Enterprise Risk Management** policies.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Gas Supply & Trading Leadership, Finance, Regulatory, BA Working Group
**Approval:** Chief Financial Officer (CFO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for SMV-02.

**Next Review:** Annually or upon significant changes in gas markets or regulations.

---

**End of Document**
