**STAGE 3 — SOFTWARE REQUIREMENT SPECIFICATION (SRS)**

**Document Information:**

| **Item** | **Value** |
| --- | --- |
| Project Name | IT Asset Management System (ITAMS) |
| Document Type | Software Requirement Specification |
| Version | 1.0 |
| Status | Approved |
| Project Type | Enterprise Internal Tool |
| Architecture | Hybrid Deployment |
| Authentication | Supabase Auth |
| Multi-Tenant | Supported |

**1\. Introduction:**

**1.1 Purpose**

The purpose of ITAMS is to provide organizations with a centralized platform for:

- Asset inventory management
- Endpoint monitoring
- Security compliance
- Asset lifecycle management
- Maintenance management
- Vendor management
- Audit and reporting

**1.2 Scope**

The system will manage:

**IT Assets**

- Laptops
- Desktops
- Servers
- Routers
- Switches
- Printers
- UPS
- Monitors

**Non-IT Assets**

- Keyboards
- Mouse
- External Storage
- Accessories
- Other Company Assets

**1.3 Product Vision**

Provide an enterprise-grade alternative to:

- Zoho Asset Management
- ManageEngine AssetExplorer
- Freshservice Assets
- Snipe-IT

while incorporating endpoint monitoring and change detection capabilities.

**2\. System Overview:**

The solution consists of five major subsystems.

**Subsystem 1**

**Asset Management Platform**

Functions:

- Asset registration
- Asset assignment
- Asset transfers
- Asset disposal

**Subsystem 2**

**Monitoring Agent**

Functions:

- Hardware inventory collection
- Software inventory collection
- Device health reporting
- Heartbeat reporting

**Subsystem 3**

**Compliance & Security Engine**

Functions:

- Change detection
- Risk classification
- Compliance scoring
- Alert generation

**Subsystem 4**

**Service Management**

Functions:

- Ticketing
- Maintenance requests
- Approval workflows

**Subsystem 5**

**Reporting & Analytics**

Functions:

- Audit reports
- Security reports
- Asset reports
- Vendor reports
- Financial reports

**3\. Stakeholders:**

**Primary:**

**System Administrator**

Full access.

**Asset Manager**

Asset operations.

**Employee**

Self-service operations.

**Secondary:**

**Management**

Analytics and reporting.

**Auditors**

Compliance verification.

**Vendors**

Maintenance and support.

**4\. User Roles:**

**Super Admin**

Permissions:

- Company management
- Tenant management
- System configuration

**Admin**

Permissions:

- Asset management
- Monitoring
- Approvals
- Reporting

**Employee**

Permissions:

- View assigned assets
- Raise tickets
- Submit requests
- View notifications

**5\. Functional Requirements**

**Authentication**

**FR-001:** Users shall authenticate through Supabase Authentication.

**FR-002:** System shall support password reset.

**FR-003:** System shall support MFA-ready authentication.

**Organization Management**

**FR-004:** System shall support multi-company management.

**FR-005:** System shall support branch management.

**FR-006:** System shall support department management.

**User Management**

**FR-007:** System shall support employee management.

**FR-008:** System shall support role assignment.

**Asset Management**

**FR-009:** Create asset.

**FR-010:** Update asset.

**FR-011:** Assign asset.

**FR-012:** Transfer asset.

**FR-013:** Reserve asset.

**FR-014:** Return asset.

**FR-015:** Retire asset.

**FR-016:** Dispose asset.

**FR-017:** Upload asset images.

**FR-018:** Manage asset relationships.

**FR-019:** Manage asset tags.

**FR-020:** Maintain asset timeline.

**Monitoring Agent**

**FR-021:** Register device.

**FR-022:** Authenticate agent.

**FR-023:** Transmit heartbeat.

**FR-024:** Upload hardware inventory.

**FR-025:** Upload software inventory.

**FR-026:** Upload network inventory.

**FR-027:** Support manual scans.

