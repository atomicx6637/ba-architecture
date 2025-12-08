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

### 2.5. Demand Management Workflow & Stage-Gate Requirements

This section defines the end-to-end workflow for demand management, aligned with the official **ESV-07: Demand Management Value Stream**. It outlines the specific requirements and key decisions at each stage for each demand tier.

**Note:** The **Break-Fix** tier is explicitly excluded from this workflow. It is considered an operational process managed via the standard incident management ticketing system.

#### 2.5.1. Workflow Stages (Value Stream Aligned)

| Stage | Purpose | Key Activities |
| :--- | :--- | :--- |
| **1. Draft** | Idea capture. | An idea is documented by a potential sponsor using a demand management tool. |
| **2. Submitted** | Formal submission for review. | The sponsor formally submits the demand, indicating it is ready for initial screening. |
| **3. Screening** | Initial triage and validation. | The EPMO and EA perform a quick review to ensure completeness, check for duplicates, and assign/validate the tier. |
| **4. Qualified** | Business case development. | The sponsor, often with support from a BA or EA, develops the detailed business case and requirements. |
| **5. Approved** | Governance and funding decision. | Governance bodies (Subcommittee and TAC) review the business case, prioritize the demand, and make a final "Go/No-Go" funding decision. |
| **6. Completed** | Handoff to execution. | Once funded, the demand is formally converted into a project and handed off to the EPMO and delivery teams. The demand record is closed. |

#### 2.5.2. Stage-Gate Requirements by Tier

| Stage | Enhancement (< $50k) | Tier 3 (< $500k) | Tier 2 ($500k - $2M) | Tier 1 (> $2M) |
| :--- | :--- | :--- | :--- | :--- |
| **Submitted** | **Form:** Simplified 1-Page Demand. <br> **Data:** Problem statement, requested change, business owner. | **Form:** Standard Demand Record. <br> **Data:** All fields in the standard record must be complete at a high level. | **Form:** Standard Demand Record. <br> **Data:** All fields must be complete with a high degree of confidence. | **Form:** Program Brief or Strategic Charter. <br> **Data:** Outlines strategic intent, vision, and expected enterprise-level outcomes. |
| **Screening** | **Process:** N/A (Handled by Team Lead). | **By:** EPMO/EA. <br> **Gate:** Is the form complete? Is the tier correct? Is it a duplicate? | **By:** EPMO/EA. <br> **Gate:** Same as Tier 3. High-level check for major architectural or cross-portfolio conflicts. | **By:** EPMO/EA/Strategy Office. <br> **Gate:** Same as Tier 2, plus validation of alignment with documented corporate strategic objectives. |
| **Qualified** | **Process:** N/A. | **By:** Business Sponsor. <br> **Requirement:** "Right-sized" business case with clear problem statement, proposed solution, cost/resource estimate (T-shirt size), and benefit estimate (ROI). | **By:** Business Sponsor + assigned BA/EA. <br> **Requirement:** Formal business case. Includes financial analysis (NPV/IRR), risk assessment, and **mandatory formal architectural review**. | **By:** Program Director + Dedicated Team. <br> **Requirement:** Comprehensive program charter and business case. Includes multi-year financial plan, benefits realization plan, and a future-state architecture vision. |
| **Approved** | **By:** Team/Business Unit Lead. <br> **Gate:** Does this fit within our enhancement budget? Final approval for team backlog. | **By:** Technology Subcommittee & TAC. <br> **Gate:** Subcommittee prioritizes and recommends. TAC provides final "Go/No-Go" funding approval, often via consent agenda. | **By:** Technology Subcommittee & TAC. <br> **Gate:** Subcommittee performs deep review of dependencies and recommends. TAC provides final "Go/No-Go" funding, typically requiring sponsor presentation. | **By:** Technology Subcommittee & TAC. <br> **Gate:** Subcommittee reviews for portfolio impact and readiness. TAC makes final strategic investment decision based on formal executive presentation. |
| **Completed** | **Handoff:** Added to team-level Kanban board/backlog for execution. | **Handoff:** EPMO assigns a Project Manager. Project Charter is finalized. Demand record is closed. | **Handoff:** Same as Tier 3. | **Handoff:** Program Director is formally chartered. EPMO establishes program-level governance and initiates project workstreams. Demand record is closed. |

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

---

## 5. Demand Tier Scenario Workflows

This section provides practical, narrative-based examples for each demand tier to illustrate how the governance process looks and feels to the stakeholders involved.

### Break-Fix Scenario
*   **Example Project:** A critical database server supporting the customer information system fails, making the application inaccessible to call center agents.
*   **Stakeholder Workflow & Experience:**
    *   **The User (Call Center Agent):** Experiences an application error. They report it immediately through the designated help desk channel. Their experience is one of urgency and waiting for a resolution.
    *   **IT Operations/On-Call Team:** An automated alert is triggered, and a high-priority incident ticket is created in the system (e.g., ServiceNow). The on-call team is paged and immediately begins diagnosis and remediation. The entire process is managed within the incident management system.
    *   **The Experience:** There is no "demand" or "project" paperwork. The process is one of **autonomy and urgency**. The goal is immediate service restoration, and the work is tracked via an operational ticket, not a demand record. Funding comes from the operational expenditure (OpEx) budget.

