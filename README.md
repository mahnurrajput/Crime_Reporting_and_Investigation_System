# Intel Crime Nexus
### Intelligence-Driven Crime Reporting & Investigation System
 
> A structured digital platform for law enforcement case management, built with real Pakistani court data and engineered for analytical depth.
 
---
 
## Overview
 
**Intel Crime Nexus** is a desktop-based crime management system designed to bring structure, traceability, and analytical intelligence to law enforcement workflows. The system supports the full lifecycle of a criminal case — from initial public report through investigation, evidence tracking, and case closure — in a role-controlled, auditable environment.
 
Built using **C# WinForms (.NET Framework)** and **SQL Server**, the project demonstrates applied software engineering across database design, access control architecture, workflow automation, and analytical logic.
 
🎓 **4th Semester Fundamentals of Software Engineering Project** | FAST NUCES – 2025
 
---
 
## Project Access
 
> The full source code is maintained in a **private repository**.
 
Recruiters, academic reviewers, and collaborators may request access for evaluation purposes:
 
📧 `mahnoornaveed2405@gmail.com`
 
---
 
## What the System Records
 
Each case in the system captures a structured set of data entities:
 
- **Case metadata** — FIR number, case title, crime type, crime category, location, date/time, and status
- **Suspects** — name, gender, criminal history, last known location, role in the crime, and conviction status
- **Victims** — identity, age, gender, condition (deceased / injured / unharmed), and recorded statement
- **Witnesses** — name, witness type (eyewitness / character / expert), statement, and submission details
- **Evidence** — type (physical item, photograph, document, forensic report), collection officer, collection date, storage location, and current status
- **Leads** — source (officer / anonymous / public), description, verification status, and timestamp
- **Crime scene** — type (indoor/outdoor), location, and scene description
- **Case timeline** — chronologically ordered log of every action taken: officer assignments, evidence collection, arrests, forensic reports, witness statements, and judgment updates
- **Officers** — designation, police station, role in each case (investigating officer, duty officer, prosecutor)
- **FIR and Reports** — filed date, filing location, report type, and approval status
- **Case assignments** — which officer was assigned by whom, when, and in what capacity
---
 
## Dataset — Grounded in Real Court Records
 
The database is populated with data extracted from **30 real criminal cases**, sourced from **official Punjab High Court judgments** published on the High Court's official website.
 
Key facts about the dataset:
 
- **30 cases** spanning diverse crime categories including murder, assault, theft, fraud, and more
- **150+ officer records** reflecting real designations, stations, and chain-of-command structures
- Full **chain of evidence** recorded per case, including forensic lab reports, autopsy records, ballistic analyses, and medical reports
- Witness statements, suspect histories, victim profiles, and case timelines reconstructed from judgment documents
- Data extraction was performed using an AI-assisted document analysis tool applied to the original PDF judgments
- A **deliberately conservative scope** — 30 cases rather than hundreds — was chosen to prioritize accuracy and traceability over volume
- Every data point can be traced back to a verifiable public court document, making this one of the few academic crime management projects with a fully attributable real-world dataset
---
 
## Core Capabilities
 
### Case Initiation — Two Pathways
- Public users submit reports that officers review and convert to formal FIRs
- Officers can independently initiate cases directly in the system
### Role-Based Access Control
- Distinct dashboards and permissions for public users, investigating officers, and senior officers
- Case assignment authority is rank-dependent
- Login credentials are admin-provisioned for officers; self-registered for public users
### Evidence & Chain of Custody
- Multimedia evidence attachments — images, videos, PDFs, audio
- Each evidence item is logged with collector, date, location, and status
- Full chain of custody maintained across all case activity
### Intelligence & Analytics Engine
 
| Module | Function |
|---|---|
| Crime Wave Detection | Identifies abnormal spikes in crime frequency within time-location clusters |
| Case Similarity Detection | Matches related cases by keyword overlap, geography, and metadata patterns |
| Fake Report Detection | Flags logically inconsistent or duplicate submissions for officer review |
| Crime Analytics Dashboard | Visual breakdown of crime types, monthly trends, hotspot locations, and victim statistics |
 
### Case Timeline Audit Log
Every update to a case — evidence collection, arrests, forensic results, witness statements, court decisions — is appended as a timestamped, actor-attributed timeline entry, providing a complete and immutable audit trail.
 
---
 
## System Modules
 
### Public User Module
- Self-registration and login, with anonymous reporting option
- Report submission with evidence and testimony attachments
- Case status tracking and submission history
- Advanced search filters across open cases
### Officer Module
- Admin-provisioned secure login
- Report review: approve, reject, or escalate to FIR
- Suspect and victim profile management
- Evidence logging and chain-of-custody tracking
- Witness statement recording
- Crime similarity and trend analysis tools
- Rank-based case assignment workflows
---
 
## Technology Stack
 
| Layer | Technology |
|---|---|
| Frontend | C# (.NET Framework), WinForms |
| Data Access | ADO.NET |
| Database | Microsoft SQL Server |
| Development Environment | Visual Studio, SQL Server Management Studio (SSMS) |
 
---
 
## Engineering Highlights
 
- **Normalized relational schema** across 15+ interconnected tables with referential integrity enforced throughout
- **Stored procedures and parameterized queries** used throughout to prevent SQL injection and centralize business logic
- **Workflow state machine** governing report → FIR → investigation → closure transitions with validation at each stage
- **Audit logging architecture** — all case mutations are recorded with actor identity and timestamp, never overwritten
- **Analytical query layer** built independently from transactional queries, enabling crime trend computation without impacting system performance
---
 
## Project Objectives
 
Intel Crime Nexus was designed to demonstrate that structured software engineering principles — applied to a real-world domain with real data — can produce a system that is both academically rigorous and practically credible.
 
The project covers:
- Relational database design and normalization
- Role-based access control and permission modeling
- Desktop application architecture with layered separation of concerns
- Integration of analytical/intelligence logic into an operational CRUD system
- Responsible use of AI tools for structured data extraction from legal documents
---
 
## Development Team
 
| Name | Role |
|---|---|
| Mahnoor Naveed | Project Lead & Software Architect |
| Fatima Riaz | Developer & Database Engineer |
| Aliza Sharafat | Database Engineer |
| Rabia Saeed | UI/UX Designer |
 
---
 
## Contact
 
**Mahnoor Naveed**
📧 [mahnoornaveed2405@gmail.com](mailto:mahnoornaveed2405@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/mahnoorrrajput/)
 
---
 
*If this project is relevant to your interests in applied database systems, desktop application architecture, or law enforcement technology — feel free to reach out or request repository access.*
