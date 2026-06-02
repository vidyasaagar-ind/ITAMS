# ITAMS - Business Requirements Document (BRD)
## Enterprise Requirement Baseline

**Project:** IT Asset Management System (ITAMS)  
**Document Type:** Business Requirements Document (BRD)  
**Version:** 1.0  
**Status:** Approved Requirement Baseline  
**Prepared During:** Stage 1 & Stage 1.5

---

# 1. Document Purpose

This document captures the approved business requirements, scope, stakeholders, business rules, risks, constraints, and functional expectations for the IT Asset Management System (ITAMS).

This BRD serves as the official baseline for:
- Requirement Analysis
- SRS Preparation
- Architecture Design
- Database Design
- Sprint Planning
- Development
- Testing

---

# 2. Project Overview

ITAMS is an enterprise-focused platform for managing, monitoring, auditing, tracking, securing, and maintaining organizational assets.

The system will support both IT and non-IT assets while providing automated monitoring through a Windows-based endpoint agent.

---

# 3. Business Objectives

## Primary Objectives

- Centralized asset inventory
- Hardware change detection
- Software compliance monitoring
- Asset lifecycle management
- Audit readiness
- Vendor management
- Maintenance management
- Employee accountability

## Secondary Objectives

- Future AI analytics readiness
- Automation readiness
- Enterprise scalability
- Multi-branch support

---

# 4. Stakeholder Analysis

## Asset Administrators
Responsible for inventory governance and compliance.

## IT Administrators
Responsible for monitoring, security, and maintenance.

## Employees
Consume assets and raise requests/tickets.

## Management
Consumes reports and analytics.

## Auditors
Review logs, compliance records, and asset history.

---

# 5. Project Scope

## In Scope

### Organizational Management
- Branchs
- Departments
- Employees

### Asset Operations
- Asset registration
- Assignment
- Transfer
- Reservation
- Return
- Disposal
- Retirement

### Monitoring
- Hardware inventory
- Software inventory
- Event monitoring
- Compliance monitoring

### Service Management
- Tickets
- Approvals
- Maintenance requests

### Reporting
- Security reports
- Audit reports
- Compliance reports
- Financial reports

## Out of Scope (Current Version)

- Mobile applications
- AI analytics implementation
- Knowledge base module
- Linux/macOS monitoring agents

---

# 6. User Roles

## Admin

Permissions:
- Full access
- User management
- Asset management
- Monitoring
- Approvals
- Reports
- Audit access

## Employee

Permissions:
- View assigned assets
- View notifications
- Raise tickets
- Upload documents
- Request changes

---

# 7. Functional Requirements

## FR-001 Authentication

Users shall authenticate securely.

## FR-002 Authorization

System shall support role-based access control.

## FR-003 Asset Registration

System shall allow creation of asset records.

## FR-004 Asset Assignment

System shall support assignment of assets to employees.

## FR-005 Asset Transfer

System shall support transfers between employees and departments.

## FR-006 Asset Reservation

System shall support reservation workflows.

## FR-007 Monitoring Agent Registration

System shall register monitoring agents.

## FR-008 Hardware Monitoring

System shall collect hardware inventory.

## FR-009 Software Monitoring

System shall collect software inventory.

## FR-010 Change Detection

System shall detect hardware and software changes.

## FR-011 Ticket Management

System shall support ticket lifecycle management.

## FR-012 Approval Workflow

System shall support approval and rejection workflows.

## FR-013 Audit Logging

System shall maintain immutable audit records.

## FR-014 Compliance Dashboard

System shall provide compliance visibility.

## FR-015 Vendor Management

System shall maintain vendor records.

## FR-016 Warranty Management

System shall track warranty periods.

## FR-017 AMC Management

System shall track AMC contracts.

## FR-018 Contract Management

System shall track vendor contracts.

## FR-019 Financial Tracking

System shall maintain asset cost information.

## FR-020 Asset Timeline

System shall maintain complete asset history.

---

# 8. Non-Functional Requirements

## NFR-001 Security

- HTTPS
- Password hashing
- MFA-ready architecture
- Session timeout

## NFR-002 Scalability

- 1000+ users
- 10000+ assets

## NFR-003 Availability

- Backup support
- Recovery planning

## NFR-004 Performance

- Dashboard response < 3 seconds

## NFR-005 Maintainability

- Modular architecture
- Clean API design

---

# 9. Business Rules

BR-001 Every asset must have a unique asset identifier.

BR-002 Audit logs cannot be deleted.

BR-003 Asset history must be preserved.

BR-004 Agent removal generates critical alerts.

BR-005 Employees cannot directly modify official asset records.

BR-006 All approvals must be audited.

BR-007 Company-owned devices are monitored.

BR-008 Personal computers are not monitored.

---

# 10. User Stories

### Asset Assignment
As an Admin, I want to assign assets to employees so that ownership is tracked.

### Ticket Creation
As an Employee, I want to raise maintenance requests so that issues are resolved.

### Compliance Monitoring
As an Admin, I want to receive alerts when hardware changes occur so that security risks are investigated.

### Warranty Tracking
As an Admin, I want expiry alerts so that assets remain covered.

---

# 11. Asset Lifecycle

Procurement
→ Inventory
→ Reserved
→ Assigned
→ Transfer
→ Maintenance
→ Return
→ Retirement
→ Disposal

---

# 12. Monitoring Requirements

## Agent Type
Windows-only monitoring agent.

## Collection Modes
- Startup scan
- Scheduled scan
- Manual scan
- Event-based monitoring

## Events
- RAM changes
- Storage changes
- BIOS changes
- Software installation
- Software removal
- USB insertion
- Login events
- Agent status events

---

# 13. Dashboard Requirements

Priority Widgets:
1. Security Alerts
2. Asset Summary
3. Open Tickets

Secondary Widgets:
4. Warranty & AMC Expiry
5. Employee Activity
6. Vendor Metrics

Additional Widgets:
7. Asset Changes
8. Maintenance Schedule
9. Distribution Analytics

---

# 14. Risk Register

## R-001 Agent Tampering
Mitigation: Heartbeat monitoring.

## R-002 Alert Fatigue
Mitigation: Severity classification.

## R-003 Data Growth
Mitigation: Delta storage approach.

## R-004 Communication Security
Mitigation: HTTPS and device registration.

---

# 15. Assumptions

- Organization owns monitored devices.
- Internet connectivity exists periodically.
- Windows is the primary operating system.
- Employees cooperate with asset governance policies.

---

# 16. Constraints

- Team size: 2 developers.
- Budget: Prototype / minimal cost.
- Delivery target: ~2 months.
- Existing monitoring script available.

---

# 17. Requirement Traceability Matrix (High Level)

| Business Need | Requirement |
|--------------|------------|
| Asset Visibility | FR-003, FR-004 |
| Security Monitoring | FR-008, FR-009, FR-010 |
| Service Operations | FR-011, FR-012 |
| Compliance | FR-013, FR-014 |
| Vendor Control | FR-015, FR-016, FR-017 |
| Financial Tracking | FR-019 |
| Lifecycle Tracking | FR-020 |

---

# 18. Requirement Freeze Record

Stage 0: Completed

Stage 1: Completed

Stage 1.5: Completed

Requirement Maturity Score: 98/100

Approved baseline for Stage 2 Requirement Analysis.