### Enhancement Scenario
*   **Example Project:** The Regulated Billing team wants to add a new "Notes" field to an internal dashboard they use to track complex billing inquiries, allowing them to better document the context of each case.
*   **Stakeholder Workflow & Experience:**
    *   **The User (Billing Analyst):** Mentions the idea to their manager during a team meeting, explaining how it would save time and reduce errors.
    *   **The Team Lead:** Recognizes the value and simplicity of the request. They confirm with their technical liaison that this is a small change (e.g., less than 40 hours of work).
    *   **The Experience:** The Team Lead fills out a simplified, one-page demand form. Since the cost is well under the $50k threshold, they approve it directly using their **pre-allocated annual enhancement budget**. The request is added to their team-level Kanban board and prioritized against other small enhancements. The central governance bodies (Subcommittee, TAC) are not involved, providing a **lightweight and autonomous** experience.

### Tier 3 Scenario
*   **Example Project:** The Fleet Management department wants to purchase and implement a new GPS tracking and telematics system for their vehicle fleet to optimize routes and monitor vehicle health. The total cost is estimated at $225,000.
*   **Stakeholder Workflow & Experience:**
    *   **The Sponsor (Fleet Manager):** Works with a business analyst to complete the standard demand record and business case. They detail the expected benefits, including fuel savings, improved maintenance scheduling, and increased driver safety, projecting an ROI within two years.
    *   **Enterprise Architecture (EA):** During the `Screening` stage, an architect quickly reviews the proposal. They confirm the solution doesn't conflict with other enterprise systems and that the data integration plan is sound. They confirm it is correctly tiered as Tier 3.
    *   **Technology Subcommittee:** The Fleet Manager presents the business case to the committee. The committee members (representing various business units) review the case, ask clarifying questions about the ROI calculation, and confirm it aligns with the broader corporate goal of "Operational Excellence." They agree it's a solid, well-defined project and prioritize it highly on their recommended funding list.
    *   **Technology Advisory Committee (TAC):** The project appears on the consent agenda recommended by the Subcommittee. Seeing the clear ROI and the Subcommittee's endorsement, the **TAC provides final funding approval** with minimal debate. The experience is one of **standardized review and justification**.

### Tier 2 Scenario
*   **Example Project:** Upgrade the core middleware platform that connects the CRM and Billing systems. The platform is approaching its end-of-life, creating performance and security risks. The total project cost is estimated at $1.2 million.
*   **Stakeholder Workflow & Experience:**
    *   **The Sponsor (IT Platform Owner):** Develops a comprehensive demand record that focuses heavily on risk mitigation, technical debt reduction, and ensuring future business continuity. The business case is less about new features and more about preventing future problems.
    *   **Enterprise Architecture (EA):** Conducts a **formal architectural review**. They create diagrams showing the numerous upstream and downstream systems that will be impacted by the upgrade. They identify that this will require coordinated testing from the Customer Service, Billing, and Marketing teams. Due to this high level of cross-portfolio dependency, they confirm its Tier 2 classification.
    *   **Technology Subcommittee:** The review is more extensive. The IT Platform Owner presents, but representatives from the affected business units are also present. They discuss the proposed project timeline and negotiate a testing and deployment schedule that minimizes disruption to their critical business operations. The Subcommittee debates the urgency of this technical project versus a revenue-generating business project, ultimately agreeing that the risk of platform failure is too high to ignore. They recommend it for funding.
    *   **Technology Advisory Committee (TAC):** The IT Platform Owner and the Lead Enterprise Architect co-present the project. The TAC members, including senior VPs, ask pointed questions about the business continuity plan during the upgrade and the specific security vulnerabilities being addressed. Convinced of the strategic necessity of this foundational investment, they **approve the funding**. The experience is one of **formal, cross-functional alignment and risk-based decision-making**.

### Tier 1 Scenario
*   **Example Project:** A multi-year, enterprise-wide program to implement a "Unified Customer Experience" platform. This involves replacing the legacy residential and commercial CRM systems with a single, modern platform and building a new customer-facing portal. The total program cost is projected to be over $15 million.
*   **Stakeholder Workflow & Experience:**
    *   **The Sponsor (VP of Customer Experience):** This initiative is born directly from the company's annual strategic plan. The sponsor, along with a dedicated team of senior leaders, develops a detailed program charter and business case that articulates a transformational vision for customer interaction.
    *   **Enterprise Architecture (EA):** Is a core part of the program planning team from the very beginning. They work with the sponsor to define the future-state business capabilities and create the high-level technology roadmap that will enable the vision.
    *   **Technology Subcommittee:** The program is presented to the Subcommittee for awareness and to understand its significant impact on all other portfolio planning. The Subcommittee's role is not to question the strategic decision but to review the plan for readiness and identify major dependencies and resource constraints that need to be communicated to the TAC. They confirm its strategic priority.
    *   **Technology Advisory Committee (TAC):** The presentation is a major event on the TAC's agenda. The **Business Sponsor (VP) presents the strategic vision** and the expected transformation in customer satisfaction and operational efficiency. The EA presents the multi-year architectural roadmap. The CFO discusses the capital funding strategy. The debate is not about "if," but "how." The TAC, composed of C-level executives, makes the final **strategic investment decision**, approving the program and chartering it with the authority to move forward. The experience is one of **top-down, strategy-driven, executive-level decision-making**.
