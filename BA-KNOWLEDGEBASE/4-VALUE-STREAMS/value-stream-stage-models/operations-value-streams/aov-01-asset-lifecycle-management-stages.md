# AOV-01: Asset Lifecycle Management - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Asset Lifecycle Management value stream
**Parent Value Stream:** AOV-01 Asset Lifecycle Management
**Triggering Stakeholder:** Asset Manager / Strategic Planner
**Receiving Stakeholder:** The Enterprise / Rate Payers
**Value Proposition:** Optimized asset performance, maximized asset life, minimized lifecycle costs, and maintained reliability and safety across all asset types.
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Asset Lifecycle Management value stream (AOV-01). This foundational value stream describes the end-to-end management of Quantum Energy's physical assets, from initial planning and acquisition through operation, maintenance, and eventual disposal. A disciplined approach to this process is critical for ensuring safety, reliability, and financial prudence across the company's vast infrastructure portfolio.

---

## 1. Value Stream Context

**Value Stream ID:** AOV-01
**Name:** Asset Lifecycle Management
**Description:** Plan, acquire, operate, maintain, and dispose of physical assets throughout their economic lifecycle to optimize reliability, performance, and cost for regulated utility infrastructure and non-regulated deployments.

**Entry Criteria:**
-   An asset need is identified based on strategy, load growth, or asset condition.
-   A business case for the asset investment is approved.
-   Funding for the asset is allocated in the capital or operational budget.

**Exit Criteria:**
-   The asset is delivering its expected performance and value.
-   The asset's costs are optimized across its entire lifecycle.
-   The asset is formally retired, decommissioned, and disposed of in a safe and compliant manner.
-   All knowledge related to the asset's life is captured.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **AOV-01.1** | **Asset Strategy & Planning** | Develop long-term strategies for asset families, forecast future needs, and create investment plans based on risk, condition, and performance. | *   12.1 Asset Investment Planning | Corporate strategy, Load forecasts, Asset health data | Asset investment plans, Long-term capital plans | Plan accuracy, Risk mitigation score |
| **AOV-01.2** | **Asset Acquisition & Commissioning** | Acquire or construct a new asset. This is the handoff to the **AOV-02 Capital Project Delivery** value stream. Once commissioned, the asset is handed back. | *   AOV-02 (Value Stream) | Approved asset plan, Business case | Commissioned asset, In-service documentation | On-time/budget delivery, Asset data registration |
| **AOV-01.3** | **Asset Operation & Monitoring** | Operate the asset to deliver its intended service. Continuously monitor its performance, condition, and utilization against established targets. | *   8.1 Distribution System Operations & Control | In-service asset, Operating procedures | Operational data, Performance metrics | Asset availability, Utilization rate, O&M cost |
| | | | *   5.1 Conventional Generation Operations | | | |
| **AOV-01.4** | **Asset Maintenance & Repair** | Plan and execute all maintenance activities, including preventative, predictive, and corrective (repair) work to ensure asset reliability and longevity. | *   12.3 Asset Maintenance & Work Management | Maintenance plans, Unplanned failure alerts | Completed work orders, Maintenance history | PM/CM ratio, Mean Time To Repair (MTTR) |
| **AOV-01.5** | **Asset Performance & Risk Assessment** | Analyze asset data to assess health, calculate risk of failure (PoF/CoF), and evaluate performance against financial and operational goals. | *   12.1 Asset Investment Planning | Operational data, Maintenance history, Failure data | Asset health indices, Risk scores, Performance reports | Asset Health Index, Remaining useful life |
| **AOV-01.6** | **Asset Renewal & Disposal Decision** | Based on risk, cost, and performance assessments, make the decision to continue maintaining, refurbish, replace, or decommission an asset. | *   12.1 Asset Investment Planning | Risk scores, Lifecycle cost analysis | Refurbish/replace/retire decision, Updated investment plan | Decision accuracy, NPV of decision |
| **AOV-01.7** | **Asset Decommissioning & Retirement** | Plan and execute the safe removal of an asset from service, including physical removal, environmental remediation, and disposal, while ensuring regulatory compliance. | *   12.5 Construction & Commissioning | Disposal decision, Asset details | Retired asset, Disposal records, Environmental compliance docs | Decommissioning cost/schedule variance |

---

## 3. Cross-Value Stream Dependencies

*   **AOV-01** provides the strategic context and triggers most work in **AOV-02 Capital Project Delivery**.
*   It governs the assets that are operated and maintained within **AOV-03 Work & Outage Management**, **AOV-04 Electric Energy Delivery**, and **AOV-05 Natural Gas Delivery**.
*   The investment decisions made here are a primary driver for **REV-01 Rate Case & Cost Recovery**.
*   Asset health and risk data are critical inputs for **AOV-06 System Reliability & Emergency Response**.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Asset Management Leadership, Engineering, Finance, BA Working Group
**Approval:** Chief Operations Officer (COO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for AOV-01.

**Next Review:** Annually or upon major changes in asset management strategy.

---

**End of Document**
