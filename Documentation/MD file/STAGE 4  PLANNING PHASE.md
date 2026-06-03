**STAGE 4 — PLANNING PHASE**

**Project Execution Strategy**

**Team Structure**

**Developer 1 (You)**

Primary Ownership:

Frontend  
UI/UX  
Dashboard  
Asset Management  
Reports  
Testing

Secondary:

Backend APIs  
Database Review

**Developer 2 (Friend)**

Primary Ownership:

Python Monitoring Agent  
FastAPI Monitoring Service  
Change Detection  
Heartbeat Engine  
Agent Packaging

Secondary:

Backend APIs  
Database Review

**Timeline Analysis**

**Total Duration**

8 Weeks

**Constraint**

Semester Exams until June 16

This means:

**Week 1**

Reduced productivity.

**Weeks 2-8**

Full development pace.

**Critical Path Analysis**

The entire project depends on these items:

Authentication  
↓  
Organization Structure  
↓  
Asset Management  
↓  
Monitoring Agent  
↓  
Snapshot Processing  
↓  
Change Detection  
↓  
Alerts  
↓  
Reports

If Monitoring Agent slips,  
the entire product value drops significantly.

Therefore:

Monitoring Agent =Priority #1

**Final MVP Definition**

Must work by release:

**Core Platform**

- Authentication
- Multi-company structure
- Branch management
- Department management
- Employee management

**Asset Management**

- Asset CRUD
- Assignment
- Transfer
- Return
- Disposal

**Monitoring**

- Device registration
- Hardware collection
- Software collection
- Heartbeat
- Snapshot upload

**Security**

- Change detection
- Risk classification
- Alert generation

**Operations**

- Ticketing
- Approval workflow

**Governance**

- Audit logs
- Reports

**Maintenance**

- Vendor management
- Warranty tracking
- AMC tracking

**Sprint Roadmap**

**Sprint 0**

Duration:

3 Days

Goal:

Foundation Setup

Tasks:

- Git repository
- Project structure
- Coding standards
- Supabase project
- Environment setup
- Authentication setup

Deliverable:

Login Working  
Project Running

**Sprint 1**

Duration:

Week 1

Goal:

Organization Foundation

Modules:

- Company
- Branch
- Department
- Employee

Frontend:

- Layout
- Sidebar
- Navbar

Backend:

- CRUD APIs

Deliverable:

Organization Management Complete

**Sprint 2**

Duration:

Week 2

Goal:

Asset Management Core

Modules:

- Asset CRUD
- Categories
- Asset Images
- Assignment

Deliverable:

Asset Inventory Working

**Sprint 3**

Duration:

Week 3

Goal:

Monitoring Agent MVP

Agent:

- Registration
- Authentication
- Snapshot Upload

Backend:

- Agent APIs

Database:

- Monitoring tables

Deliverable:

Device Successfully Registered

**Sprint 4**

Duration:

Week 4

Goal:

Change Detection Engine

Modules:

- Snapshot Comparison
- Event Generation
- Alert Generation

Deliverable:

Hardware Changes Detected

**Sprint 5**

Duration:

Week 5

Goal:

Ticketing + Approvals

Modules:

- Tickets
- Approval Engine

Deliverable:

Request Workflow Working

**Sprint 6**

Duration:

Week 6

Goal:

Maintenance Management

Modules:

- Vendors
- Warranty
- AMC

Deliverable:

Maintenance Tracking Working

**Sprint 7**

Duration:

Week 7

Goal:

Reports + Audit Logs

Modules:

- Audit Trail
- Asset Reports
- Security Reports

Deliverable:

Governance Features Complete

**Sprint 8**

Duration:

Week 8

Goal:

Stabilization

Tasks:

- Bug fixing
- Security review
- Performance review
- UAT

Deliverable:

Release Candidate

**Repository Structure**

Approved:

ITAMS/

├── frontend/

├── backend-express/

├── monitoring-service/

├── agent/

├── docs/

├── database/

└── deployment/

**Major Risks**

**Risk 1**

Monitoring Agent Complexity

Impact:

Very High

Mitigation:

Build by milestones:

Collect  
↓  
Upload  
↓  
Register  
↓  
Heartbeat  
↓  
Compare

Never attempt everything at once.

**Risk 2**

Overbuilding Dashboard

Impact:

Medium

Mitigation:

Functional first.  
Visual polish later.

**Risk 3**

Database Redesign

Impact:

High

Mitigation: Complete Stage 5 Database Design before coding.

**AI Development Strategy**

**Use Anti-Gravity AI For**

- Full feature implementation
- Refactoring
- UI generation
- API generation

**Use Codex For**

- Bug fixing
- Database queries
- Small features
- Validation