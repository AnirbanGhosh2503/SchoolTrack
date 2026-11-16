# FEASIBILITY STUDY

**Project:** SchoolTrack – RFID-Based Student Movement Management System  
**Document ID:** ST-FS-001  
**Version:** 0.1  
**Status:** Preliminary Assessment  
**Prepared By:** Anirban Ghosh and Satyajit Moitra  
**Date:** 16 November 2026

---

## 1. Introduction

A feasibility study is conducted to evaluate whether a proposed project can be successfully developed, implemented and maintained within its technical, economic, operational, legal and scheduling constraints.

The purpose of this study is to assess the feasibility of developing SchoolTrack, an RFID-based Student Movement Management System intended to provide an educational institution with independent control over its student movement records.

The proposed solution involves the integration of RFID identification hardware, embedded systems, communication infrastructure, database management and a web-based administrative application.

The system is initially intended to accommodate approximately 2,000 students.

This document evaluates the proposed system across five major dimensions of feasibility and identifies the conditions that must be addressed before proceeding with full-scale development and deployment.

## 2. Technical Feasibility

Technical feasibility evaluates whether the required hardware, software, infrastructure and technical expertise are available or can reasonably be acquired to develop the proposed system.

### 2.1 Proposed System Components

The proposed architecture consists of the following components:

1. RFID identification hardware.
2. Embedded controllers and firmware.
3. Device communication infrastructure.
4. Backend application and APIs.
5. Centralised database.
6. Web-based administrative interface.
7. Reporting and data export modules.
8. Authentication and access control mechanisms.

### 2.2 Hardware Feasibility

The system will require RFID readers capable of identifying registered student cards at designated checkpoints.

The anticipated hardware components include:

- RFID cards or tags.
- RFID readers.
- Microcontrollers or embedded controllers.
- Communication modules.
- Power supply units.
- Local storage or buffering facilities, where required.
- Supporting electronic components and enclosures.

Hardware selection will depend on the existing RFID infrastructure, compatibility requirements, reading range, communication protocols, operating environment and procurement costs.

Particular attention must be given to bus-mounted devices, which may experience intermittent internet connectivity and varying power conditions.

**Preliminary Assessment:** Conditionally Feasible.

**Pending Investigation:**
- Existing RFID card technology.
- Reader models and communication interfaces.
- Existing hardware compatibility.
- Hardware procurement requirements.
- Power and network availability.

### 2.3 Software Feasibility

The software system is expected to consist of several independent but integrated modules.

| Module | Proposed Responsibility |
|---|---|
| Student Management | Student records and class assignments |
| RFID Management | Card registration and assignment |
| Device Management | Reader identification and monitoring |
| Movement Management | Recording and retrieving RFID events |
| Transportation Management | Bus, route and trip information |
| User Management | Authentication and access control |
| Reporting | Attendance and movement reports |
| Data Export | CSV, Excel and PDF generation |
| Audit Management | Recording important administrative activities |

An additional Academic Attendance Management module may be considered in a future development phase.

### 2.4 Database Feasibility

The database must accommodate student information, RFID card assignments, movement events, transportation records and administrative information.

The anticipated student population is approximately 2,000.

The database design must support:

- Unique student identification.
- Efficient retrieval of student movement history.
- Relationship management between students, classes and RFID cards.
- Timestamp-based event queries.
- Bus-wise and route-wise movement records.
- Historical reporting.
- Backup and recovery.
- Appropriate access restrictions.

MongoDB and PostgreSQL are identified as candidate database technologies.

A comparative evaluation will be performed before final selection, considering data relationships, querying requirements, reporting complexity, scalability and maintenance.

### 2.5 Application Architecture Feasibility

A modular architecture is proposed to separate the hardware communication layer, backend services, database and frontend application.

The initial architectural candidates include:

- Backend: Python FastAPI or Node.js.
- Frontend: React.
- Database: MongoDB or PostgreSQL.
- API Communication: REST.
- Cloud Infrastructure: MongoDB Atlas or an equivalent managed infrastructure.
- Version Control: Git and GitHub.

Final technology selection will be documented in the System Design phase.

### 2.6 Infrastructure Feasibility

Three possible deployment architectures have been identified.

**A. Cloud-Based Architecture**

The application and database will be hosted on cloud infrastructure, allowing authorised users to access the system remotely.

Advantages:
- Remote accessibility.
- Centralised data storage.
- Reduced local server maintenance.
- Easier remote administration.

