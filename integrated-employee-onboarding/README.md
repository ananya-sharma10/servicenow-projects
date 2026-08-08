# Integrated Employee Onboarding System

## Overview

The Integrated Employee Onboarding System is a ServiceNow workflow automation project designed to streamline the onboarding of new employees across HR, IT, and Facilities teams.

The system uses a centralized onboarding request to automatically coordinate the tasks and approvals required before an employee joins the organization.

## Reference Screenshots

The following screenshots are representative ServiceNow interfaces related to the workflow concepts demonstrated in this project.

### 1. Onboarding Catalog Item

![Onboarding Catalog Item](screenshots/01-onboarding-catalog.jpg)

### 2. Onboarding Workflow

![Onboarding Workflow](screenshots/02-onboarding-catalog.jpg)

### 3. Requested Item (RITM)

![Requested Item](screenshots/03-onboarding-catalog.jpg)

### 4. Generated Tasks

![Generated Tasks](screenshots/04-onboarding-catalog.jpg)


## Workflow

Employee Onboarding Request
→ Manager Approval
→ HR Tasks + IT Tasks + Facilities Tasks
→ Welcome Notification
→ Onboarding Completed

## Key Features

- Employee onboarding request through Service Catalog
- Manager approval workflow
- Automated task creation for HR, IT, and Facilities
- Requested Item (RITM) tracking
- Automated task assignment
- Employee onboarding status tracking
- Completion notification

## ServiceNow Technologies Used

- Service Catalog
- Catalog Items
- Flow Designer
- Requested Items (RITMs)
- Catalog Tasks
- Service Portal
- Notifications
- Workflow Automation

## Project Workflow

### 1. Onboarding Request

A manager submits an onboarding request containing employee information such as:

- Employee name
- Start date
- Department
- Employment type
- Work location
- Manager

### 2. Approval

The request is routed for manager approval before onboarding activities begin.

### 3. Automated Task Creation

Once approved, the workflow automatically generates tasks for:

- HR — employee documentation and records
- IT — account and equipment provisioning
- Facilities — workspace and access setup

### 4. Progress Tracking

The onboarding request and generated tasks can be tracked through their respective ServiceNow records.

### 5. Completion

Once the required activities are completed, the workflow sends a confirmation notification and marks the onboarding process as complete.

## Project Architecture

```text
Service Catalog
      │
      ▼
Onboarding Request
      │
      ▼
Manager Approval
      │
      ▼
Flow Designer
      │
 ┌────┼────┐
 ▼    ▼    ▼
 HR   IT   Facilities
 │    │    │
 └────┼────┘
      ▼
Welcome Notification
      │
      ▼
Onboarding Complete
```

## Portfolio Note

The interface visuals included in this repository are conceptual portfolio mockups created to represent the project's workflow and functionality. They are not screenshots exported from a currently active ServiceNow instance.

## What I Learned

This project provided practical experience with ServiceNow workflow automation, Service Catalog requests, Flow Designer, task orchestration, approvals, and cross-team process automation.
