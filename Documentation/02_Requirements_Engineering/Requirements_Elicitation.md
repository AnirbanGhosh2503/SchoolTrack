# Requirements Elicitation

**Project:** SchoolTrack – RFID-Based Student Movement Management System  
**Document ID:** ST-RE-001  
**Version:** 0.1  
**Status:** Initial Working Draft – Requirements Under Elicitation  
**Prepared by:** Anirban Ghosh and Satyajit Moitra  
**Date:** 16 November 2026

---

## 1. Introduction

### 1.1 Purpose

The purpose of this document is to identify, collect and organise the requirements of SchoolTrack by examining the needs of its stakeholders, the existing RFID-based student movement management process and the operational environment of the school.

This document will serve as the initial record of information gathered during the Requirements Engineering phase.

It will distinguish confirmed stakeholder needs from proposed features, temporary assumptions and unresolved questions.

### 1.2 Project Background

The school currently uses an RFID-based system to record student movement, including entry into and exit from school premises and boarding or deboarding school buses.

The existing arrangement involves an external RFID service provider. The school has expressed the need for greater independence and access to its student movement data.

SchoolTrack is proposed as an independent system that will allow the school to manage student movement records, access relevant information and generate operational reports.

The preferred architectural direction for further investigation is a hybrid approach involving local event storage and cloud synchronisation. This remains subject to technical validation.

### 1.3 Objectives of Requirements Elicitation

The primary objectives are:

1. Understand the school's existing student movement recording process.
2. Identify the information required by the School Office and other stakeholders.
3. Understand the capabilities and limitations of the existing RFID hardware.
4. Identify the required software functionalities.
5. Determine operational, security, privacy and performance expectations.
6. Identify connectivity and offline-operation requirements.
7. Discover potential exceptions and unusual operational scenarios.
8. Establish a foundation for the Software Requirements Specification (SRS).

---

## 2. Stakeholder Identification

The following stakeholders have been identified as relevant to requirements elicitation.

| Stakeholder | Relevance to Requirements |
|---|---|
| School Secretary | Final institutional approval and major project decisions |
| Principal | Institutional oversight and operational expectations |
| School Office | Primary operational user; student movement monitoring and reporting |
| IT / Computer Department | Technical support and possible system administration |
| Teachers | Potential users of student movement and attendance information |
| Transport Department | Bus movement and transport-related requirements |
| Bus Operators | Practical operation of bus-based RFID devices |
| Students | Individuals whose movement records are maintained |
| Parents / Guardians | Potential future recipients of student-related notifications |
| Development Team | Technical requirements, implementation and validation |
| Existing RFID Provider | Potential source of hardware and system information |

The identification of a stakeholder does not automatically imply that the stakeholder will receive access to the system.

Access permissions and responsibilities will be determined separately.

---

## 3. Initial Understanding of the Existing System

Based on information currently available, the following understanding has been established.

### 3.1 Existing Operational Functions

- Students use RFID cards.
- RFID readers record student movement events.
- Events include entry into and exit from school premises.
- Bus-related events include boarding and deboarding.
- The existing arrangement involves an external service provider.

### 3.2 Known Institutional Context

- The replacement initiative originated from the School Office.
- The initiative received support from the Principal and Secretary.
- The Secretary is the final project approval authority.
- The School Office is the primary operational stakeholder.
- The School Office is expected to interact with the system approximately two to four times per day, depending on school timings.
- The school has expressed interest in accessing and managing its own movement data.

### 3.3 Information Yet to Be Verified

The following details are not yet sufficiently established:

- RFID reader and card specifications.
- Reader connectivity and communication protocols.
- Existing data storage arrangements.
- Whether the existing hardware supports local data extraction.
- Availability of timestamps and reader identification in exported records.
- Existing data export formats.
- School LAN and internet infrastructure.
- Bus-device connectivity and data transfer mechanisms.
- Existing vendor data access and migration possibilities.

These details will be investigated before finalising the technical requirements.

---

## 4. Preliminary Requirement Categories

The following categories will guide the elicitation process.

### 4.1 Functional Requirements

These describe the operations that SchoolTrack may need to perform.

Preliminary areas of investigation include:

- Student registration and profile management.
- RFID card registration and assignment.
- RFID movement event collection.
- School entry and exit monitoring.
- Bus boarding and deboarding records.
- Student movement history.
- Search and filtering of records.
- Report generation.
- Data export in Excel, CSV and PDF formats.
- User account and access management.
- Device and synchronisation monitoring.

These are candidate functionalities, not yet approved final requirements.

### 4.2 Non-Functional Requirements

These describe the quality attributes and operational expectations of the system.

Areas requiring investigation include:

- Reliability and data integrity.
- Performance under normal school operations.
- Availability during internet interruptions.
- Offline event storage and subsequent synchronisation.
- Security and access control.
- Privacy and protection of student information.
- Usability for non-technical office personnel.
- Maintainability and recoverability.
- Compatibility with available hardware and infrastructure.

### 4.3 Business Requirements

These concern the institutional objectives of the project.

Initial areas include:

- Greater school independence in managing student movement information.
- Reliable access to movement records.
- Reduced dependence on the existing external service provider.
- Efficient generation of operational reports.
- Improved availability of historical student movement information.

### 4.4 Proposed Future Enhancements

The following ideas have been suggested but have not been approved as baseline project requirements:

1. Automated academic attendance calculation using RFID movement records.
2. Monthly class-wise attendance reports.
3. Identification of students falling below an institutionally defined attendance threshold, such as 65%.
4. Parent or guardian notifications.
5. Additional student and transport-related reporting.

Any automated attendance functionality will require explicit institutional policies covering late arrival, early departure, holidays, approved leave, missing scans, half-days and other exceptions.

Raw movement records must remain distinguishable from derived attendance records.

---

## 5. Requirements Classification Convention

Every requirement or piece of information recorded during elicitation will be assigned one of the following classifications.

| Classification | Meaning |
|---|---|
| Confirmed | Explicitly communicated or validated by an authorised stakeholder |
| Proposed | Suggested as a possible feature or improvement |
| Assumed | Temporarily accepted for analysis but awaiting verification |
| Open | Information currently unavailable or requiring clarification |

This classification will prevent unverified assumptions from being treated as approved institutional requirements.

---

## 6. Requirements Elicitation Methods

The following methods will be used.

### 6.1 Stakeholder Interviews

Discussions with the School Office, Principal, Secretary and other relevant personnel to understand operational needs, expectations and constraints.

### 6.2 Observation

Observation of existing student movement recording procedures, including school entry, exit and bus operations.

### 6.3 Existing System Investigation

Examination of available RFID hardware, cards, software interfaces, data exports and existing operational documentation.

### 6.4 Technical Investigation

Collaboration between the development team to examine device capabilities, connectivity, local storage, synchronisation and integration possibilities.

### 6.5 Document Analysis

Review of available student records, movement reports, attendance policies, operational instructions and other relevant institutional documents, subject to authorised access.

---

## 7. Initial Open Questions

The following questions will guide further investigation.

### 7.1 Institutional and Operational Questions

- What exact information does the School Office currently receive from the existing RFID system?
- Which reports are required daily, weekly and monthly?
- Who should be authorised to view, modify and export student information?
- What happens when a student forgets or loses an RFID card?
- How are corrections to incorrect movement records currently handled?
- Does the school require historical records to be migrated?

### 7.2 Hardware Questions

- Which RFID technology and card type are currently in use?
- What are the models of the existing readers?
- Are readers connected to a central controller or operate independently?
- How are school-premises readers connected?
- How are bus readers connected?
- Can devices store events locally?
- Can stored events be exported through USB, serial connection, network or another interface?
- Is the existing hardware reusable?

### 7.3 Infrastructure Questions

- Does the school have an existing local server?
- Is a school-wide LAN available?
- What is the reliability of the school's internet connection?
- Is there a provision for backup power?
- Are there restrictions on using external cloud services?

### 7.4 Data and Privacy Questions

- Which student information is genuinely necessary?
- Who owns and controls the collected records?
- How long should movement records be retained?
- What access restrictions should apply to different user categories?
- What security and privacy requirements must be followed?
- What institutional approvals are necessary before processing student information through cloud infrastructure?

### 7.5 Attendance-Related Questions

- Does the school intend to use RFID movement records for academic attendance?
- What constitutes a full day, half-day or absence?
- How should late arrivals and early departures be treated?
- How should missing scans and device failures be handled?
- Which attendance policy and threshold should the system follow?

---

## 8. Initial Requirements Elicitation Status

At this stage, SchoolTrack has an initial understanding of its institutional purpose, major stakeholders and broad operational environment.

However, detailed functional, non-functional and technical requirements have not yet been validated.

The existing RFID system, hardware capabilities, institutional workflows and school infrastructure require further investigation.

Therefore, this document is an evolving working record and must not be treated as the final Software Requirements Specification.

---

## 9. Next Steps

The following activities are planned:

1. Investigate the existing RFID hardware and data collection process.
2. Gather detailed operational requirements from the School Office.
3. Identify school infrastructure and connectivity constraints.
4. Discuss technical requirements with the hardware and software development team.
5. Classify and prioritise the collected requirements.
6. Prepare the Requirements Analysis document.
7. Develop use cases and process models.
8. Prepare and validate the Software Requirements Specification.

---

**End of Document**

*SchoolTrack — RFID-Based Student Movement Management System*
