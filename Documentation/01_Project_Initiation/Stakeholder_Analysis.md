# STAKEHOLDER ANALYSIS

**Project:** SchoolTrack – RFID-Based Student Movement Management System  
**Document ID:** ST-PA-001  
**Version:** 0.2  
**Status:** Revised Draft – Pending Stakeholder Validation  
**Prepared By:** Anirban Ghosh and Satyajit Moitra  
**Last Updated:** 16 November 2026

---

## 1. Introduction

Stakeholder analysis is the process of identifying individuals, groups and organisations that can influence, participate in, or be affected by a project.

The purpose of this document is to identify the stakeholders associated with SchoolTrack, understand their interests and expectations, assess their potential influence and establish appropriate engagement strategies.

The findings will contribute to requirements engineering, system architecture, project governance and the eventual deployment of the proposed system.

This document incorporates preliminary information obtained through discussions with the institution's office.

## 2. Stakeholder Identification

The stakeholders associated with SchoolTrack are classified into four broad categories.

### 2.1 Institutional Decision-Makers

- School Secretary – Project approval authority.
- School Principal – Institutional leadership and project supporter.
- School Office – Originating department and primary operational stakeholder.

### 2.2 Internal Operational Stakeholders

- School Administration.
- IT/Computer Department.
- Teachers.
- Transport Department.
- Bus Operators.

### 2.3 External and Indirect Stakeholders

- Students.
- Parents and Guardians.
- RFID Hardware Suppliers.
- Cloud Infrastructure Providers.
- Existing RFID Service Provider.

### 2.4 Project Development Team

- Anirban Ghosh – Database architecture, backend development, application software and documentation.
- Satyajit Moitra – Hardware design, embedded systems, firmware and hardware integration.

## 3. Stakeholder Register

The following register identifies the primary stakeholders, their interests, responsibilities and preliminary levels of influence.

| ID | Stakeholder | Primary Interest / Responsibility | Influence |
|---|---|---|---|
| SH-01 | School Secretary | Final project approval and institutional authorisation | Very High |
| SH-02 | School Principal | Institutional oversight and project support | High |
| SH-03 | School Office | Project initiation and day-to-day system operation | High |
| SH-04 | IT/Computer Department | Technical administration and maintenance | Medium–High |
| SH-05 | Teachers | Student information and potential automated attendance | Medium |
| SH-06 | Transport Department | Bus operations and student movement monitoring | Medium–High |
| SH-07 | Bus Operators | Recording boarding and deboarding events | Low–Medium |
| SH-08 | Students | RFID-based identification and movement recording | Low |
| SH-09 | Parents/Guardians | Student safety and potential access to movement information | Medium |
| SH-10 | Development Team | System design, development, integration and delivery | High |
| SH-11 | External Technology Providers | Hardware supply, cloud infrastructure and technical support | Medium |

Influence classifications are preliminary and may be revised after further institutional consultation.

## 4. Stakeholder Expectations and Requirements

### 4.1 School Secretary

**Role:** Final Project Approval Authority.

Expected interests:

- Complete institutional control over the RFID data management system.
- Reduced dependency on external service providers.
- Reliable access to student movement information.
- Appropriate data security and administrative control.
- Visibility into project costs, progress and deliverables.

The Secretary will be the primary authority for formal project approval and acceptance.

### 4.2 School Principal

**Role:** Institutional Leadership and Project Support.

Expected interests:

- Improved monitoring of student movements.
- Reliable attendance-related information.
- Improved administrative efficiency.
- A system that supports institutional requirements.
- Appropriate oversight of the deployed solution.

### 4.3 School Office

**Role:** Project Originating Department and Primary Operational Stakeholder.

The replacement of the existing RFID system was originally suggested by the school office and supported by the Principal and Secretary.

Expected interests:

- Independent access to RFID-generated information.
- Convenient retrieval of student entry and exit records.
- Efficient monitoring of student movements.
- Centralised student and RFID card information.
- Searchable and downloadable reports.
- Simple and reliable daily operation.

