# Value Stream Heat Maps
## Quantum Energy - Strategic Visualizations

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Conceptual heat maps visualizing Quantum Energy's value streams based on various criteria
**Framework Standards:** BIZBOK
**Related Documents:**
*   [Enterprise Value Streams Catalog (ent-value-streams-catalog.md)](../ent-value-streams-catalog.md)
*   [Quantum Energy Strategic Objectives](../../2-STRATEGY/ent-strategic-objectives.md)
*   [Current State Value Stream Performance Metrics (current-state-metrics.md)](./current-state-metrics.md)
*   [Target State Value Stream Performance Metrics (target-state-metrics.md)](./target-state-metrics.md)

---

## Executive Summary

This document presents conceptual heat maps to visually represent key aspects of Quantum Energy's business value streams. These visualizations provide quick insights into their strategic importance, current performance (relative to targets), and where investment is most needed to achieve our strategic objectives across both our regulated and non-regulated operations.

---

## 1. Introduction to Heat Maps

Value stream heat maps serve as a high-level communication tool for stakeholders to quickly grasp the status and priority of end-to-end value delivery. The color coding (typically Red, Amber, Green, or shades thereof) indicates the status or priority based on a defined legend.

**Color Legend (Illustrative):**
*   **Dark Green:** Exceeding Target / Very High Performance
*   **Light Green:** Meeting Target / High Performance
*   **Yellow:** Near Target / Medium Performance (some gaps)
*   **Orange:** Below Target / Low Performance (significant gaps)
*   **Red:** Significantly Below Target / Very Low Performance (critical issues)

---

## 2. Strategic Importance Heat Map

This heat map illustrates the strategic importance of each value stream to Quantum Energy's overall 2025-2030 strategy, balancing regulated obligations with non-regulated growth targets. Importance is assessed based on direct contribution to strategic themes and objectives, regulatory criticality, and revenue generation potential.

```mermaid
graph TD
    subgraph Regulated Customer Value Streams
        A1[RCV-01: Regulated Customer Acquisition]
        A2[RCV-02: Regulated Customer Service Delivery]
        A3[RCV-03: Regulated Billing & Payment]
        A4[RCV-04: Regulated Customer Program Participation]
        A5[RCV-05: Regulated Service Disconnection & Reconnection]
    end

    subgraph Non-Regulated Customer Value Streams
        B1[NCV-01: Smart Home Solution Delivery]
        B2[NCV-02: EV Charging Solution Deployment]
        B3[NCV-03: Distributed Generation (DG) & Storage Solution Provision]
        B4[NCV-04: Non-Regulated Energy Advisory & Consulting]
    end

    subgraph Asset and Operations Value Streams
        C1[AOV-01: Asset Lifecycle Management]
        C2[AOV-02: Capital Project Delivery]
        C3[AOV-03: Work & Outage Management]
        C4[AOV-04: Electric Energy Delivery]
        C5[AOV-05: Natural Gas Delivery]
        C6[AOV-06: System Reliability & Emergency Response]
    end

    subgraph Supply and Market Value Streams
        D1[SMV-01: Electric Energy Supply & Trading]
        D2[SMV-02: Natural Gas Supply & Trading]
        D3[SMV-03: Distributed Energy Resource (DER) Aggregation & Optimization]
        D4[SMV-04: Non-Regulated Energy Market Participation]
    end

    subgraph Regulatory & External Affairs Value Streams
        E1[REV-01: Rate Case & Cost Recovery]
        E2[REV-02: Regulatory Compliance & Reporting]
        E3[REV-03: External Stakeholder Engagement]
        E4[REV-04: Environmental Stewardship & Compliance]
    end

    subgraph Enterprise Support Value Streams
        F1[ESV-01: Enterprise Strategic Planning & Execution]
        F2[ESV-02: Talent Management]
        F3[ESV-03: Financial Management & Reporting]
        F4[ESV-04: Information Technology & Digital Service Delivery]
        F5[ESV-05: Enterprise Risk Management]
        F6[ESV-06: Procurement & Supply Chain Management]
    end

    %% Apply colors based on perceived Strategic Importance
    class A1,A2,A3,C4,C5,C6,E1,E2,F1 color:white,fill:#7CFC00; %% Dark Green - Very High (Core utility, critical regulatory, strategic guidance)
    class B1,B2,B3,D3,D4 color:white,fill:#90EE90; %% Light Green - High (Key non-regulated growth engines)
    class A4,A5,B4,C1,C2,C3,D1,D2,E3,E4,F2,F3,F4,F5,F6 color:white,fill:yellow; %% Yellow - Medium (Important supporting or growth areas)
```

