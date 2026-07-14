
# AI-Enabled Student Admission System

## Project Overview

The **AI-Enabled Student Admission System** is a Salesforce-based intelligent admission management solution designed to streamline student admission processing through automated application evaluation, document verification, AI-assisted admission guidance, and real-time analytics.

This project leverages Salesforce platform capabilities including **Agentforce, Prompt Builder, Flow Builder, Validation Rules, Reports, and Dashboards** to reduce manual admission processing and improve the efficiency of admission officers.

The system keeps admission officers in control of final admission decisions while using AI to assist with application review and guidance.

---

## Features

### Admission Application Management

- Create, update, and manage student admission applications.
- Store applicant and academic information.
- Track application status.
- Manage program selection.
- Monitor application completeness.

### Automated Application Evaluation

- Automatically evaluate application completeness.
- Check academic percentage against program eligibility criteria.
- Identify missing applicant documents.
- Assign application status based on evaluation results.
- Reduce repetitive manual verification work.

### Document Verification

- Track applicant document verification.
- Identify missing documents.
- Store document verification status.
- Record verification comments.
- Maintain verification information for each admission application.

### AI Admission Guidance

- Generate intelligent admission guidance using Prompt Builder.
- Analyze application information and academic details.
- Identify incomplete application information.
- Suggest the next action for admission officers.
- Generate professional suggested responses for applicants.
- Maintain human review before final admission decisions.

### Agentforce Integration

- AI-powered Student Admission Assistant.
- Application-based admission guidance.
- Admission Application ID-based interaction.
- Applicant status and missing-document assistance.
- AI-assisted responses for admission queries.
- Enhanced admission officer productivity.

### Automated Email Notifications

- Send admission status update emails.
- Notify applicants when application status changes.
- Use Salesforce Email Templates and Email Alerts.
- Reduce delays in applicant communication.

### Reporting & Analytics

- Applications by Status Report.
- Applications by Program Report.
- Application Review Performance Report.
- Application pipeline monitoring.
- Program demand analysis.
- Admission officer review performance tracking.

### Security & Access Control

- Admission Officer Profile.
- Admission Manager Profile.
- System Administrator access.
- Permission Sets for AI and reporting features.
- Field-Level Security for sensitive admission information.
- Role-based access to admission data.

---

## Technologies Used

- Salesforce Developer Edition
- Salesforce Lightning Experience
- Agentforce
- Prompt Builder
- Prompt Templates
- Flow Builder
- Record-Triggered Flows
- Validation Rules
- Email Templates
- Email Alerts
- Reports & Dashboards
- Profiles
- Permission Sets
- Field-Level Security

---

## System Workflow

1. A student admission application is created.
2. Applicant and academic information is stored in Salesforce.
3. The record-triggered flow evaluates application completeness.
4. Academic percentage is checked against program eligibility criteria.
5. Required applicant documents are verified.
6. Missing documents are identified.
7. Application status is automatically updated.
8. Agentforce analyzes the admission application information.
9. AI Admission Guidance is generated using Prompt Builder.
10. The admission officer reviews the AI-generated guidance.
11. The admission officer processes the application.
12. Applicants receive admission status update notifications.
13. Admission data is monitored through reports and dashboards.

---

## Reports Implemented

### Applications by Status

Displays student admission applications grouped by application status.

Application statuses include:

- Submitted
- Under Review
- Documents Pending
- Eligible
- Shortlisted
- Approved
- Rejected

### Applications by Program

Displays the number of admission applications received for each academic program.

Helps admission managers analyze:

- Program demand
- Application volume
- Student program preferences

### Application Review Performance

Tracks:

- Applications reviewed
- Pending applications
- Completed reviews
- Admission officer workload
- Review performance

---

## Admission Management Dashboard

The **Admission Management Dashboard** provides real-time visibility into the student admission process.

Dashboard components include:

- Applications by Status – Donut Chart
- Applications by Program – Bar Chart
- Admission Review Performance – Summary Chart

The dashboard helps admission managers monitor application progress, program demand, and admission team performance.

---

## Lightning Application

### AI-Enabled Student Admission System

The custom Salesforce Lightning App includes:

