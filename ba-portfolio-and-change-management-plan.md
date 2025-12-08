# Strategic Portfolio and Change Management Plan

## 1. Introduction and Vision

This document outlines a phased approach to establish a robust Portfolio Management capability and a supporting Change Management plan to ensure its successful adoption. The vision is to create a system that provides **full transparency** into all significant technology and business initiatives while empowering teams with the **autonomy** to manage smaller-scale work efficiently.

The initial focus of this plan is on maturing the **Demand Management value stream**, which is the critical front-end process for intake, evaluation, and prioritization, occurring before an initiative is formally handed off to the Project Management value stream for execution.

Our success will be measured by our ability to build this capability over several years, tracking progress through key metrics focused on **visibility, efficiency, and productivity**.

---

## 2. Portfolio Management Approach

### 2.1. Portfolio Structure

To start simply, portfolios will be structured to mirror our organizational design, not by products or value streams. This provides clear ownership and aligns with existing budgeting processes.

*   **Initial Structure:** Portfolios will be aligned to major **Teams or Business Units**.
    *   *Example Portfolios: Regulated Operations, Customer Experience & Solutions, Enterprise Corporate Systems, etc.*
*   **Future Evolution:** As our maturity grows (Year 3+), we will evolve this model to align portfolios with end-to-end Value Streams, enabling a more strategic, customer-centric view of investment.

### 2.2. Demand Tiers & Governance

To balance autonomy with oversight, all incoming demand will be categorized into tiers. The **Technology Subcommittee** serves as the primary body for reviewing and ensuring the prioritization of all project investments is aligned with strategic objectives. The **Technology Advisory Committee (TAC)** serves as the single, final authority for funding all projects.

| Tier | Description | Budget | Governance & Documentation Level |
| :--- | :--- | :--- | :--- |
| **Break-Fix** | Urgent, non-discretionary work required to restore service in production environments. | N/A (OpEx) | **Autonomy:** Managed within operational teams via standard ticketing. No formal demand record is needed. |
| **Enhancement**| Small, discretionary improvements to existing systems or processes. | < $50k | **Lightweight:** A simplified, one-page demand form. Approved directly by the team/business unit lead. Tracked on a team-level Kanban board for visibility. |
| **Tier 3** | Small, discrete projects with localized impact. | < $500k | **Standard:** Full demand record and business case required. Reviewed and prioritized by the **Technology Subcommittee**, then presented to the **TAC for final funding approval**. |
| **Tier 2** | Medium-sized projects with significant cross-team or business unit impact. | $500k - $2M | **Formal:** As above, plus a formal architectural review by EA. Reviewed and prioritized by the **Technology Subcommittee**, then presented to the **TAC for final funding approval**. |
| **Tier 1** | Large, strategic programs with major enterprise-wide impact. | > $2M | **Strategic:** As above. Presented by the business sponsor and EA to the **TAC for final funding approval**, with prioritization confirmed by the Subcommittee. |

> **Complexity Adjustment Rule:** A demand's tier can be elevated (e.g., a Tier 3 moved to Tier 2 governance) if it is deemed to have high complexity, significant cross-portfolio dependencies, or major architectural impact. This determination is made by the Enterprise Architecture (EA) team during the `Screening` stage.

### 2.3. Governance Charters

To ensure the governance process is clear and effective, the following charters define the mandates and responsibilities of the key oversight bodies in the Demand Management process.

#### **Technology Subcommittee Charter**

The Technology Subcommittee is the primary review and alignment body responsible for preparing demands for executive-level funding decisions.

**Mandate & Responsibilities:**
*   **Review:** Assess all Tier 1, 2, and 3 demands for clarity, completeness, business value, and alignment with Business Unit strategy.
*   **Prioritize:** Be responsible for the stack-ranking of demands within their respective portfolios, balancing business needs with resource realities and technical feasibility.
*   **Validate:** Ensure that a sound business case exists for each demand and that it is accurately tiered according to the defined budget and complexity rules.
*   **Recommend:** Formulate and present a formal, prioritized portfolio recommendation to the Technology Advisory Committee (TAC) for funding.
*   **Liaise:** Act as the primary communication channel between their respective operational teams and the TAC, providing context and answering questions on submitted demands.

#### **Technology Advisory Committee (TAC) Charter**

The Technology Advisory Committee (TAC) is the executive-level governance body with ultimate financial authority over the technology and business project portfolio.

**Mandate & Responsibilities:**
*   **Approve Funding:** Serve as the single, final authority for the financial approval and funding of all Tier 1, 2, and 3 projects.
*   **Strategic Oversight:** Ensure the overall investment portfolio is directly aligned with the company's annual and long-term strategic objectives.
*   **Make Go/No-Go Decisions:** Review the prioritized list of demands recommended by the Technology Subcommittee and make binding "Go/No-Go" decisions on which initiatives will be chartered as formal projects.
*   **Monitor Portfolio Health:** Periodically review the health of the overall portfolio and the progress of major strategic (Tier 1) initiatives.

### 2.4. Annual Enhancement Budget Allocation

To empower teams with autonomy while ensuring strategic investment in the continuous improvement of our core systems, the following process will be used to allocate the annual "Enhancement" tier budget.

**Goal:** To move from a purely "gut feel" budget allocation to a data-driven approach that directs funds toward the systems and capabilities that need it most.

**Annual Process:**

