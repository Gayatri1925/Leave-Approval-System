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

## Usage

Follow these steps to use the Leave Approval Management System:

### 1. Submit a Leave Request
- Log in to the ServiceNow instance.
- Open the **Leave Request** application.
- Click **New** and fill in the required details, including the employee name, manager, leave type, start date, end date, and reason.
- Submit the leave request.

### 2. Manager Reviews the Request
- The assigned manager receives the leave request for approval.
- The manager opens the approval request from the **My Approvals** module.
- The manager reviews the leave details and chooses to **Approve** or **Reject** the request.

### 3. Automatic Workflow Execution
- The Flow Designer workflow processes the manager's decision.
- The leave request status is automatically updated based on the approval outcome.

### 4. Employee Notification
- The employee receives an automated email informing them whether the leave request has been approved or rejected.

### 5. Track Leave Requests
- Employees and administrators can view the current status and history of leave requests from the application records.

## System Architecture

```text
+------------------+
|    Employee      |
+------------------+
         |
         | Submit Leave Request
         v
+---------------------------+
| Leave Request Form        |
| (Custom Table & Form)     |
+---------------------------+
         |
         | Triggers
         v
+---------------------------+
|      Flow Designer        |
|  (Automation Workflow)    |
+---------------------------+
         |
         | Sends Approval
         v
+---------------------------+
|         Manager           |
|    Reviews Request        |
+---------------------------+
      |              |
      | Approve      | Reject
      |              |
      +------+-------+
             |
             v
+---------------------------+
| Update Leave Status       |
| (Approved / Rejected)     |
+---------------------------+
             |
             | Sends Notification
             v
+---------------------------+
|   Email Notification      |
+---------------------------+
             |
             v
+---------------------------+
|        Employee           |
| Receives Status Update    |
+---------------------------+
```

### Architecture Description

The Leave Approval Management System follows a workflow-driven architecture in which an employee submits a leave request through a custom ServiceNow form. The request is stored in a custom table and automatically triggers a Flow Designer workflow. The workflow sends an approval request to the assigned manager, who reviews and either approves or rejects the request. Based on the manager's decision, the system updates the leave request status and sends an automated email notification to the employee, ensuring a seamless and efficient leave management process.

## Configuration
## Key Configuration Areas

- **Application Settings:** Configure the scoped application and assign the required user roles.
- **Custom Table:** Define the Leave Request table with fields for employee, manager, leave details, and status.
- **Forms:** Design and configure the Leave Request form for employee submissions.
- **Approval Workflow:** Configure Flow Designer to automate the manager approval process.
- **Approval Rules:** Define the approval logic to route requests to the assigned manager.
- **Email Notifications:** Configure automated email alerts for leave approval and rejection.
- **User Roles:** Assign appropriate permissions to employees, managers, and administrators.
- **Status Management:** Configure automatic status updates based on the manager's approval decision.

## Testing

Comprehensive test cases and validation scenarios are included to ensure the Leave Approval Management System functions correctly. Test coverage includes:

- **Form Validation:** Verify that employees can submit leave requests with valid and complete information.
- **Approval Workflow Testing:** Test the Flow Designer workflow for manager approval and rejection scenarios.
- **Email Notification Testing:** Validate that employees receive email notifications after the manager's decision.
- **End-to-End Testing:** Verify the complete leave request lifecycle from submission to approval/rejection and status update.

## Troubleshooting

### Common Issues and Solutions

| Issue | Solution |
|--------|----------|
| Leave request is not triggering the workflow. | Verify that the Flow Designer trigger is active and configured correctly. |
| Manager does not receive the approval request. | Ensure the Manager field is populated and the approval action is configured properly. |
| Approval does not update the leave request status. | Check the flow logic and confirm the status update action is executed after approval or rejection. |
| Email notifications are not sent. | Verify that email notifications are enabled and configured correctly in the flow. |
| **My Approvals** is empty for the manager. | Confirm the user has the required roles and that the approval is assigned to the correct manager. |
| Users cannot access the application. | Verify that the appropriate roles and permissions have been assigned to the user. |

## Support & Maintenance

- **Documentation:** Refer to the **Project Documentation** section for detailed implementation and configuration guides.
- **Demonstration:** Review the **Project Demonstration** section to understand the complete leave request and approval workflow.
- **Issue Reporting:** Report bugs, issues, or enhancement requests through the project's GitHub repository.

---

## Future Enhancements

- Implement multi-level leave approval workflows.
- Add leave balance calculation and tracking.
- Develop an administrative dashboard with leave analytics and reports.
- Integrate with HR systems for employee data synchronization.
- Enable mobile access through the ServiceNow Mobile App.
- Add calendar integration for leave scheduling and reminders.
- Implement role-based dashboards and advanced reporting features.

---

## Contributing

To contribute to this project:

1. Fork the repository.
2. Create a new feature branch.
3. Make your changes and test them thoroughly.
4. Commit your changes with meaningful commit messages.
5. Submit a pull request with a detailed description of your changes.

---

## License

This project is provided for educational and learning purposes to demonstrate workflow automation using the ServiceNow platform.

---

## Authors & Contributors

**Project Developer:** Gayatri Pinakana

Contributions, feedback, and suggestions from mentors, faculty members, and the developer community are greatly appreciated.

---

## Acknowledgments

This project demonstrates the implementation of ServiceNow best practices for automating employee leave request and approval workflows. Special thanks to the ServiceNow Developer Program, official documentation, mentors, and learning resources that supported the successful development of this project.

---

**Last Updated:** June 2026

**Version:** 1.0

**Repository:** Leave-Approval-Management-System-ServiceNow
