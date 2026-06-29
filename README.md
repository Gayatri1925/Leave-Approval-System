# Leave-Approval-System
Employees apply for leave through ServiceNow.
## Project Overview

The **Leave Approval Management System** is a ServiceNow-based application designed to simplify and automate the employee leave request process within an organization. Instead of relying on manual approvals and email communication, the system provides a centralized platform where employees can submit leave requests and managers can review, approve, or reject them through an automated workflow.

The application is built using ServiceNow's low-code capabilities, including custom tables, forms, Flow Designer, and email notifications. When an employee submits a leave request, the system automatically routes it to the assigned manager for approval. Based on the manager's decision, the leave request status is updated, and the employee is notified via email.

This project demonstrates the implementation of workflow automation in ServiceNow by integrating request management, approval processes, and automated notifications to improve efficiency, transparency, and user experience.

## Project Objectives

The primary objectives of the **Leave Approval Management System** are:

- Automate the employee leave request and approval process using ServiceNow.
- Eliminate manual paperwork and reduce the time required to process leave requests.
- Provide employees with a simple and user-friendly interface to submit leave applications.
- Enable managers to review and approve or reject leave requests through an automated workflow.
- Send automatic email notifications to employees regarding the status of their leave requests.
- Maintain accurate and centralized records of all leave requests for easy tracking and management.
- Improve transparency by allowing employees and managers to monitor the progress of leave requests.
- Demonstrate the use of ServiceNow features such as custom tables, forms, Flow Designer, approvals, and notifications in building a real-world business application.

  ## Key Features

- **Employee Leave Request Form:** Allows employees to submit leave requests by providing details such as leave type, start date, end date, reason, and assigned manager.

- **Automated Approval Workflow:** Uses ServiceNow Flow Designer to automatically trigger the approval process when a leave request is submitted.

- **Manager Approval Process:** Routes leave requests to the assigned manager, who can approve or reject the request directly from the approval interface.

- **Automatic Status Updates:** Updates the leave request status based on the manager's decision, ensuring accurate tracking of requests.

- **Email Notifications:** Sends automated email notifications to employees informing them whether their leave request has been approved or rejected.

- **Centralized Leave Records:** Stores all leave requests in a single location, making it easy to view, manage, and track leave history.

- **User-Friendly Interface:** Provides intuitive forms and records for employees and managers, making the leave management process simple and efficient.

- **Workflow Automation:** Reduces manual intervention by automating request routing, approvals, and notifications, improving overall organizational efficiency.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| **ServiceNow** | Platform used to develop and manage the Leave Approval Management System. |
| **Flow Designer** | Automates the leave approval workflow and business processes. |
| **Custom Tables** | Stores employee leave request data and related information. |
| **Forms** | Provides an interface for employees to submit leave requests and managers to review them. |
| **Approval Engine** | Manages the approval and rejection process for leave requests. |
| **Email Notifications** | Sends automated emails to employees about the status of their leave requests. |
| **ServiceNow Studio** | Used to develop and manage the application components. |
| **Personal Developer Instance (PDI)** | Used as the development and testing environment for the application. |

## Project Phases

### 1. Ideation Phase
The idea was to develop an automated Leave Approval Management System that simplifies and streamlines the leave request and approval process.

### 2. Requirement Analysis
The functional and technical requirements were identified to support leave requests, manager approvals, status tracking, and email notifications.

### 3. Project Design Phase
The system architecture, database structure, forms, and workflow were designed to ensure an efficient approval process.

### 4. Project Planning Phase
The project scope, development timeline, implementation tasks, and testing strategy were planned before development began.

### 5. Project Development Phase
The application was developed in ServiceNow using custom tables, forms, Flow Designer workflows, approval mechanisms, and email notifications.

### 6. Project Documentation
Comprehensive documentation was prepared to describe the project's objectives, implementation, workflow, and usage.

### 7. Project Demonstration
The completed application was demonstrated by submitting a leave request, processing manager approval, and verifying the automated workflow and notifications.

## Installation and Setup

### Prerequisites

Before deploying the project, ensure you have the following:

- A ServiceNow Personal Developer Instance (PDI) or ServiceNow instance.
- Admin access to configure tables, forms, Flow Designer, and notifications.
- Basic knowledge of the ServiceNow platform and navigation.
- A modern web browser (Google Chrome, Microsoft Edge, or Mozilla Firefox).
- An active internet connection.

### Deployment Steps

#### 1. Access Your ServiceNow Instance

Navigate to your ServiceNow instance using the following URL:

```text
https://your-instance.service-now.com
```

Log in using your administrator credentials.

---

#### 2. Create the Application

- Open **Studio** from the Application Navigator.
- Create a new scoped application named **Leave Approval Management System**.

---

#### 3. Create the Custom Table

- Create a custom table to store employee leave requests.
- Add the required fields such as Employee, Manager, Leave Type, Start Date, End Date, Reason, and Status.

---

#### 4. Configure the Leave Request Form

- Design the form by arranging all required fields.
- Configure field properties and make mandatory fields as needed.

---

#### 5. Create the Flow Designer Workflow

- Open **Flow Designer**.
- Create a new flow that is triggered when a leave request record is created or submitted.

---

#### 6. Configure the Approval Process

- Add an approval action to send the leave request to the selected manager.
- Configure the flow to wait for the manager's approval or rejection.

---

#### 7. Configure Status Updates

- Update the leave request status automatically based on the manager's decision (Approved or Rejected).

---

#### 8. Configure Email Notifications

- Create email notification actions to inform employees when their leave request is approved or rejected.

---

#### 9. Test the Application

- Submit a leave request as an employee.
- Impersonate the assigned manager and approve or reject the request.
- Verify that the request status is updated and the employee receives the appropriate email notification.

---

#### 10. Validate the Workflow

- Ensure the complete leave approval process functions correctly from request submission to manager approval and employee notification.