*   **Step 1: Data Collection & Analysis (Q3)**
    *   The Enterprise Architecture (EA) team will partner with IT Operations and Business Unit leads to gather metrics on our core systems and capabilities.
    *   **Key Data Points:** System stability (e.g., number of break-fix tickets), technology health (e.g., age of tech stack), business criticality, and user feedback/pain points.
*   **Step 2: Strategic Assessment (Q3)**
    *   The **Technology Subcommittee** reviews the collected data to identify investment themes for the upcoming year. For example, they may determine that the legacy CRM system requires a larger enhancement budget to address technical debt, while the new ERP system needs funding focused on user-experience tweaks.
*   **Step 3: Budget Proposal & Allocation (Q4)**
    *   Based on the assessment, the Subcommittee proposes a total enhancement budget for the upcoming year, with recommended allocations for each major system, capability, or business unit portfolio.
    *   This proposal is submitted to the **TAC** for review and approval as part of the overall annual budgeting process. The TAC approves the total allocation for each area, not the individual enhancements.
*   **Step 4: Autonomous Execution (Throughout the Year)**
    *   Once the TAC approves the budget, the allocated funds are given to the respective team or business unit leads.
    *   These leaders have full autonomy to approve individual enhancement requests (<$50k) against their budget throughout the year. They are accountable for managing their allocated funds and are required to maintain visibility of all work on their team-level Kanban boards.

---

## 3. Phased Maturity Roadmap (3-Year Plan)

### Year 1: Foundation & Visibility
*   **Primary Goal:** Establish the process and achieve full transparency into all planned work.
*   **Key Actions:**
    1.  **Implement Process:** Formally launch the Demand Management value stream and the tiering model.
    2.  **Constitute Governance:** Formally charter the Technology Subcommittee and Technology Advisory Committee (TAC) with clear mandates.
    3.  **Train Stakeholders:** Conduct comprehensive training on the new intake process, tiering model, and the role of the governance bodies.
    4.  **Build Dashboards:** Create initial portfolio dashboards in ServiceNow or a BI tool, providing a consolidated view of all Tier 1-3 demands by Business Unit.
*   **Success Metrics:**
    *   **Visibility:** >90% of all project-based work is captured in the demand system.
    *   **Efficiency:** Establish a baseline for the average cycle time from `Submitted` to `Approved` for each tier.

### Year 2: Optimization & Efficiency
*   **Primary Goal:** Refine the process, improve flow, and introduce capacity-aware planning.
*   **Key Actions:**
    1.  **Analyze & Refine:** Use Year 1 metrics to identify and address bottlenecks in the review and approval process.
    2.  **Introduce Capacity Planning:** The EPMO and relevant team leads will provide high-level resource estimates (in FTEs) during the `Qualified` stage to inform prioritization.
    3.  **Automate Reporting:** Automate the generation and distribution of portfolio health reports and dashboards.
*   **Success Metrics:**
    *   **Visibility:** Portfolio dashboards include high-level resource demand vs. capacity.
    *   **Efficiency:** Reduce the average `Submitted` to `Approved` cycle time by 15% from the Year 1 baseline.
    *   **Productivity:** Track the percentage of approved demands that successfully start execution within the planned quarter.

### Year 3: Strategic Alignment & Value Realization
*   **Primary Goal:** Shift the focus from managing a list of projects to managing investment alignment with strategic goals.
*   **Key Actions:**
    1.  **Evolve Portfolio Structure:** Begin a pilot to structure one portfolio around a core Value Stream (e.g., "Customer Acquisition") instead of a business unit.
    2.  **Introduce Benefits Realization:** Implement a lightweight process, owned by the EPMO, to track the stated benefits of completed Tier 1 and 2 projects against their original business case.
    3.  **Integrate with Annual Planning:** The portfolio approval process becomes a primary input into the annual corporate budgeting and strategic planning cycle.
*   **Success Metrics:**
    *   **Visibility:** Portfolio views clearly map each Tier 1 and Tier 2 initiative back to a primary corporate strategic objective.
    *   **Efficiency:** >75% of the total project budget is allocated to initiatives aligned with the top 3 corporate strategic objectives.
    *   **Productivity:** Report on the benefits realized (e.g., cost savings, revenue growth) from projects completed in the prior year.

---

## 4. Change Management Plan (ADKAR Framework)

*   **Awareness** (The "Why"):
    *   Communicate the vision and goals through leadership town halls and targeted emails. Emphasize that the goal is *not* more bureaucracy, but "right-sized" governance and greater autonomy for smaller tasks.
*   **Desire** (The "What's in it for me?"):
    *   Engage directly with team leads and managers. Highlight the benefits: clear approval paths for big ideas and a "fast lane" with minimal overhead for Enhancements and Break-Fixes.
*   **Knowledge** (The "How"):
    *   Conduct mandatory but practical training workshops focused on the new intake process, how to select the right tier, and what constitutes a "good enough" business case for Tier 3.
    *   Provide simple cheat sheets, templates, and quick-reference guides.
*   **Ability** (The "Let me try"):
    *   Host "Portfolio Office Hours" where the EA team can personally walk stakeholders through submitting their first few demands. This hands-on support is critical for building confidence.
*   **Reinforcement** (The "Let's stick with it"):
    *   Celebrate and publicize early wins, such as a team successfully managing its own enhancements or a Tier 1 project getting funded through the new process.
    *   Share the portfolio dashboards widely to make the benefits of transparency tangible to everyone.
    *   Establish a simple feedback mechanism (e.g., a dedicated Teams channel) to gather input on the process and make iterative improvements, demonstrating that this is an evolving system.
