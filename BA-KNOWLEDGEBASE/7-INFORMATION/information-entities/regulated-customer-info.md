# Regulated Customer Information - Entity Definition
## Quantum Energy

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Definition of key information entities related to Quantum Energy's regulated customers
**Related Documents:**
*   [Enterprise Business Information Model - Conceptual (ent-business-information-model.md)](../ent-business-information-model.md)
*   [Regulated Customers - Stakeholder Segment](../../5-STAKEHOLDERS/stakeholder-segments/regulated-customers.md)

---

## Executive Summary

This document defines the key information entities related to Quantum Energy's regulated customer base. This information is critical for managing utility services, billing, regulatory compliance, and customer relations for electric and natural gas customers. It focuses on the data required to support core utility operations, distinct from data related to non-regulated offerings.

---

## 1. Introduction

Regulated Customer Information comprises data necessary to identify, serve, and bill customers for their consumption of regulated electric and natural gas services. It also supports compliance with regulatory mandates for customer protection and reporting.

---

## 2. Key Information Entities

### 2.1. Customer Account (Regulated)

*   **Definition:** A unique identifier and record representing a regulated customer's relationship with Quantum Energy for core utility services at a specific premise.
*   **Attributes:**
    *   `Regulated_Account_ID` (Primary Key)
    *   `Customer_ID` (Foreign Key - links to generic Customer entity)
    *   `Premise_ID` (Foreign Key - links to Premise entity)
    *   `Service_Type` (e.g., "Electric", "Gas", "Dual-Fuel")
    *   `Account_Status` (e.g., "Active", "Inactive", "Pending Service")
    *   `Rate_Schedule_ID` (Foreign Key - links to Tariff/Rate Schedule entity)
    *   `Start_Date`
    *   `End_Date` (if applicable)
    *   `Billing_Cycle_Code`
    *   `Service_Address` (Redundant, but often held for quick reference)
    *   `Contact_Preference` (for regulated communications)
    *   `Marketing_Opt_Out` (for regulated programs)
*   **Relationships:**
    *   One-to-many with Customer Profile (a customer can have multiple regulated accounts, e.g., for different premises).
    *   One-to-one with Premise.
    *   One-to-many with Meter Point (multiple meters at a premise/account).
    *   One-to-many with Service Agreement.
    *   One-to-many with Billing & Payment History.

### 2.2. Customer Profile (Regulated)

*   **Definition:** Personal and demographic information identifying the individual or organization responsible for a regulated utility account.
*   **Attributes:**
    *   `Customer_ID` (Primary Key)
    *   `Name` (Individual/Organization Name)
    *   `Tax_ID` / `SSN` (for credit checks, masked)
    *   `Date_of_Birth` / `Formation_Date`
    *   `Mailing_Address`
    *   `Primary_Contact_Phone`
    *   `Primary_Contact_Email`
    *   `Preferred_Language`
    *   `Customer_Type` (e.g., "Residential", "Commercial", "Industrial", "Governmental")
    *   `Credit_Score` (from external agencies, if stored)
    *   `Credit_Rating` (internal)
    *   `Deposit_Required_Flag`
    *   `Vulnerable_Customer_Flag` (e.g., medical, low-income)
*   **Relationships:**
    *   One-to-many with Regulated Customer Account.

### 2.3. Premise

*   **Definition:** The physical location where Quantum Energy provides regulated electric or natural gas service.
*   **Attributes:**
    *   `Premise_ID` (Primary Key)
    *   `Service_Address`
    *   `GIS_Coordinates` (Latitude, Longitude)
    *   `Service_Territory_Zone`
    *   `Feeder_ID` (for electric)
    *   `Pressure_Zone_ID` (for gas)
    *   `Meter_Location_Details`
    *   `Transformer_ID` (for electric)
    *   `Gas_Main_Connection_ID` (for gas)
*   **Relationships:**
    *   One-to-one with Customer Account.
    *   One-to-many with Meter Point.

### 2.4. Service Agreement (Regulated)

*   **Definition:** The formal or implied contract between Quantum Energy and a regulated customer for the provision of utility service.
*   **Attributes:**
    *   `Service_Agreement_ID` (Primary Key)
    *   `Account_ID` (Foreign Key)
    *   `Product_ID` (Foreign Key - links to Regulated Product definitions)
    *   `Start_Date`
    *   `End_Date` (if applicable)
    *   `Terms_and_Conditions_Version`
    *   `Special_Provisions` (e.g., medical certificates, payment arrangements)
*   **Relationships:**
    *   One-to-one with Customer Account.

---

## 3. Data Governance Considerations

*   **Confidentiality:** Strict measures to protect Personally Identifiable Information (PII) and sensitive customer data.
*   **Regulatory Compliance:** Adherence to PUC rules regarding data retention, privacy, and customer access.
*   **Data Accuracy:** High importance placed on accurate customer and premise data for billing and service delivery.
*   **Data Separation:** Clear delineation and audit trails for data used solely for regulated operations versus data that might be shared (with customer consent) for non-regulated offerings.
*   **Master Data Management:** Customer and Premise are key master data entities.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Data Governance Council, Customer Service, Regulatory Affairs, Legal, BA Review Board
**Approval:** Chief Data Officer
**Version History:**
- v1.0 (2025-11-25): Initial definition of Regulated Customer Information Entities.

**Next Review:** Annually or upon significant changes to customer systems or regulatory requirements

---

**End of Document**
