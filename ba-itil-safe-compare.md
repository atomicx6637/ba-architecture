# Value Stream Alignment with ITIL and SAFe

This document outlines how the defined Demand Management and Project Management value streams align with the principles and practices of the ITIL 4 and Scaled Agile (SAFe) frameworks.

### Demand Management Value Stream Alignment

Our Demand Management value stream (`Draft` -> `Submitted` -> `Screening` -> `Qualified` -> `Approved` -> `Completed`) serves as the strategic front door for all new work. It aligns very well with concepts in both ITIL and SAFe.

#### **Alignment with ITIL 4**

In ITIL 4, this process is a direct implementation of the **Demand Management** and **Portfolio Management** practices.

*   **Demand Management Practice:** The primary goal of this ITIL practice is to understand, anticipate, and influence customer demand for services.
    *   **`Draft` & `Submitted`:** These stages align with *identifying and logging sources of demand*.
    *   **`Screening` & `Qualified`:** These stages directly correspond to *analyzing patterns of business activity* and developing a business case for the demand, which is a core ITIL recommendation.
*   **Portfolio Management Practice:** This ITIL practice is responsible for managing the service portfolio. Our value stream feeds directly into it.
    *   **`Approved`:** This stage, where the Technology Advisory Committee (TAC) provides financial approval, **is** Portfolio Management in action. The TAC is acting as the governance body that decides which new services or projects will be chartered and funded, ensuring they align with the overall business strategy.
*   **Service Value Chain:** This entire value stream maps to the **"Plan"** and **"Engage"** activities within the ITIL Service Value Chain, where strategic planning and stakeholder engagement occur.

#### **Alignment with Scaled Agile Framework (SAFe)**

In SAFe, managing the intake and analysis of large initiatives is handled by the **Lean Portfolio Management (LPM)** function using a **Portfolio Kanban**. Our Demand Management value stream is a perfect representation of this system.

*   **Portfolio Kanban System:** The stages map almost one-to-one with the states in a SAFe Portfolio Kanban.
    *   **`Draft` & `Submitted`:** This is the **"Funnel"** in SAFe, where all new ideas and epics are captured.
    *   **`Screening`:** This corresponds to the **"Reviewing"** state, where an initial check for strategic fit and potential duplication is performed.
    *   **`Qualified`:** This is the **"Analyzing"** state. During this phase, a "Portfolio Epic" is elaborated with a lightweight business case, solution assessment, and definition of a Minimum Viable Product (MVP).
    *   **`Approved`:** This represents the "Go" decision from the Lean Portfolio Management function. Once approved, the Epic moves to the **"Portfolio Backlog"**, ready to be pulled by an Agile Release Train (ART).
*   **Lean Portfolio Management (LPM):** The roles we defined (EA, Tech Subcommittee, TAC) are an embodiment of the LPM function. The TAC, as the financial approval body, is fulfilling the LPM's responsibility for **Strategy & Investment Funding**.

---

### Project Management Value Stream Alignment

Our Project Management value stream (`Initiating` -> `Planning` -> `Executing` -> `Delivering` -> `Closing`) is defined in a more traditional, phase-gated manner. Here’s how it aligns and where it differs.

#### **Alignment with ITIL 4**

ITIL 4 is less prescriptive about project execution but provides key practices that this value stream supports.

*   **Project Management Practice:** ITIL acknowledges the need for a formal project management practice to create or modify services. Our value stream follows a structure very similar to common methodologies like PMI's PMBOK, which ITIL recommends.
*   **Service Transition:** This is a critical ITIL concept, and our value stream directly enables it.
    *   **`Delivering` & `Closing`:** These stages encompass the activities of Service Transition. This includes deployment, user acceptance testing, change management, and the formal handoff to operations, ensuring the new or changed service is stable and supportable.
*   **Change Enablement:** Throughout the `Executing` and `Delivering` stages, the ITIL practice of "Change Enablement" (formerly Change Management) would run in parallel to assess and control the risk of making changes to the production environment.

#### **Alignment with Scaled Agile Framework (SAFe)**

This is where the alignment is more conceptual than literal, as SAFe avoids traditional, phased-based project management.

*   **Philosophical Difference:** SAFe replaces temporary "projects" with long-lived, cross-functional **Agile Release Trains (ARTs)** that deliver value continuously. A pure SAFe implementation would not have a "Project Management" value stream in this form.
*   **Conceptual Mapping:** However, we can map the *intent* of our stages to SAFe events and activities. This can be useful for organizations transitioning to SAFe.
    *   **`Initiating` & `Planning`:** This work is analogous to what happens during a **PI Planning** event in SAFe. In PI Planning, teams and stakeholders come together to plan the features and stories for the next 8-12 week Program Increment (PI). The "Project Plan" from our value stream is conceptually similar to the set of **PI Objectives** created during this event.
    *   **`Executing`:** Instead of one long execution phase, this corresponds to the series of **Sprints/Iterations** within a PI where Agile teams build and test the features.
    *   **`Delivering`:** This maps to SAFe's principle of **"Release on Demand."** In SAFe, value is delivered to end-users when the business needs it, which can be at any point during a PI, decoupled from the development cadence.

In summary, your Demand Management process is highly aligned with modern Lean-Agile and IT Service Management principles. Your Project Management process follows a more traditional structure but can be seen as a wrapper for, or a bridge to, the iterative execution model promoted by frameworks like SAFe.
