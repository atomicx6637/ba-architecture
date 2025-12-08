# Demand Management Workflow Visual

This document contains a Mermaid diagram illustrating the consolidated demand management workflow for all project types. This version has been rewritten for improved compatibility and rendering.

```mermaid
flowchart TD
    %% Define Node Shapes
    style A rect
    style B rhombus
    style C rect
    style D rect
    style E rhombus
    style F rect
    style G rect
    style H rect
    style I rect
    style J rhombus
    style K rect
    style L rect
    style M rhombus
    style N rhombus
    style O rect
    style P rect
    style Z rect

    %% Define Node Text
    A["Start: Business Idea or Need"]
    B{"What is the nature of the work?"}
    C["Handled by **Operational Incident Process**
    Outside Demand Workflow"]
    D["Submit Lightweight Demand"]
    E{"Approved by
    **Team or Business Unit Lead**?"}
    F["Work added directly to
    **Team Backlog or Kanban**"]
    G["Demand Rejected or Revised"]
    H["1. Draft and 2. Submitted"]
    I["3. Screening"]
    J{"Is demand viable, unique,
    and correctly tiered?"}
    K["4. Qualified"]
    L["5. Approved"]
    M{"1. Technology Subcommittee
    Reviews and Recommends?"}
    N{"2. Technology Advisory Committee TAC
    Approves Funding?"}
    O["6. Completed"]
    P["Demand is converted to a formal Project
    and handed off to **EPMO or Delivery Team**"]
    Z["End"]

    %% Define Connections
    A --> B

    B -->|Break-Fix| C
    B -->|"**Enhancement**
    e.g. less than 50k"| D

    B -->|"**Project**
    Tier 1, 2, or 3"| H

    C --> Z
    
    D --> E
    E -->|Yes| F
    E -->|No| G
    F --> Z
    G --> Z

    H --> I
    I -->|"Triage by EPMO or EA"| J
    J -->|No| G
    J -->|Yes| K
    K -->|"Business case and architectural
    review are performed.
    Rigor increases with each Tier."| L
    
    L --> M
    M -->|No| G
    M -->|Yes| N
    N -->|No| G
    N -->|Yes| O
    
    O --> P
    P --> Z

    %% Styling
    classDef governance fill:#cde4ff,stroke:#0050be,stroke-width:2px;
    class L,M,N governance;
```