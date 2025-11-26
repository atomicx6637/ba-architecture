# Energy Consumption Data - Entity Definition
## Quantum Energy

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Definition of key information entities related to energy consumption and metering data
**Related Documents:**
*   [Enterprise Business Information Model - Conceptual (ent-business-information-model.md)](../ent-business-information-model.md)
*   [Metering and Measurement (L1 Cap 9)](../../3-CAPABILITIES/ent-capabilities-l1-l2.md#_9-metering-and-measurement-ent)

---

## Executive Summary

This document defines the key information entities related to energy consumption and metering data at Quantum Energy. This data is fundamental for accurate billing, operational planning, grid management, and providing energy insights to customers across both regulated utility services and non-regulated advanced energy solutions.

---

## 1. Introduction

Energy Consumption Data encompasses all measurements collected from various metering devices (traditional, AMI, smart devices) that quantify the usage of electricity and natural gas. This data forms the basis for revenue generation, operational efficiency analysis, and customer engagement.

---

## 2. Key Information Entities

### 2.1. Meter Point

*   **Definition:** A unique identifier representing the physical point at which energy consumption or generation is measured. A Meter Point is typically associated with a Premise and may have multiple physical Meter assets over time.
*   **Attributes:**
    *   `Meter_Point_ID` (Primary Key)
    *   `Premise_ID` (Foreign Key - links to Premise entity)
    *   `Service_Type` (e.g., "Electric", "Gas")
    *   `Service_Voltage` / `Service_Pressure`
    *   `Meter_Cycle_Route`
    *   `Billing_Determinants` (e.g., demand components, power factor)
    *   `AMI_Capable_Flag`
    *   `Last_Read_Date`
*   **Relationships:**
    *   One-to-one with Premise.
    *   One-to-many with Meter.
    *   One-to-many with Meter Reading.

### 2.2. Meter

*   **Definition:** A unique identifier and record for a physical metering device installed at a Meter Point to measure energy consumption or generation.
*   **Attributes:**
    *   `Meter_ID` (Primary Key)
    *   `Meter_Point_ID` (Foreign Key)
    *   `Manufacturer`
    *   `Model`
    *   `Serial_Number`
    *   `Installation_Date`
    *   `Installation_Type` (e.g., "Standard", "AMI", "Smart Meter")
    *   `Last_Test_Date`
    *   `Status` (e.g., "In Service", "Retired", "Removed")
    *   `Communication_Method` (e.g., "Manual", "RF", "Cellular", "Powerline")
*   **Relationships:**
    *   One-to-one with Meter Point (at any given time).
    *   One-to-many with Meter Reading.

### 2.3. Meter Reading

*   **Definition:** A discrete record of energy consumption or generation measured by a Meter at a specific point in time.
*   **Attributes:**
    *   `Reading_ID` (Primary Key)
    *   `Meter_ID` (Foreign Key)
    *   `Meter_Point_ID` (Foreign Key)
    *   `Timestamp` (Date and Time of reading)
    *   `Reading_Value` (e.g., kWh, Therms, kVA)
    *   `Reading_Type` (e.g., "Actual", "Estimated", "Billed", "Interval")
    *   `Read_Source` (e.g., "Manual", "AMI", "SCADA", "Customer")
    *   `Flags` (e.g., "Estimated", "Suspicious", "Valid")
    *   `Demand_Value` (for electric, if applicable)
    *   `Interval_Duration` (for interval data, e.g., 15 min, 60 min)
*   **Relationships:**
    *   Many-to-one with Meter.
    *   Many-to-one with Meter Point.
    *   Forms the basis for Financial Transactions (billing).

### 2.4. Consumption Profile

*   **Definition:** Aggregated or disaggregated patterns of energy consumption or generation for a Meter Point or Customer Account over a period. This is often derived from Meter Readings.
*   **Attributes:**
    *   `Profile_ID` (Primary Key)
    *   `Meter_Point_ID` (Foreign Key)
    *   `Time_Period` (e.g., "Daily", "Hourly", "Monthly")
    *   `Avg_Consumption`
    *   `Peak_Consumption`
    *   `Load_Factor`
    *   `Creation_Date`
    *   `Last_Update_Date`
    *   `Profile_Type` (e.g., "Load Shape", "Baseline")
*   **Relationships:**
    *   Many-to-one with Meter Point.
    *   Used for Customer Insights & Analytics, grid planning, and personalized offers.

---

## 3. Data Governance Considerations

*   **Accuracy & Reliability:** Critical for billing accuracy, revenue assurance, and grid stability.
*   **Timeliness:** Especially for interval and real-time data, crucial for grid operations and customer insights.
*   **Integrity:** Protection against tampering and unauthorized modification.
*   **Regulatory Compliance:** Adherence to standards for metering, billing, and data retention (e.g., PUC rules on AMI data).
*   **Data Volume:** Management of very large volumes of interval data from AMI and smart devices.
*   **Data Access:** Secure and controlled access to consumption data, balancing operational needs with customer privacy and non-regulated business needs (with consent).
*   **Standardization:** Consistent data formats and definitions across different metering technologies and service types.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Data Governance Council, Metering, Grid Operations, Financial Management, BA Review Board
**Approval:** Chief Data Officer
**Version History:**
- v1.0 (2025-11-25): Initial definition of Energy Consumption Data Entities.

**Next Review:** Annually or upon significant changes to metering technologies or regulatory requirements

---

**End of Document**