**Interpretation:**
*   **Very High Strategic Importance (Dark Green):** Critical for core utility operations (e.g., Energy Delivery, Regulated Customer Service), regulatory compliance (Rate Case, Regulatory Compliance), and enterprise strategic direction.
*   **High Strategic Importance (Light Green):** Represents the primary drivers of non-regulated growth and diversification (e.g., Smart Home, EV Charging, DER Aggregation) which are key to Quantum Energy's future.
*   **Medium Strategic Importance (Yellow):** Important supporting value streams and other regulated or non-regulated offerings that contribute to overall success but might not be existential.

---

## 3. Current Performance Heat Map (Relative to Target)

This heat map visualizes the current performance of key value streams relative to their defined target metrics (from `current-state-metrics.md` and `target-state-metrics.md`).

```mermaid
graph TD
    subgraph Regulated Customer Value Streams
        A1[RCV-01: Regulated Customer Acquisition]
        A2[RCV-02: Regulated Customer Service Delivery]
    end

    subgraph Non-Regulated Customer Value Streams
        B1[NCV-01: Smart Home Solution Delivery]
        B2[NCV-02: EV Charging Solution Deployment]
    end

    subgraph Asset and Operations Value Streams
        C1[AOV-04: Electric Energy Delivery]
        C2[AOV-05: Natural Gas Delivery]
    end

    subgraph Regulatory & External Affairs Value Streams
        D1[REV-01: Rate Case & Cost Recovery]
    end

    subgraph Enterprise Support Value Streams
        E1[ESV-01: Enterprise Strategic Planning & Execution]
    end

    %% Apply colors based on Current Performance (Red to Dark Green)
    class A1,A2,B1,B2,E1 color:white,fill:orange; %% Below Target / Low Performance (significant gaps)
    class C1,C2,D1 color:white,fill:yellow; %% Near Target / Medium Performance (some gaps)
```

**Interpretation:**
*   **Orange (Low Performance):** Value streams showing significant gaps between current performance and target metrics. These require substantial focus and transformation initiatives (e.g., Regulated Customer Service, Smart Home Solution Delivery).
*   **Yellow (Medium Performance):** Value streams that are performing reasonably well but still have room for improvement to meet target metrics (e.g., Electric Energy Delivery, Rate Case).

---

## 4. Investment Priority Heat Map

This heat map combines strategic importance and performance gaps to indicate where Quantum Energy should prioritize its investment in value stream optimization and transformation.

```mermaid
graph TD
    subgraph Regulated Customer Value Streams
        A1[RCV-01: Regulated Customer Acquisition]
        A2[RCV-02: Regulated Customer Service Delivery]
    end

    subgraph Non-Regulated Customer Value Streams
        B1[NCV-01: Smart Home Solution Delivery]
        B2[NCV-02: EV Charging Solution Deployment]
    end

    subgraph Asset and Operations Value Streams
        C1[AOV-04: Electric Energy Delivery]
        C2[AOV-05: Natural Gas Delivery]
    end

    subgraph Regulatory & External Affairs Value Streams
        D1[REV-01: Rate Case & Cost Recovery]
    end

    subgraph Enterprise Support Value Streams
        E1[ESV-01: Enterprise Strategic Planning & Execution]
    end

    %% Apply colors based on Investment Priority (Red = High, Yellow = Medium, Green = Low)
    %% High Priority: High Strategic Importance AND Low Performance
    %% Medium Priority: High Strategic Importance AND Medium Performance OR Medium Strategic Importance and Low Performance
    %% Low Priority: High Performance OR Low Strategic Importance
    class A1,A2,B1,B2 color:white,fill:red; %% High Investment Priority (Critical for Customer Experience & Non-Reg Growth)
    class C1,C2,D1,E1 color:white,fill:orange; %% Medium Investment Priority (Important for Core Ops & Strategic Mgmt)
```

**Interpretation:**
*   **Red (High Priority):** These value streams are strategically critical and currently underperforming significantly. They demand immediate and substantial investment to close performance gaps and unlock strategic value (e.g., Regulated Customer Service, Non-Regulated Solution Delivery). These often drive multiple strategic objectives.
*   **Orange (Medium Priority):** These value streams are strategically important and have some performance gaps. They require focused initiatives to reach target performance (e.g., Core Energy Delivery, Strategic Planning).

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** BA Review Board, Strategic Planning Office, Executive Leadership
**Approval:** Chief Strategy Officer
**Version History:**
- v1.0 (2025-11-25): Initial draft of Value Stream Heat Maps for Quantum Energy.

**Next Review:** Annually (aligns with Strategic Plan and investment cycles)

---

**End of Document**