**Operational consideration:**

The system is expected to support the institution's different academic schedules, including Pre-Primary and Primary–High School operations.

Based on preliminary discussions, system operations are expected to occur approximately two to four times daily, corresponding to the different school schedules and operational cycles.

The precise workflows and operating responsibilities will be established during requirements gathering.

### 4.4 IT/Computer Department

**Role:** Technical Administration and Maintenance.

Expected interests:

- Secure and manageable system architecture.
- Administrative control over users and devices.
- Database backup and recovery facilities.
- Maintainability and technical documentation.
- Reliable network and device connectivity.
- Independent management of institutional data.

### 4.5 Teachers

**Role:** Academic and Classroom-Level Stakeholders.

Expected interests:

- Convenient access to relevant student information.
- Reduced manual attendance-related workload.
- Reliable attendance records.
- Class-wise and section-wise attendance reports.

**Proposed additional requirement:**

An automated academic attendance module may be introduced as a future enhancement.

The proposed module would utilise verified school entry and exit records to calculate daily student attendance and generate monthly class-wise attendance sheets.

Potential functionalities include:

- Automated daily attendance calculation.
- Present, absent and half-day classification.
- Monthly attendance summaries.
- Identification of students with attendance below 65%.
- Downloadable class-wise attendance reports.
- Authorised manual correction of attendance records.

This proposal has not yet been approved by the institution and is not currently considered a mandatory project requirement.

Its feasibility and institutional acceptance will be investigated separately.

### 4.6 Transport Department

**Role:** Transportation Operations and Monitoring.

Expected interests:

- Bus-wise student movement records.
- Boarding and deboarding information.
- Route and trip management.
- Identification of incomplete or missing movement events.
- Convenient access to historical transportation records.

### 4.7 Bus Operators

**Role:** Operational Users of Bus-Based RFID Hardware.

Expected interests:

- Simple device operation.
- Reliable recording of RFID scans.
- Clear indication of successful and unsuccessful scans.
- Minimal manual intervention.
- Reliable operation despite intermittent internet connectivity.

### 4.8 Students

**Role:** Primary Subjects of RFID Identification and Movement Recording.

Expected interests:

- Reliable student identification.
- Accurate recording of movement events.
- Protection of personal information.
- Minimisation of incorrect or duplicate attendance records.

### 4.9 Parents and Guardians

**Role:** Indirect Beneficiaries and Potential Future Users.

Expected interests:

- Reliable information regarding student attendance and movement.
- Protection of student information.
- Potential access to relevant notifications.

Parent-facing notifications and applications are not currently mandatory requirements. They may be considered as future enhancements subject to institutional approval.

### 4.10 Development Team

**Role:** System Design, Development, Integration and Delivery.

**Anirban Ghosh:**
- Database architecture and implementation.
- Backend development.
- Application software and APIs.
- Web dashboard development in collaboration with the team.
- Technical documentation.

**Satyajit Moitra:**
- RFID hardware design and selection.
- Embedded systems and firmware.
- Device communication.
- Hardware prototyping and integration.

**Joint responsibilities:**
- System architecture decisions.
- Requirements validation.
- Hardware-software integration.
- Testing and evaluation.
- Deployment preparation.
- Technical demonstrations.

### 4.11 External Technology Providers

**Role:** External Infrastructure and Hardware Support.

Expected contributions may include:

- RFID hardware specifications.
- Device communication documentation.
- Hardware procurement.
- Cloud infrastructure services.
- Technical compatibility information.

The existing RFID service provider may be approached for hardware documentation and compatibility information, subject to institutional approval.

## 5. Power-Interest Analysis

Stakeholders are classified according to their relative power and interest in the project.

### 5.1 Stakeholder Classification

| Category | Stakeholders | Engagement Strategy |
|---|---|---|
| High Power – High Interest | Secretary, Principal, School Office, Development Team | Manage Closely |
| High Power – Lower Interest | Other institutional decision-makers, if applicable | Keep Satisfied |
| Lower Power – High Interest | Teachers, Transport Department, Bus Operators, Students, Parents | Keep Informed |
| Lower Power – Lower Interest | Peripheral external stakeholders | Monitor |

