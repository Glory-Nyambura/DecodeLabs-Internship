🛡️ Project 1: Data Quality & Cleaning Report

Internship Assessment Project

🎯 Project Overview

This project executes an end-to-end data audit, validation, and cleaning pipeline on an business transactional dataset containing 1,200 records. Raw transactional data often contains formatting conflicts, empty rows, and structural layout vulnerabilities that break live dashboards. The goal of this phase was to eliminate these flaws and establish absolute format uniformity before processing data for analytics.


📊 Data Quality Summary

*   Total Rows: 1,200 rows verified. 0 duplicate rows found across structural data keys.
*   Exact Duplicate Records: 0 redundant database entries detected during global identity checks.
*   Missing & Null Values: 309 blank rows identified in the `CouponCode` field and successfully resolved.
*   Date Fields: All timeline dates standardized into strict `YYYY-MM-DD` syntax.
*   Numeric Fields: Enforced whole integers for quantities and currency formats for pricing fields.

Column-Level & Cleanup

*   OrderID: Primary Key validated. Ensured alphanumeric structure contains no blank fields.
*   Date: Temporal fields standardized to a uniform date notation to fix variance.
*   CustomerID: System alpha-keys validated against internal database reference indices.
*   Product: Text entries scrubbed to remove hidden trailing and leading white spaces.
*   Quantity: Integer constraints verified to eliminate fractional purchase errors.
*   UnitPrice: Verified as floating-point positive currency layout blocks.
*   ShippingAddress: String fields parsed and unified for logistical analysis.
*   PaymentMethod: Categorical text strings checked against accepted gateway metrics.
*   OrderStatus: Transaction tracking flags verified and mapped uniformly.
*   TrackingNumber: Shipment string layers validated for structural integrity.
*   ItemsInCart: Quantity volume metrics matched to corresponding customer records.
*   CouponCode: Imputed 309 missing inputs with a standard "No Coupon" text marker.
*   ReferralSource: Marketing channel text standardized to optimize source attribution.


🛠️ Data Skills Demonstrated

* Missing Value Imputation: Resolved 309 blank entries in the coupon column, preserving row records without introducing null data blind spots.
* Structural Consistency Audits: Deployed range validation rules to confirm that zero data shifting or data loss occurred between the raw source and final sheet.
