# Case Verification Management System using Salesforce

##  Project Overview

The **Case Verification Management System** is a Salesforce-based customer support solution that searches published Knowledge Articles before creating a support Case. It helps reduce duplicate Cases and enables customers to resolve common issues using existing solutions.

##  Problem Statement

Support teams often receive repetitive Cases for issues that already have solutions in published Knowledge Articles. This project addresses the problem by verifying existing solutions before creating a new Case.

##  Key Features

- **Knowledge Article Search:** Searches published Knowledge Articles for relevant troubleshooting solutions.
- **Problem Verification:** Uses a Salesforce Screen Flow to capture issue details and guide customers through the verification process.
- **Conditional Case Creation:** Creates a Case only when no matching article is found or the suggested solution does not resolve the issue.
- **Duplicate Case Prevention:** Avoids creating a new Case when the existing solution resolves the customer's problem.
- **Automated Notifications:** Notifies the customer after a Case is created.
- **Customer Support App:** Provides a centralized Lightning app with Cases, Knowledge, Reports, Dashboards, and a Ticket page.

##  Technologies Used

- Salesforce CRM
- Salesforce Flow Builder
- Salesforce Knowledge
- Lightning App Builder
- Salesforce Cases, Contacts, and Users
- Get Records, Decision, Create Records, and Screen Flow elements

##  Workflow

1. The customer enters the problem description, issue category, and email address.
2. The Screen Flow searches published Knowledge Articles.
3. If a matching article is found, its solution is displayed to the customer.
4. If the solution is helpful, the Flow ends without creating a Case.
5. If the solution is not helpful, the customer proceeds to Case creation.
6. If no matching article is found, a Case is created directly.
7. The customer receives a notification confirming Case creation.

##  Salesforce Components

| Component | Purpose |
|---|---|
| Screen Flow | Captures problem details and controls the verification process |
| Knowledge Articles | Stores published troubleshooting solutions |
| Get Records | Retrieves matching Knowledge Articles |
| Decision | Determines the next step based on search results and customer feedback |
| Create Records | Creates a Case when required |
| Notification Action | Notifies the customer after Case creation |
| Customer Support App | Provides the central support workspace |
| Ticket Page | Hosts the verification Screen Flow |

##  Testing Scenarios

- Validate required input fields.
- Verify retrieval of matching published Knowledge Articles.
- Confirm that a helpful solution does not create a Case.
- Confirm that an unhelpful solution leads to Case creation.
- Verify Case creation when no matching article is found.
- Validate Case field mapping and customer notifications.

##  Project Outcome

The system streamlines customer support by encouraging self-service resolution, reducing unnecessary Case creation, and automating the process of handling unresolved customer issues through Salesforce Flow.

##  Future Enhancements

- Improve Knowledge Article matching using advanced search techniques.
- Add dashboards to analyze Case volume and resolution trends.
- Introduce additional automation for Case assignment and escalation.
- Enhance customer feedback collection.

##  Project Type

Salesforce Administration and Automation Project

**Domain:** Customer Support Management