The IT/Computer Department and relevant operational departments may move between categories depending on their actual responsibilities and authority.

### 5.2 Power-Interest Matrix

The matrix below represents the preliminary classification.

| | High Interest | Lower Interest |
|---|---|---|
| High Power | Manage Closely | Keep Satisfied |
| Lower Power | Keep Informed | Monitor |

Stakeholder positions will be reassessed as the project progresses and actual responsibilities become clearer.

## 6. Stakeholder Communication and Engagement Plan

| Stakeholder | Communication Method | Proposed Frequency |
|---|---|---|
| School Secretary | Formal meetings and project demonstrations | At major milestones and approval stages |
| School Principal | Progress reviews and demonstrations | At major milestones |
| School Office | Interviews, operational discussions and feedback | During requirements analysis and testing |
| IT Department | Technical consultations | Throughout development |
| Teachers | Interviews and usability feedback | During requirements analysis and UAT |
| Transport Department | Workflow discussions and demonstrations | During requirements and integration |
| Bus Operators | Practical demonstrations and hardware testing | During prototyping and integration |
| Students/Parents | Institutional consultation and feedback, where appropriate | As required |
| Development Team | Technical meetings and progress reviews | Weekly or as required |
| External Providers | Technical correspondence and documentation requests | When required |

## 7. Stakeholder-Related Risks

Potential risks arising from stakeholder involvement include:

1. Incomplete or unclear institutional requirements.
2. Conflicting expectations between administrative and transportation departments.
3. Limited availability of institutional personnel for consultations.
4. Resistance to changes in existing operational procedures.
5. Delays in obtaining technical specifications from external providers.
6. Unclear responsibility for long-term maintenance.
7. Uncertainty regarding user access privileges.
8. Unapproved expansion of the project scope through additional feature requests.
9. Lack of agreement on automated attendance calculation policies.

Appropriate mitigation strategies will be incorporated into the Project Risk Register.

## 8. Open Questions for Stakeholder Consultation

The following matters require further investigation:

### 8.1 Institutional Governance

1. Who will be responsible for day-to-day technical administration after deployment?
2. Will the school appoint a dedicated system administrator?
3. What will be the formal acceptance criteria for the completed project?

### 8.2 System Operation

4. Which office personnel will operate the system?
5. Will separate administrative accounts be required for different departments?
6. What reports are required during each operational cycle?
7. Should the system support different academic schedules independently?

### 8.3 Academic Attendance

8. Does the institution intend to replace manual classroom attendance with RFID-derived attendance?
9. What are the official rules for half-day attendance?
10. How should late arrivals and early departures be classified?
11. Should teachers be permitted to correct automatically calculated attendance?
12. Is the 65% attendance threshold applied to total working days or another institutional calculation?

### 8.4 Transportation

13. Who will manage bus routes, trips and student assignments?
14. Will bus operators interact directly with the application?
15. How will offline bus movement records be transferred?

### 8.5 Future Enhancements

16. Would the institution consider parent-facing notifications in a future phase?
17. Would teachers benefit from individual accounts and class-specific dashboards?

## 9. Conclusion

The stakeholder analysis identifies the principal institutional, operational, technical and indirect stakeholders associated with SchoolTrack.

Preliminary institutional discussions have established that the project originated from the school office, received support from the Principal and Secretary, and will require final approval from the Secretary.

The school office is expected to be the primary operational stakeholder, while the IT Department and other relevant departments will contribute to the technical and operational requirements.

Potential enhancements, including automated academic attendance management and parent-facing notifications, have also been identified for further evaluation.

The stakeholder register, influence classifications and engagement strategies will be reviewed and updated as additional information becomes available.

---

**Document ID:** ST-PA-001  
**Version:** 0.2  
**Status:** Revised Draft – Pending Stakeholder Validation  
**Prepared By:** Anirban Ghosh and Satyajit Moitra
