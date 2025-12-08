# EA and EPMO RACI Matrix (Process-Ownership Model)

This document defines the roles and responsibilities of the Enterprise Architecture (EA) team, Enterprise Project Management Office (EPMO), and key governance bodies. This revision reflects a clear process-ownership model where **EA manages the Demand Management process** and the **EPMO manages the Project & Program Delivery process**.

**RACI Key:**
- **R** = Responsible (Does the work)
- **A** = Accountable (Owns the work/process)
- **C** = Consulted (Provides input)
- **I** = Informed (Is kept up-to-date)

---

## ESV-07: Demand Management Value Stream (EA Owned)

EA is accountable for the end-to-end Demand Management process. The **Technology Subcommittee** provides review and ranking support, and the **Technology Advisory Committee (TAC)** provides final financial approval.

| Value Stream Stage | Key Activity | EA Role | EPMO Role | Tech Subcommittee | TAC | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Draft** | Stakeholder captures initial idea. | A | I | I | I | EA owns the intake process. All other parties are informed a demand is being drafted. |
| **2. Submitted**| Demand is formally logged for review. | A | I | I | I | EA is accountable for receiving and assigning new demands. |
| **3. Screening** | High-level assessment for duplication and strategic fit. | A/R | C | C | I | EA performs the screening, consulting EPMO for project complexity and the Subcommittee for business area context. |
| **4. Qualified** | Develop business case and architectural assessment. | A/R | C | C | I | EA develops the business case, consulting EPMO on estimates and the Subcommittee to ensure business needs are met. |
| **5. Approved** | Score and stack rank demands with Subcommittee review. | A/R | I | R | I | EA is accountable for the scoring process. The Tech Subcommittee is **Responsible** for reviewing and providing ranking input. |
| | Present final recommendation for approval. | R | I | C | A | The TAC is **Accountable** for the final funding decision. EA is Responsible for presenting. The Subcommittee is Consulted as liaisons. |
| **6. Completed** | Formally hand off approved demand to EPMO. | A/R | R | I | I | EA is accountable for the hand-off. EPMO is responsible for accepting the new project. |

---

## ESV-08: Project & Program Delivery Value Stream (EPMO Owned)

EPMO is accountable for the end-to-end Project & Program Delivery process. EA is consulted for architectural guidance and to ensure strategic alignment is maintained.

| Value Stream Stage | Key Activity | EPMO Role | EA Role | Notes |
| :--- | :--- | :--- | :--- | :--- |
| **1. Initiating**| Develop and approve the Project Charter. | A/R | C | EPMO owns project initiation. EA is consulted to ensure the charter aligns with the intent of the original demand. |
| **2. Planning** | Develop detailed Project Management Plan (PMP). | A/R | C | EPMO owns the PMP. EA is consulted for architectural plans and to ensure they are integrated into the main schedule. |
| | Provide detailed Solution Architecture. | C | R/A | While EPMO owns the overall plan, EA is accountable for delivering the solution architecture as a key input to that plan. |
| **3. Executing** | Direct and manage project work. | A/R | I | EPMO owns project execution. EA is informed of status. |
| | Conduct architectural compliance reviews. | C | A/R | EA is accountable for architectural governance and performs the reviews. EPMO is consulted and must accommodate them in the plan. |
| **4. Delivering** | Manage deployment and transition to operations. | A/R | C | EPMO owns the delivery and go-live. EA is consulted to ensure architectural integrity during deployment. |
| **5. Closing** | Formally close the project and document lessons learned. | A/R | C | EPMO owns project closure. EA is consulted for feedback on the architectural process and outcomes. |