**FR-028:** Support scheduled scans.

**Change Detection**

**FR-029:** Detect RAM changes.

**FR-030:** Detect storage changes.

**FR-031:** Detect motherboard changes.

**FR-032:** Detect BIOS changes.

**FR-033:** Detect software installation.

**FR-034:** Detect software removal.

**FR-035:** Detect software version changes.

**FR-036:** Detect USB activity.

**FR-037:** Detect unknown device activity.

**FR-038:** Detect agent removal.

**Ticketing**

**FR-039:** Create tickets.

**FR-040:** Assign tickets.

**FR-041:** Update ticket status.

**FR-042:** Close tickets.

**Approval Workflow**

**FR-043:** Asset assignment approval.

**FR-044:** Asset transfer approval.

**FR-045:** Maintenance approval.

**FR-046:** Asset disposal approval.

**FR-047:** Employee modification request approval.

**Vendor Management**

**FR-048:** Manage vendors.

**FR-049:** Manage contracts.

**FR-050:** Track SLAs.

**FR-051:** Track warranty.

**FR-052:** Track AMC.

**Financial Management**

**FR-053:** Track purchase cost.

**FR-054:** Track depreciation.

**FR-055:** Track ownership cost.

**Reporting**

**FR-056:** Asset reports.

**FR-057:** Compliance reports.

**FR-058:** Audit reports.

**FR-059:** Security reports.

**FR-060:** Vendor reports.

**FR-061:** Financial reports.

**6\. Non-Functional Requirements**

**Security**

**NFR-001:** All communication shall use HTTPS.

**NFR-002:** Passwords shall never be stored locally.

**NFR-003:** Role-based access control shall be enforced.

**NFR-004:** Audit logging shall be immutable.

**Performance**

**NFR-005:** Dashboard response < 3 seconds.

**NFR-006:** Pagination required for large datasets.

**Scalability**

**NFR-007:** Support 1000+ users.

**NFR-008:** Support 10000+ assets.

**NFR-009:** Support 1000+ monitoring agents.

**Availability**

**NFR-010:** Daily backups.

**NFR-011:** Recovery procedures documented.

**7\. Security Requirements**

**Authentication Security**

- Supabase Auth
- Session timeout
- MFA-ready design

**Agent Security**

- Device registration
- Agent tokens
- Device fingerprinting
- Heartbeat validation

**Audit Security**

- Immutable logs
- User activity tracking
- Change tracking

**8\. Business Rules**

**BR-001:** Every asset shall have a unique Asset ID.

**BR-002:** Audit logs shall not be deleted.

**BR-003:** Asset history shall be preserved permanently.

**BR-004:** Agent inactivity >72 hours shall trigger Critical Risk alerts.

**BR-005:** Agent removal shall trigger Critical Risk alerts.

**BR-006:** Employees cannot directly modify official asset records.

**BR-007:** All approvals shall be logged.

**9\. User Flow Summary**

**Asset Assignment Flow:**

Admin  
↓  
Select Asset  
↓  
Assign Employee  
↓  
Employee Acknowledges  
↓  
Assignment Recorded

**Monitoring Flow:**

Agent Scan  
↓  
Upload Snapshot  
↓  
Compare Snapshot  
↓  
Generate Events  
↓  
Generate Alerts  
↓  
Display Dashboard

**Ticket Flow:**

Employee  
↓  
Create Ticket  
↓  
Admin Review  
↓  
Work In Progress  
↓  
Resolved  
↓  
Closed

**10\. Constraints**

- Budget constrained prototype
- Team size: 2
- Development period: ~2 months
- Windows-only monitoring agent (MVP)

**11\. Future Scope**

**Phase 2**

- Knowledge Base
- N8N Automation
- Advanced Procurement
- Advanced License Compliance
- Asset Health Score

**Phase 3**

- Linux Agent
- macOS Agent
- Mobile Application
- SaaS Commercialization