- Home
- Admission Applications
- Programs
- Document Verifications
- AI Feedbacks
- Reports
- Dashboards
- Contacts
- Agentforce Integration

---

## Sample Objects Used

### Standard Objects

- Account
- Contact

### Custom Objects

- Admission Application
- Program
- Document Verification
- AI Feedback

### Custom Fields

- Application Number
- Applicant
- Program Applied
- Academic Percentage
- Application Status
- Application Priority
- Application Completeness
- Missing Documents
- AI Admission Guidance
- Application Date
- Review Date
- Admission Decision

---

## AI Feedback

The system captures admission officer feedback on AI-generated guidance.

Feedback information includes:

- AI Suggestion Type
- Feedback Status
- Admission Officer Comments
- Related Admission Application
- Created By

Feedback statuses:

- Helpful
- Not Helpful

This feedback mechanism provides a foundation for evaluating and improving AI-generated admission guidance.

---

## Validation Rule

### Academic Percentage Required

The system prevents an admission application from being submitted without the applicant's academic percentage.

```text
AND(
    ISPICKVAL(Application_Status__c, "Submitted"),
    ISBLANK(Academic_Percentage__c)
)
````

**Error Message:**

> Academic Percentage must be provided before submitting the admission application.

---

## Agentforce AI Assistant

### Student Admission Assistance

The Agentforce AI assistant helps admission officers analyze student admission applications.

The assistant can:

* Review applicant information.
* Analyze academic percentage.
* Review the selected program.
* Check application status.
* Identify missing information.
* Generate AI Admission Guidance.
* Suggest the next action for the admission officer.
* Generate a professional response for the applicant.

The AI assistant does **not make final admission decisions**.

Final admission decisions remain under human admission officer review.

---

## Project Screenshots

Project screenshots are available in the `Screenshots` folder.

Screenshots include:

* Salesforce Setup Home
* Student Admission Lightning App
* Program Object Manager
* Document Verification Object
* AI Feedback Object
* Admission Application Record
* Academic Percentage Validation Rule
* Admission Application Evaluation Flow
* Admission Status Email Template
* Agentforce AI Admission Assistant
* Admission Reports Folder
* Admission Management Dashboard
* Admission Officer Profile
* Admission Manager Profile
* Permission Sets

---

## Folder Structure

```text
ai-enabled-student-admission-system
│
├── README.md
├── Project_Report.pdf
│
├── Screenshots
│   ├── Salesforce_Setup_Home.png
│   ├── Student_Admission_Lightning_App.png
│   ├── Program_Object_Manager.png
│   ├── Document_Verification_Object.png
│   ├── AI_Feedback_Object.png
│   ├── Admission_Application_Record.png
│   ├── Academic_Percentage_Validation_Rule.png
│   ├── Admission_Application_Evaluation_Flow.png
│   ├── Admission_Status_Email_Template.png
│   ├── Agentforce_AI_Admission_Assistant.png
│   ├── Admission_Reports_Folder.png
│   ├── Admission_Management_Dashboard.png
│   ├── Admission_Officer_Profile.png
│   ├── Admission_Manager_Profile.png
│   └── Permission_Sets.png
│
└── Documentation
    └── AI_Enabled_Student_Admission_System_Documentation.pdf
```

---

## Author

**Annamneedi Satyanarayana**

B.Tech – Computer Science & Engineering

Bonam Venkata Chalamayya Engineering College

Email: [siddunaidu592@gmail.com](mailto:siddunaidu592@gmail.com)

GitHub: [https://github.com/satya-1114](https://github.com/satya-1114)

LinkedIn: [https://www.linkedin.com/in/annamneedi-s14](https://www.linkedin.com/in/annamneedi-s14)

---
## 🎥 Project Demo

🎥 **Watch the complete project demonstration:** [View Demo Video on Google Drive](https://drive.google.com/file/d/127yzljtJLITX34ECFjfZ-5zY_Gmw1xGC/view?usp=drivesdk)

## License

This project is developed for **educational and learning purposes** using Salesforce Developer Edition.

The project demonstrates Salesforce administration, automation, Agentforce AI integration, Prompt Builder, security configuration, and admission management concepts.