Limitations:
- Dependence on internet connectivity for real-time access.
- Recurring hosting expenses.
- Dependence on external infrastructure providers.

**B. School-Hosted Architecture**

The application and database will operate on a server located within the institution.

Advantages:
- Local accessibility without internet connectivity.
- Direct control over physical infrastructure.
- Reduced dependence on external cloud hosting.

Limitations:
- Hardware maintenance.
- Local backup and disaster recovery responsibilities.
- Additional requirements for secure remote access.
- Dependence on local power and network availability.

**C. Hybrid Architecture**

The system will use local device-level event buffering combined with centralised cloud storage and synchronisation.

Advantages:
- Temporary offline operation.
- Remote access to synchronised records.
- Reduced risk of event loss during connectivity interruptions.
- Greater flexibility in device communication.

Limitations:
- Increased implementation complexity.
- Synchronisation and duplicate-event handling requirements.
- Additional monitoring and maintenance.

The hybrid architecture is recommended for further technical investigation, but final selection will depend on hardware capabilities, infrastructure availability and institutional preferences.

### 2.7 Technical Expertise

The development team has complementary technical responsibilities.

| Team Member | Primary Technical Responsibility |
|---|---|
| Anirban Ghosh | Database design, backend development, application software and documentation |
| Satyajit Moitra | Hardware design, embedded systems, firmware and hardware integration |

Both members will participate in architectural decisions, testing and integration.

Additional technical consultation may be necessary for networking, cloud deployment, security and specialised RFID hardware.

### 2.8 Technical Feasibility Assessment

**Status: Conditionally Feasible.**

The proposed technologies and development approach are technically achievable. However, final feasibility depends on hardware compatibility, infrastructure availability, communication reliability and successful hardware-software integration.

---

## 3. Economic Feasibility

Economic feasibility evaluates whether the anticipated benefits of the project justify the development, deployment and maintenance expenditure.

### 3.1 Initial Development Costs

Potential initial expenses include:

- RFID readers and cards.
- Microcontrollers and electronic components.
- Supporting communication modules.
- Development and testing equipment.
- Server or cloud infrastructure setup.
- Networking equipment.
- Installation and integration.
- Deployment and staff training.

### 3.2 Recurring Operational Costs

Potential recurring expenses include:

- Cloud hosting and database services.
- Internet connectivity.
- Hardware maintenance.
- Replacement of damaged RFID cards.
- Device replacement and repairs.
- Backup infrastructure.
- Software maintenance.

### 3.3 Software and Infrastructure Costs

The project may utilise open-source development technologies and tools to minimise licensing expenses.

Potential technologies include:

- Python.
- FastAPI.
- React.
- PostgreSQL or MongoDB.
- Git and GitHub.
- Open-source testing frameworks.

Cloud infrastructure expenses will depend on the selected provider, deployment region, storage requirements, compute resources, backups and network traffic.

MongoDB Atlas provides different deployment and pricing options, including a free tier for learning and experimentation. Production deployment will require a separate assessment of appropriate service tiers and operational requirements. <Cite refs={["turn523446search0"]}/>

### 3.4 Economic Benefits

The anticipated benefits include:

1. Reduced dependency on external data management services.
2. Improved administrative efficiency.
3. Reduced manual effort in retrieving attendance and movement records.
4. Centralised access to institutional information.
5. Improved reporting and record retrieval.
6. Reduced time spent preparing administrative reports.
7. Greater flexibility in managing institutional requirements.
8. Potential reduction in long-term operational dependency on external service providers.

If the proposed Academic Attendance Management module is approved, additional benefits may include reduced manual classroom attendance recording and automated preparation of monthly attendance reports.

These benefits will require validation before being included in a formal cost-benefit calculation.

### 3.5 Cost-Benefit Analysis

A numerical cost-benefit analysis cannot yet be completed because hardware specifications, procurement prices, hosting requirements, existing infrastructure and deployment costs are unknown.

A detailed financial assessment will be conducted after hardware evaluation and infrastructure selection.

### 3.6 Economic Feasibility Assessment

**Status: Undetermined.**

The project may be economically viable, particularly if existing hardware can be reused and open-source technologies are adopted.

However, final economic feasibility depends on the estimated initial investment and recurring operational expenses.

---

## 4. Operational Feasibility

Operational feasibility evaluates whether the proposed system can function effectively within the institution's existing administrative and operational environment.

