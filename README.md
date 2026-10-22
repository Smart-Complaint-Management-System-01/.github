# Smart Complaint Management System

A web-based complaint management platform designed to provide a centralized mechanism for lodging, tracking, managing, and resolving complaints.

The system provides separate functionality for complainants/users and administrators, with role-based access control, complaint tracking, assignment, resolution management, search and filtering, and status notifications.

## Project Overview

The Smart Complaint Management System aims to replace unstructured complaint handling with a centralized digital platform.

A registered user can:

- Create an account and log in
- Lodge a complaint
- Receive a unique complaint ID
- Track the current status of a complaint
- View complaint history and updates
- Receive notifications when significant status changes occur

Administrators can:

- View and manage submitted complaints
- Search and filter complaints
- Assign complaints to an appropriate administrator or department
- Update complaint status
- Add complaint updates
- Record resolution details
- Mark complaints as resolved

The system also incorporates authentication, role-based authorization, secure password storage, session management, data persistence, and input validation.

## Key Features

### User Management
- User registration
- User authentication
- Role-based access control
- Secure password storage
- Session management

### Complaint Management
- Complaint submission
- Unique complaint ID generation
- Complaint categorization
- Complaint status tracking
- Complaint history
- Complaint updates
- Complaint assignment
- Complaint resolution

### Search and Monitoring
- Search complaints by complaint ID
- Filter complaints by category
- Filter complaints by status
- Filter complaints by submission date

### Notifications
- In-application notifications for significant complaint status changes

### Security
- Authentication for protected operations
- Role-based authorization
- Password hashing
- Session invalidation on logout
- Server-side input validation
- Protection of complaint data from unauthorized access

## Technology Stack

| Component | Technology |
|-----------|------------|
| Frontend | HTML5, CSS, JavaScript |
| Backend | Python, Django |
| Architecture | Django MVT |
| Database | MySQL |
| ORM | Django ORM |
| Authentication | Django Authentication System |
| Version Control | Git / GitHub |
| Diagrams | draw.io |

## System Architecture

The system follows a web-based architecture consisting of the following major components:

```text
                    ┌──────────────────┐
                    │    Web Browser   │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │   Django Web UI  │
                    └────────┬─────────┘
                             │
                             ▼
                 ┌─────────────────────────┐
                 │     Django Backend      │
                 │                         │
                 │  Authentication & RBAC  │
                 │  Complaint Management   │
                 │  Search & Filtering     │
                 │  Notifications          │
                 └────────────┬────────────┘
                              │
                              ▼
                       ┌─────────────┐
                       │    MySQL    │
                       │   Database  │
                       └─────────────┘
