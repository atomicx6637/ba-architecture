# Capability Heat Maps
## Quantum Energy - Strategic Visualizations

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Conceptual heat maps visualizing Quantum Energy's capabilities based on various criteria
**Framework Standards:** BIZBOK
**Related Documents:**
*   [Enterprise Capabilities - Level 1 and Level 2](../../ent-capabilities-l1-l2.md)
*   [Quantum Energy Strategic Objectives](../../2-STRATEGY/ent-strategic-objectives.md)
*   [Current State Capability Maturity Assessment](../capability-assessments/capability-maturity-current.md)
*   [Target State Capability Maturity Assessment](../capability-assessments/capability-maturity-target.md)
*   [Capability Gap Analysis](../capability-assessments/capability-gap-analysis.md)

---

## Executive Summary

This document presents conceptual heat maps to visually represent key aspects of Quantum Energy's business capabilities. These visualizations provide quick insights into strategic importance, current maturity, and investment priority, highlighting areas that require immediate attention and strategic focus across both our regulated and non-regulated operations.

---

## 1. Introduction to Heat Maps

Heat maps are a powerful visualization tool used in Business Architecture to convey complex information about capabilities at a glance. They allow stakeholders to quickly identify areas of strength, weakness, strategic focus, and investment need. The color coding (typically Red, Amber, Green, or shades thereof) indicates the status or priority based on a defined legend.

**Color Legend (Illustrative):**
*   **Dark Green (5):** Optimizing / Very High
*   **Light Green (4):** Quantitatively Managed / High
*   **Yellow (3):** Defined / Medium
*   **Orange (2):** Managed / Low
*   **Red (1):** Initial / Very Low

---

## 2. Strategic Importance Heat Map (L1 Capabilities)

This heat map illustrates the strategic importance of each Level 1 capability to Quantum Energy's overall 2025-2030 strategy. Importance is assessed based on direct contribution to strategic themes and objectives, as well as criticality for regulated compliance and non-regulated growth.

```mermaid
graph TD
    subgraph Strategic Capabilities
        A1[1. Enterprise Strategy & Performance Management]
        A2[2. Market Development & Competitive Intelligence]
        A3[3. Regulatory & Government Affairs]
        A4[4. Brand & Reputation Management]
    end

    subgraph Core Capabilities
        B1[5. Energy Generation]
        B2[6. Natural Gas Supply & Storage]
        B3[7. Energy Transmission]
        B4[8. Electric Distribution]
        B5[9. Gas Distribution]
        B6[10. Customer Engagement & Service]
        B7[11. Non-Regulated Product Development]
        B8[12. Non-Regulated Sales & Marketing]
        B9[13. System Operations & Grid Control]
    end

    subgraph Supporting Capabilities
        C1[14. Financial Management]
        C2[15. Human Capital Management]
        C3[16. Information Technology & Digital Services]
        C4[17. Procurement & Supply Chain Management]
        C5[18. Legal & Compliance]
    end

    %% Apply colors based on perceived Strategic Importance
    class A1,A2,A3,A4,B4,B6,B7,B8,B9,C3,C5 color:white,fill:#7CFC00; %% Dark Green - Very High
    class B1,B2,B3,B5,C1,C2,C4 color:white,fill:#90EE90; %% Light Green - High
```

**Interpretation:**
*   **Very High Strategic Importance (Dark Green):** These capabilities are absolutely critical to Quantum Energy's existence and future success. This includes core strategic functions (e.g., Enterprise Strategy, Regulatory Affairs), fundamental customer interaction, critical grid operations, and the engines of non-regulated growth (Product Development, Sales & Marketing).
*   **High Strategic Importance (Light Green):** These capabilities are foundational to our operations and contribute significantly to strategic objectives, ensuring the reliable and efficient delivery of regulated services and supporting overall enterprise functions.

---

## 3. Current Maturity Heat Map (L2 Capabilities - Selected)

This heat map visually represents the current maturity levels for a selection of key Level 2 capabilities, based on the assessment in `capability-maturity-current.md`.