### 4.1 Institutional Compatibility

The proposed system is intended to support the institution's existing student identification and movement monitoring requirements.

The primary operational stakeholder is the School Office, which initiated the replacement proposal.

The system is expected to support approximately two to four operational cycles daily, corresponding to different academic schedules, including Pre-Primary and Primary–High School operations.

### 4.2 User Accessibility

A web-based dashboard is proposed to provide authorised personnel with access to relevant information.

The interface should support:

- Student record retrieval.
- RFID card management.
- Movement history.
- Bus-wise records.
- Attendance-related reports.
- Search and filtering.
- Data export.

The interface should be sufficiently simple for administrative personnel without requiring specialised technical knowledge.

### 4.3 Administrative Workflow

The proposed workflow is:

1. Register student information.
2. Assign an RFID card to the student.
3. Configure RFID readers and operational locations.
4. Record RFID events.
5. Transmit events to the central application.
6. Store and process movement information.
7. Provide authorised users with searchable records and reports.

### 4.4 Operational Reliability

The system must consider the following operational challenges:

- Temporary internet interruptions.
- Hardware malfunction.
- Duplicate RFID scans.
- Unregistered or invalid RFID cards.
- Lost or damaged cards.
- Missing movement events.
- Incorrect student information.
- Device synchronisation failures.

Appropriate exception handling, event buffering, device monitoring and administrative correction mechanisms should be incorporated.

### 4.5 Training and Maintenance

Administrative personnel and other authorised users will require basic training.

Technical documentation and user manuals should be provided.

The institution should also establish responsibility for:

- User account management.
- Student record maintenance.
- RFID card assignment.
- Device monitoring.
- Database backups.
- Hardware maintenance.
- Incident handling.

### 4.6 Operational Feasibility Assessment

**Status: Conditionally Feasible.**

The proposed system aligns with the institution's identified operational requirements.

Successful implementation will depend on user acceptance, reliable hardware operation, appropriate training and clearly assigned administrative responsibilities.

---

## 5. Legal Feasibility

Legal feasibility evaluates whether the proposed system can operate in accordance with applicable laws, regulations and institutional policies.

Since the proposed application will process personal information relating to schoolchildren, data protection and privacy are particularly important considerations.

### 5.1 Applicable Regulatory Framework

The project must consider the following:

- Digital Personal Data Protection Act, 2023.
- Digital Personal Data Protection Rules, 2025.
- Applicable contractual and institutional data management requirements.
- Other applicable laws and regulations concerning information security and privacy.

The DPDP Act and Rules have staggered commencement provisions. The applicable obligations must therefore be reviewed against the intended deployment date.

### 5.2 Children's Personal Data

The system will process information concerning students, many of whom are likely to be under eighteen years of age.

Accordingly, the project must investigate applicable requirements concerning children's personal data, parental consent, educational purposes and any relevant statutory exemptions.

The institution's legal responsibilities and the respective responsibilities of any technology providers must be established before production deployment.

### 5.3 Data Security and Privacy

The proposed system should incorporate:

- Authentication and authorisation.
- Role-based access control.
- Secure communication.
- Appropriate protection of stored information.
- Audit logging.
- Backup and recovery.
- Data retention and deletion policies.
- Protection against unauthorised access.
- Appropriate incident and breach handling procedures.

### 5.4 Cloud Data Management

If cloud infrastructure is selected, the following matters must be evaluated:

- Data processing agreements.
- Provider security arrangements.
- Data storage and processing locations.
- Access permissions.
- Backup and recovery arrangements.
- Data portability and export.
- Contract termination and data deletion.
- Applicable cross-border data transfer requirements.

### 5.5 Legal Feasibility Assessment

**Status: Conditionally Feasible.**

The proposed system can be designed with appropriate privacy and security safeguards.

However, production deployment will require verification of applicable legal obligations, institutional policies, data processing arrangements and any necessary approvals.

---

## 6. Schedule Feasibility

Schedule feasibility evaluates whether the project can be completed within a realistic timeframe considering the available personnel, resources and technical dependencies.

### 6.1 Development Team

The initial development team consists of two members.

Their responsibilities are divided according to their respective areas of expertise.

- Anirban Ghosh: Database, backend, application software and documentation.
- Satyajit Moitra: Hardware, firmware, embedded systems and device integration.

Both members will participate in system architecture, integration and testing.

### 6.2 Major Development Phases

