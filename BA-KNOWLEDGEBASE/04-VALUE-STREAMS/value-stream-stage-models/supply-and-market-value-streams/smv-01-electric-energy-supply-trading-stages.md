# SMV-01: Electric Energy Supply & Trading - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Electric Energy Supply & Trading value stream
**Parent Value Stream:** SMV-01 Electric Energy Supply & Trading
**Triggering Stakeholder:** Load Serving Entity / Portfolio Manager
**Receiving Stakeholder:** The Grid / Electric Customers
**Value Proposition:** Adequate, reliable, and cost-effective electric supply to meet all load obligations with appropriate reserves, optimizing market returns within risk parameters.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Electric Energy Supply & Trading value stream (SMV-01). This complex process describes how Quantum Energy forecasts electric demand, optimizes its own generation assets, and interacts with wholesale energy markets to ensure a reliable and cost-effective power supply for its regulated customers. It is a critical function that sits at the intersection of grid operations, risk management, and finance.

---

## 1. Value Stream Context

**Value Stream ID:** SMV-01
**Name:** Electric Energy Supply & Trading
**Description:** Secure electrical energy supply through owned generation, market purchases, and contracts to meet load obligations, reserve requirements, and manage wholesale market exposure.

**Entry Criteria:**
-   A load forecast for the planning horizon is available.
-   The enterprise supply portfolio strategy and risk tolerances are defined.
-   Quantum Energy has established credit and access to participate in wholesale energy markets (ISOs/RTOs).

**Exit Criteria:**
-   Sufficient energy and ancillary services are secured to meet the load obligation plus reserve margins.
-   The cost of the resulting supply portfolio is optimized and deemed prudent.
-   Market risk exposure (e.g., price, volume) is within established tolerance bands.
-   All transactions are settled, and costs are tracked for regulatory recovery.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **SMV-01.1** | **Load Forecasting & Portfolio Strategy** | Develop short, medium, and long-term electric load forecasts. Define the overall portfolio strategy for meeting this load (e.g., mix of owned generation vs. market purchases). | *   11.1 Load & Resource Forecasting | Historical load data, Economic forecasts | Load forecast, Portfolio plan | Forecast accuracy (MAPE), Portfolio diversification |
| **SMV-01.2** | **Generation Fleet Bidding & Dispatch** | Develop and submit bids into the wholesale market for the company's own generation assets. Economically dispatch these assets based on market awards and system needs. | *   5.4 Generation Scheduling & Dispatch | Asset availability, Fuel costs, Market rules | Generation bids, Dispatch schedules | Plant profitability, Bid accuracy |
| **SMV-01.3** | **Wholesale Market Trading (Day-Ahead/Real-Time)** | Transact in the day-ahead and real-time energy markets to balance the portfolio, acquiring supply to cover load or selling excess generation. | *   11.2 Energy Trading & Hedging | Portfolio position, Market prices | Executed trades, Updated position | Trading profit & loss (P&L), Market capture rate |
| **SMV-01.4** | **Bilateral Contract Management** | Manage long-term bilateral contracts (e.g., Power Purchase Agreements - PPAs) for energy, ensuring counterparties meet their obligations and contracts are optimized. | *   11.4 Contract & Transaction Management | Bilateral contracts | Contract nominations, Performance tracking | Counterparty risk exposure, PPA value |
| **SMV-01.5** | **Position & Risk Management** | Consolidate the overall supply portfolio position (generation, trades, contracts) and assess the financial and operational risk against established limits (e.g., VaR, Stop-Loss). | *   11.3 Portfolio & Risk Management | Consolidated position, Market volatility data | Risk exposure reports, Hedge recommendations | Value at Risk (VaR), Position exposure |
| **SMV-01.6** | **Market Settlement & Reconciliation** | Validate and settle all wholesale market transactions with the ISO/RTO. Reconcile invoices and ensure accurate financial accounting for all supply costs. | *   11.4 Contract & Transaction Management | ISO/RTO settlement statements, Trade blotters | Settled transactions, Reconciled invoices | Settlement dispute rate, On-time payment |
| **SMV-01.7** | **Regulatory Cost Recovery & Reporting** | Aggregate all prudent supply costs and prepare testimony and filings to have these costs recovered through regulated customer rates. | *   14.6 Regulatory Strategy & Management | Settled supply costs | Regulatory filings, Prudence reviews | Recovered cost percentage, Regulatory lag |

---

## 3. Cross-Value Stream Dependencies

*   **SMV-01** provides the energy that is delivered via **AOV-04 Electric Energy Delivery**.
*   It is the primary mechanism for managing financial risk for the commodity portion of the customer's bill, which is charged in **RCV-03 Regulated Billing & Payment**.
*   The costs incurred in this value stream are a major component of what is recovered in **REV-01 Rate Case & Cost Recovery**.
*   It works in close coordination with **SMV-03 DER Aggregation & Optimization** as DERs become a supply-side resource.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Energy Trading & Risk Management Leadership, Generation, Finance, BA Working Group
**Approval:** Chief Financial Officer (CFO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for SMV-01.

**Next Review:** Annually or upon significant changes in market rules or supply strategy.

---

**End of Document**
