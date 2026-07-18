# Business Requirements — Uber Ride Analytics Dashboard

## Context

Uber's operations team needs visibility into booking performance, revenue, cancellations, and demand patterns across vehicle types and locations. This document defines the KPIs and report structure used to scope the Power BI build.

## Objectives

- Track booking volume and completion rate over time.
- Identify revenue drivers by vehicle type, payment method, and customer.
- Understand why rides are cancelled or left incomplete, and by whom (customer vs. driver).
- Surface location- and time-based demand patterns.
- Segment riders by frequency (first-time, returning, regular).

## Page-by-page requirements

### 1. Overview
**KPIs:** Completed Bookings, Lost Bookings, Revenue, Total Distance, Average Distance.

**Breakdowns:**
- Monthly trend — bookings completed, revenue
- Quarterly trend — bookings completed, revenue
- Revenue by vehicle type
- Top pickup and drop locations by booking count
- Average rider rating, average driver rating

**Filters:** Vehicle type.

### 2. Vehicle
Detail view by vehicle type: booking count, revenue, and revenue contribution.

### 3. Revenue
Revenue broken down by customer, vehicle type, and payment method, viewed monthly and quarterly.

### 4. Rider
- Cancelled rides by reason
- Cancellations by payment method
- Monthly and quarterly cancellation trends
- Detail table segmenting riders into First Rider, Return Rider, Regular Rider

### 5. Location
- Total distance by month
- Total distance by vehicle type
- Busiest time slots
- Busiest pickup/drop areas

## Cross-page requirements

- Collapsible filter panel on every page to preserve screen space.
- Consistent slicers across pages (vehicle type, month, time slot, payment method, pickup/drop location) so filtering carries through the report.
- Bookmark-based navigation between pages.

## Out of scope

- Real-time or API-connected data (this report runs on a static dataset snapshot).
- Predictive/forecasting models — the report is descriptive, not predictive.