```mermaid
graph TD
    subgraph Regulated Operations
        A[8.5. Distribution Automation & Grid Modernization]
        B[9.5. Leak Detection & Pipeline Safety]
        C[13.3. Electric System Balancing & Dispatch]
    end

    subgraph Enterprise Core
        D[10.5. Digital Customer Experience]
        E[10.8. Customer Insights & Analytics]
        F[16.4. Cybersecurity & Information Security]
        G[14.2. General Accounting & Reporting]
    end

    subgraph Non-Regulated Growth
        H[11.3. Product Development & Engineering]
        I[12.4. Customer Acquisition & Conversion]
    end

    %% Apply colors based on Current Maturity (Level 1-5, Red to Dark Green)
    class A,D,E,H,I color:white,fill:orange; %% Level 2 (Managed/Planned)
    class B,F,G color:white,fill:yellow; %% Level 3 (Defined/Standardized)
    class C color:white,fill:#90EE90; %% Level 4 (Quantitatively Managed/Measured)
```

**Interpretation:**
*   **Orange (Level 2):** Indicates capabilities that are in an early stage of development, with processes managed but not yet standardized or widely adopted (e.g., Digital Customer Experience, Non-Regulated Product Development). These areas require significant investment.
*   **Yellow (Level 3):** Represents capabilities with defined processes and standards, but still room for quantitative management and optimization (e.g., Leak Detection, Cybersecurity).
*   **Light Green (Level 4):** Reflects highly mature capabilities that are quantitatively managed and predictable (e.g., Electric System Balancing & Dispatch), demonstrating operational excellence.

---

## 4. Investment Priority Heat Map (L2 Capabilities - Selected)

This heat map combines strategic importance and maturity/gap analysis to prioritize where Quantum Energy should focus its investment to achieve its strategic objectives. Capabilities with a large gap and high strategic importance will typically be "hot" (Red/Orange).

```mermaid
graph TD
    subgraph Regulated Operations
        A[8.5. Distribution Automation & Grid Modernization]
        B[9.5. Leak Detection & Pipeline Safety]
        C[13.3. Electric System Balancing & Dispatch]
    end

    subgraph Enterprise Core
        D[10.5. Digital Customer Experience]
        E[10.8. Customer Insights & Analytics]
        F[16.4. Cybersecurity & Information Security]
        G[14.2. General Accounting & Reporting]
    end

    subgraph Non-Regulated Growth
        H[11.3. Product Development & Engineering]
        I[12.4. Customer Acquisition & Conversion]
    end

    %% Apply colors based on Investment Priority (Red = High, Yellow = Medium, Green = Low)
    %% High Priority: High Strategic Importance AND large maturity gap (e.g., 2 levels or more)
    %% Medium Priority: High Strategic Importance AND moderate maturity gap (e.g., 1 level) OR medium strategic importance and large gap
    %% Low Priority: Already high maturity OR low strategic importance
    class A,D,E,H,I color:white,fill:red; %% High Investment Priority (Large Gap, High Strategic Impact)
    class B,F,G color:white,fill:orange; %% Medium Investment Priority (Moderate Gap, High Strategic Impact)
    class C color:white,fill:yellow; %% Lower Investment Priority (Small Gap, Already High Maturity)
```

**Interpretation:**
*   **Red (High Priority):** Capabilities where there is a significant gap between current and target maturity, and which are highly critical for achieving strategic objectives. These are prime candidates for major transformation initiatives and immediate investment (e.g., Digital Customer Experience, Non-Regulated Product Development).
*   **Orange (Medium Priority):** Capabilities that are strategically important and have a moderate maturity gap. These require continued investment and focused improvement efforts (e.g., Leak Detection, Cybersecurity).
*   **Yellow (Lower Priority):** Capabilities that are already highly mature or have a relatively small gap, requiring sustained but potentially lower-intensity investment to maintain excellence or achieve the next level (e.g., Electric System Balancing & Dispatch).

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** BA Review Board, Strategic Planning Office, Executive Leadership
**Approval:** Chief Strategy Officer
**Version History:**
- v1.0 (2025-11-25): Initial draft of Capability Heat Maps for Quantum Energy.

**Next Review:** Annually (aligns with Strategic Plan and investment cycles)

---

**End of Document**
