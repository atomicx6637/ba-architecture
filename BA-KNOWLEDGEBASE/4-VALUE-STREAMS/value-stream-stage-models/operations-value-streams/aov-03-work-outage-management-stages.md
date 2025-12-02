# AOV-03: Work & Outage Management - Stages
## Quantum Energy - Detailed Value Stream Stages

**Document Version:** 1.0
**Date:** 2025-12-01
**Scope:** Detailed stages for the Work & Outage Management value stream
**Parent Value Stream:** AOV-03 Work & Outage Management
**Triggering Stakeholder:** Operations (planned work) / Customer (outage)
**Receiving Stakeholder:** The Grid / Restored Customer
**Value Proposition:** Safe, efficient work execution with minimized outage duration (regulated) and timely installation/repair (non-regulated).
**Related Documents:**
*   [Enterprise Value Streams Catalog](../ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document details the stages of the Work & Outage Management value stream (AOV-03). This process describes the end-to-end management of all field-based work, from planned maintenance and construction to the high-pressure environment of unplanned outage restoration. Mastering this value stream is essential for operational efficiency, field force productivity, customer satisfaction, and public safety.

---

## 1. Value Stream Context

**Value Stream ID:** AOV-03
**Name:** Work & Outage Management
**Description:** Plan, schedule, and execute field work activities including maintenance, construction, and outage response for both regulated infrastructure and non-regulated installations.

**Entry Criteria:**
-   A work request is generated (e.g., from asset management system, new customer connect).
-   An unplanned event or outage occurs and is detected.
-   Resources (crews, materials) are available for dispatch.

**Exit Criteria:**
-   The planned or corrective work is completed successfully and safely.
-   The asset is returned to service or the new service is activated.
-   If an outage occurred, all customers are restored.
-   All work and cost information is documented and closed out.

---

## 2. Value Stream Stages and Enabling Capabilities

| Stage ID | Stage Name | Description | Enabling Capabilities (L2 Examples) | Expected Inputs | Expected Outputs | Key Metrics |
| :------- | :--------- | :---------- | :---------------------------------- | :-------------- | :--------------- | :---------- |
| **AOV-03.1** | **Work & Event Initiation** | Receive or generate a work request from various sources (asset management, customer request, outage event) and create a formal work order. | *   12.3 Asset Maintenance & Work Management | Work request, Outage alert, Customer call | Validated work order, Outage event record | Work order creation time, Outage detection time |
| | | | *   13.6 Outage & Disturbance Management | | | |
| **AOV-03.2** | **Work Planning & Design** | For planned work, create a detailed work package including engineering designs, material lists, and required permits. For outages, assess damage and form a restoration plan. | *   12.4 Engineering & Design | Work order | Work package, Restoration plan, Estimated restoration time (ETR) | Planning cycle time, Design accuracy |
| **AOV-03.3** | **Work Scheduling & Resource Assignment** | Prioritize and schedule the work based on criticality and available resources. Assign specific crews, vehicles, and materials to the work order. | *   10.2 Field Service & Work Management | Work packages, Crew availability | Master work schedule, Assigned work orders | Schedule adherence, Resource utilization |
| **AOV-03.4** | **Dispatch & Field Execution** | Dispatch the scheduled work to the field crews. Crews travel to the site and execute the work safely and efficiently according to the work package. | *   10.2 Field Service & Work Management | Dispatched work order | In-progress work, Field status updates | Travel time, Wrench time, Safety incidents |
| **AOV-03.5** | **Real-Time Monitoring & Support** | Monitor the progress of field work in real-time. Provide support to crews by resolving issues, adjusting schedules, and communicating status to stakeholders. | *   13.2 Real-Time System Monitoring & Analysis | Field status updates | Updated work status, Resolved field issues | Schedule adjustments, Crew support time |
| **AOV-03.6** | **Work Completion & Service Restoration** | The crew completes the work, tests the asset, and reports completion. For outages, service is restored to customers, and notifications are sent. | *   10.2 Field Service & Work Management | Completed field tasks | In-service asset, Restored customers | Restoration time (CAIDI/SAIDI), Customer notifications sent |
| **AOV-03.7** | **Work Closeout & As-Built Documentation** | Close the work order, record as-built information, reconcile materials used, and capture all costs. This information updates the asset records. | *   12.3 Asset Maintenance & Work Management | Completed work order | Closed work order, Updated asset records, Financial actuals | Work order closeout time, Data accuracy |

---

## 3. Cross-Value Stream Dependencies

*   **AOV-03** is the primary execution arm for maintenance work planned in **AOV-01 Asset Lifecycle Management**.
*   It executes the construction activities for **AOV-02 Capital Project Delivery**.
*   It is the core process for restoring service, which is tracked by **AOV-06 System Reliability & Emergency Response**.
*   New customer connections in **RCV-01 Regulated Customer Acquisition** and installations for **NCV-01, NCV-02, NCV-03** all trigger work in this value stream.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Field Operations Leadership, System Control, Asset Management, BA Working Group
**Approval:** Chief Operations Officer (COO)
**Version History:**
- v1.0 (2025-12-01): Initial detailed stage model for AOV-03.

**Next Review:** Annually or upon major changes in work management or field technologies.

---

**End of Document**
