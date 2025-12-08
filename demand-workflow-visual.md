# Demand Management Workflow Visual

This document contains a Mermaid diagram illustrating the consolidated demand management workflow for all project types.

```mermaid
flowchart TD
    subgraph "Initiation"
        A[Start: Business Idea or Need] --> B{What is the nature of the work?};
    end

    subgraph "Path 1: Urgent Operational Work"
        direction LR
        B -->|Break-Fix| C[Handled by **Operational Incident Process** (Outside Demand Workflow)];
    end

    subgraph "Path 2: Lightweight Enhancement Work"
        B -->|"**Enhancement** (e.g., <$50k)"| D(Submit Lightweight Demand);
        D --> E{Approved by **Team/Business Unit Lead**?};
        E -->|Yes| F[Work added directly to **Team Backlog/Kanban**];
        E -->|No| G[Demand Rejected or Revised];
    end

    subgraph "Path 3: Formal Project Work"
        B -->|"**Project** (Tier 1, 2, or 3)"| H(1. Draft & 2. Submitted);
        H --> I(3. Screening);
        I -->|"Triage by EPMO/EA"| J{Is demand viable, unique, and correctly tiered?};
        J -->|No| G;
        J -->|Yes| K(4. Qualified);
        K -->|"Business case and architectural review are performed. *Rigor increases with each Tier.*"| L(5. Approved);
    end

    subgraph "Governance Decision"
        style L fill:#cde4ff
        L --> M{1. Technology Subcommittee Reviews & Recommends?};
        M -->|No| G;
        M -->|Yes| N{2. Technology Advisory Committee (TAC) Approves Funding?};
        N -->|No| G;
    end

    subgraph "Execution Handoff"
        N -->|Yes| O(6. Completed);
        O --> P[Demand is converted to a formal Project and handed off to **EPMO/Delivery Team**];
    end

    %% Endpoints
    C --> Z([End]);
    F --> Z;
    G --> Z;
    P --> Z;

    %% Styling
    classDef governance fill:#cde4ff,stroke:#0050be,stroke-width:2px;
    class L,M,N governance;
```
