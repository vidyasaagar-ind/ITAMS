# IT Asset Management System (ITAMS)
## Stage 1 – Requirement Gathering Package

**Version:** 1.0
**Status:** Requirement Freeze Approved
**Project Type:** Internal Company Tool

---

# Executive Summary

ITAMS is an enterprise-oriented platform for managing, monitoring, auditing, and tracking IT and non-IT assets. The system is designed to detect unauthorized hardware/software changes, manage asset lifecycles, support maintenance operations, and provide centralized visibility across an organization.

---

# Business Problem Statement

Organizations face challenges including:

- Unauthorized hardware replacement
- Installation of unapproved software
- Missing asset ownership records
- Lack of centralized monitoring
- Poor warranty and AMC tracking
- Incomplete audit trails

ITAMS addresses these problems through centralized governance, monitoring, and reporting.

---

# Stakeholders

## Admin
- Asset management
- User management
- Monitoring
- Approvals
- Reporting
- Audit oversight

## Employee
- View assigned assets
- Raise tickets
- Request maintenance
- Upload supporting files

---

# Functional Requirements

## Authentication & Authorization
- Secure login
- Role-based access control
- Session management
- MFA-ready architecture

## Asset Management
- Create assets
- Update assets
- Assign assets
- Transfer assets
- Reserve assets
- Retire assets
- Dispose assets

## Monitoring Agent
- Startup execution
- Scheduled execution
- Manual execution
- Device registration
- Heartbeat monitoring

## Change Detection
- RAM changes
- Storage changes
- Motherboard changes
- BIOS changes
- Software installation/removal
- Software version changes
- USB insertion
- Unknown login activity
- Agent removal

## Notifications
- Realtime notifications
- Email notifications
- Severity-based alerts

## Ticketing
- Asset requests
- Maintenance requests
- Repair requests
- Software requests
- Asset return requests

## Reports
- Inventory reports
- Audit reports
- Security reports
- Warranty reports
- Vendor reports
- Employee reports

---

# Non-Functional Requirements

## Security
- HTTPS
- Password hashing
- Session timeout
- Access logging
- Device/IP tracking
- Backup support

## Scalability
- 1000+ users
- 10000+ assets
- Multi-branch support

## Performance
- Dashboard response under 3 seconds
- Indexed queries
- Pagination

---

# Asset Categories

- Laptops
- Desktops
- Servers
- Routers
- Switches
- Printers
- Monitors
- Keyboards
- Mouse
- External HDD/SSD
- UPS
- Software Licenses
- Mobile Devices
- Other

---

# Asset Lifecycle

Procurement → Inventory → Reserved → Assigned → Transfer → Maintenance → Return → Retirement → Disposal

---

# Monitoring Strategy

## Scheduled Scans
- Startup scan
- Daily scans

## Event Monitoring
- USB insertion
- Software install/removal
- Login events
- Agent status changes

## Heartbeat
Agent periodically reports health status. Missing heartbeat generates alerts.

---

# Alert Severity

## Critical
- Agent removed
- Agent disabled
- Extended inactivity

## High
- RAM changes
- Disk changes
- Motherboard changes
- BIOS changes
- Unauthorized software

## Medium
- USB insertion
- Network changes

## Low
- Approved software updates

---

# Business Rules

- Every asset must have a unique asset ID.
- Asset history is permanent.
- Audit logs cannot be deleted.
- Agent removal creates a critical alert.
- Employees cannot directly modify official asset records.
- All approvals are audited.

---

# Dashboard Priorities

1. Security Alerts
2. Asset Summary
3. Open Tickets
4. Warranty & AMC Expiry
5. Employee Activity
6. Vendor Metrics
7. Recent Asset Changes
8. Maintenance Schedule
9. Asset Distribution Analytics

---

# Technology Stack

## Frontend
- React
- Vite
- Tailwind CSS

## Backend
- Node.js
- Express.js

## Database
- Supabase PostgreSQL

## Storage
- Supabase Storage

## Monitoring Agent
- Python

---

# Risks

1. Monitoring agent tampering
2. Alert fatigue
3. Inventory data growth
4. Communication security

Mitigations include Windows Service deployment, heartbeat monitoring, severity classification, HTTPS, and secure device registration.

---

# MVP Scope (2 Months)

## Phase 1
- Authentication
- User management
- Dashboard

## Phase 2
- Asset management
- Lifecycle management

## Phase 3
- Monitoring integration
- Change detection
- Notifications

## Phase 4
- Ticketing
- Reporting
- Audit logs
- Deployment

---

# Requirement Freeze

Requirement Gathering Phase completed and approved.
This document serves as the official Stage 1 requirement baseline for Stage 2 Requirement Analysis.