The anticipated development sequence is:

| Phase | Major Activities |
|---|---|
| 1. Project Initiation | Project planning and documentation |
| 2. Requirements Engineering | Stakeholder consultation and SRS preparation |
| 3. System Design | Architecture, database and hardware design |
| 4. Prototyping | Hardware and software prototypes |
| 5. Implementation | Backend, frontend, database and firmware development |
| 6. Integration | Hardware-software integration |
| 7. Testing | Functional, integration, performance and security testing |
| 8. Deployment | Installation, configuration and training |
| 9. Documentation | Final technical documentation and project closure |

### 6.3 Potential Scheduling Risks

- Delays in hardware procurement.
- Difficulty obtaining existing hardware specifications.
- Hardware compatibility problems.
- Delays in institutional requirements approval.
- Limited development time alongside professional responsibilities.
- Integration difficulties.
- Unanticipated scope expansion.
- Deployment and testing delays.

### 6.4 Schedule Management

The project will adopt an iterative development approach.

Major deliverables will be divided into smaller milestones, allowing independent development and testing of individual modules.

A detailed project schedule, including task dependencies, estimated durations and milestone dates, will be prepared after requirements analysis and resource estimation.

### 6.5 Schedule Feasibility Assessment

**Status: Undetermined.**

The project can be divided into manageable development phases, but its completion timeline cannot yet be reliably estimated.

A realistic schedule will require confirmation of hardware availability, institutional requirements, team availability and deployment expectations.

---

## 7. Preliminary Risk Assessment

The following risks have been identified during the feasibility investigation.

| Risk ID | Risk Description | Potential Impact | Preliminary Mitigation |
|---|---|---|---|
| R-01 | Existing RFID hardware incompatibility | Additional expenditure | Inspect existing hardware before procurement |
| R-02 | Internet connectivity interruptions | Delayed event transmission | Local event buffering |
| R-03 | Hardware malfunction | Missing movement records | Device monitoring and testing |
| R-04 | Unauthorised data access | Privacy and security incidents | Authentication and access control |
| R-05 | Incomplete requirements | Rework and delays | Structured requirements gathering |
| R-06 | Excessive project scope | Development delays | Formal scope management |
| R-07 | Cloud service interruption | Temporary loss of remote access | Backup and recovery planning |
| R-08 | Incorrect attendance calculation | Inaccurate academic records | Institutional rule validation and correction mechanisms |
| R-09 | Limited maintenance resources | Long-term operational difficulties | Technical documentation and training |
| R-10 | Unplanned operational expenses | Increased project cost | Detailed cost estimation |

A separate Risk Register will be developed during the project planning and risk management activities.

---

## 8. Overall Feasibility Assessment

The preliminary findings are summarised below.

| Feasibility Dimension | Preliminary Status |
|---|---|
| Technical | Conditionally Feasible |
| Economic | Undetermined |
| Operational | Conditionally Feasible |
| Legal | Conditionally Feasible |
| Schedule | Undetermined |

### 8.1 Overall Assessment

The proposed SchoolTrack system appears technically achievable and is aligned with the institution's identified need for independent management of RFID-generated student movement information.

However, several important factors remain unresolved, including existing hardware compatibility, infrastructure availability, financial requirements, regulatory obligations and development scheduling.

These uncertainties must be addressed before the project can receive a final feasibility determination.

### 8.2 Preliminary Recommendation

It is recommended that the project proceed to detailed requirements engineering and technical investigation, subject to institutional approval and the resolution of the identified feasibility constraints.

Particular priority should be given to:

1. Inspection of the existing RFID hardware.
2. Evaluation of cloud, local and hybrid deployment architectures.
3. Database technology comparison.
4. Hardware procurement and cost estimation.
5. Verification of applicable data protection requirements.
6. Validation of administrative and transportation workflows.

---

## 9. Conclusion

The feasibility study indicates that SchoolTrack has a reasonable basis for further development, provided that the outstanding technical, economic, operational, legal and scheduling considerations are properly investigated.

The proposed system offers the potential to improve institutional control over student movement information, simplify administrative reporting and establish a foundation for future automation.

The final development architecture and implementation plan will be determined following detailed requirements analysis, technical evaluation and institutional consultation.

---

**Document ID:** ST-FS-001  
**Version:** 0.1  
**Status:** Preliminary Assessment  
**Prepared By:** Anirban Ghosh and Satyajit Moitra
