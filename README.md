# CRM Desktop Application

## Customer Relationship Management System

A structured CRM desktop application built using **C# Windows Forms** and **SQL Server**, following a **3-Tier Architecture** approach.

The system is designed to manage clients, application users, and permission-based access while maintaining a clear separation between the presentation, business logic, and data access layers.

---

# Developed By

## Zynox Tech

**Website:** https://zynoxtech.site
**Email:** [hello@zynoxtech.site](mailto:hello@zynoxtech.site)
**Location:** Abbottabad, Pakistan

Zynox Tech is a software development company specializing in:

* Enterprise Software Solutions
* Web Applications
* Mobile Applications
* Artificial Intelligence Solutions
* Custom Business Automation Systems

We build scalable, reliable, and user-focused technology solutions that help businesses improve efficiency and digital operations.

For software development services and technology partnerships:

**Website:** https://zynoxtech.site
**Email:** [hello@zynoxtech.site](mailto:hello@zynoxtech.site)

---

# Project Overview

The **CRM Desktop Application** is a Customer Relationship Management system designed to manage clients and system users through a structured Windows desktop environment.

The system allows users to maintain customer information and control access to different parts of the application through a permission-based user management system.

The project includes:

* Database design
* Application architecture
* Business logic implementation
* Windows Forms user interface
* Client management
* User administration
* Permission-based access control

The application was developed to demonstrate the design and implementation of a structured desktop application using a multi-layer architecture.

---

# Architecture

The application follows a **3-Tier Architecture** that separates application responsibilities into dedicated layers.

```text
Presentation Layer
        ↓
Business Layer
        ↓
Data Access Layer
        ↓
SQL Server Database
```

This architecture improves code organization, maintainability, and separation of concerns.

---

## Presentation Layer

The Presentation Layer is developed using **Windows Forms** and handles application interfaces and user interaction.

The layer includes:

* Login interface
* Client management forms
* User management screens
* Permission management interfaces
* Input validation
* Application navigation

The user interface communicates with the database through the Business Layer.

---

## Business Layer

The Business Layer contains the core application logic.

Responsibilities include:

* Client data validation
* User management operations
* Permission checks
* Application workflow management
* Coordination between the UI and Data Access Layer

This layer separates business rules from the user interface and database implementation.

---

## Data Access Layer

The Data Access Layer manages communication with the **SQL Server database**.

Responsibilities include:

* Executing SQL queries
* Reading database records
* Writing application data
* Managing database connections
* Processing database operations

This layer isolates database functionality from the rest of the application.

---

# Main Features

## Login and Authentication

The application provides a database-backed login system.

Authentication functionality includes:

* User authentication
* Login validation
* Database-based user verification
* Permission-based access control

Users are granted access to application functionality according to their assigned permissions.

---

## User Management

The user management system allows administrators to manage application users.

Features include:

* Add new users
* View users
* Find users
* Update users
* Delete users
* Manage user permissions

The system provides dedicated Windows Forms for different user management operations.

---

## Permission Management

The CRM application includes a permission-based access system.

Permissions can be assigned to users to control access to different application functionality.

This provides a basic access control mechanism for managing system users.

---

## Client Management

The client management module provides functionality for maintaining customer records.

Features include:

* Add new clients
* View client records
* Update client information
* Delete clients
* Search for clients

The system provides dedicated interfaces for individual client operations.

---

## Client Search

Users can search for stored client records through the client search interface.

This allows users to quickly locate customer information maintained within the CRM database.

---

## Data Validation

The application includes basic input validation.

Validation functionality helps:

* Reduce invalid input
* Maintain structured records
* Improve data consistency
* Prevent incomplete data processing

---

# Application Screenshots

Explore the desktop interfaces, client management functionality, user administration tools, and permission system of the **CRM Desktop Application**.

## Login and Main Application Interface

<p align="center">
  <img src="https://github.com/user-attachments/assets/975865b6-c053-46a0-87f8-41474821aa84" alt="CRM Application Interface" width="45%" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/0ec74afe-86ca-482a-8c21-3f826350c19a" alt="CRM Main Interface" width="45%" />
</p>

## Client Management

<p align="center">
  <img src="https://github.com/user-attachments/assets/b3aa1b18-baf6-4a00-b5c8-ddc8d51ab888" alt="CRM Client Management" width="45%" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/12b9d463-6a26-44ec-a044-7b0a95baa7e2" alt="CRM Client Records" width="45%" />
</p>

## User and Permission Management

<p align="center">
  <img src="https://github.com/user-attachments/assets/0524f063-8c1a-4beb-a570-d0adedb472c5" alt="CRM User Management" width="45%" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/64ad9750-0bc7-4bdb-a026-4da473a05f3f" alt="CRM Permission Management" width="45%" />
</p>

---

# Database

The application uses **Microsoft SQL Server** for structured data storage.

The database maintains client records, system users, and application permissions.

---

## Clients Table

The Clients table stores customer information including:

* ClientID
* ClientName
* Phone
* Email
* TotalOrders
* TotalPurchaseValue

This table maintains customer-related CRM records.

---

## Users Table

The Users table stores system user information and access permissions.

Stored information includes:

* UserID
* UserName
* FullName
* Email
* Password
* Permissions

The permission field is used by the application to manage user access.

---

# Database Setup

The database schema and sample data are included in:

```text
Database/CRMproject.sql
```

Running the SQL script creates:

* CRM database
* Required database tables
* Database structure
* Sample testing data

---

# Technology Stack

## Application Development

* C#
* .NET Framework

## Desktop User Interface

* Windows Forms
* WinForms Controls

## Database

* Microsoft SQL Server
* SQL

## Data Access

* ADO.NET
* SQL Server Connections

## Architecture

* 3-Tier Architecture
* Presentation Layer
* Business Layer
* Data Access Layer

---

# Application Architecture

The project separates application functionality into dedicated layers.

```text
Windows Forms UI
        ↓
Business Logic
        ↓
Data Access Components
        ↓
ADO.NET
        ↓
SQL Server Database
```

The architecture helps isolate interface logic, application rules, and database operations.

---

# Project Structure

The project is organized into multiple modules that separate user interfaces, business logic, data access, settings, and database scripts.

```text
CRM-WinForms-App/

├── BusinessLayer/
│   ├── ClsBusinessLayer.cs
│   └── BusinessLayer.csproj
│
├── ClsClient/
│   ├── ClsClient.cs
│   └── ClsClient.csproj
│
├── ClsDataAccessSettings/
│   ├── ClsDataAccessSettings.cs
│   └── ClsDataAccessSettings.csproj
│
├── ClsDataLayer/
│   ├── ClsDataLayer.cs
│   └── ClsDataLayer.csproj
│
├── ClsUser_Person/
│   ├── ClsUser.cs
│   └── Related project files
│
├── Database/
│   └── CRMproject.sql
│
├── Screenshots/
│   ├── login.png
│   ├── add_user.png
│   ├── client_list.png
│   ├── remove_user.png
│   ├── search_client.png
│   └── user_roles.png
│
├── Settings/
│   ├── Settings.cs
│   └── Settings.csproj
│
├── frmAddNewClient/
├── frmAddNewUser/
├── frmDeleteUser/
├── frmFindUser/
├── frmMainScreen/
├── frmManageUsers/
├── frmPermissions0/
├── frmRemoveClient/
├── frmSearchClient/
├── frmUpdateClient(After FindUser First)/
├── frmUpdateClient/
├── frmUpdateUser0/
├── frmViewClients/
├── frmViewUsers/
│
├── App.config
├── CRM.sln
└── README.md
```

This structure reflects the modular organization of the application.

Each functional area is separated into dedicated projects or components while business logic and data access operations remain isolated within their respective layers.

---

# Installation and Setup

## Requirements

Before running the project, install:

* Visual Studio
* .NET Framework development tools
* Microsoft SQL Server
* SQL Server Management Studio
* Git

---

# Clone the Repository

Clone the project using Git:

```bash
git clone https://github.com/Zynox-Tech/CRM-WinForms-App.git
```

Navigate to the project directory:

```bash
cd CRM-WinForms-App
```

---

# Create the Database

Open **SQL Server Management Studio (SSMS)**.

Locate the SQL script:

```text
Database/CRMproject.sql
```

Open and execute the script.

The script creates the required database structure and testing data.

---

# Configure the Database Connection

Open:

```text
App.config
```

Update the SQL Server connection string according to your environment.

Example:

```xml
<connectionStrings>
  <add name="CRMConnection"
       connectionString="Server=.;Database=CRMproject;Trusted_Connection=True;"
       providerName="System.Data.SqlClient"/>
</connectionStrings>
```

Ensure that the server and database configuration match your local SQL Server environment.

---

# Open the Solution

Open the Visual Studio solution:

```text
CRM.sln
```

Visual Studio will load the CRM projects and application components.

---

# Set the Startup Project

Inside Visual Studio:

1. Locate the executable Windows Forms project.
2. Right-click the project.
3. Select:

```text
Set as Startup Project
```

This ensures Visual Studio launches the CRM desktop application instead of a class library.

---

# Run the Application

Press:

```text
F5
```

Alternatively, click **Start** inside Visual Studio.

The CRM desktop application will launch and connect to the configured SQL Server database.

---

# Demo Video

A demonstration video of the CRM Desktop Application is available at:

https://bit.ly/CRM-System-Demo

The demo provides an overview of the application's interface and core CRM functionality.

---

# Troubleshooting

## Application Cannot Connect to Database

Ensure that:

* SQL Server is running
* The database script has been executed
* The database exists
* The connection string in `App.config` is correct
* The SQL Server instance name is correctly configured

---

## Class Library Cannot Be Started Directly

If Visual Studio displays:

```text
Class Library cannot be started directly
```

The incorrect project has been selected as the startup project.

Locate the executable Windows Forms project and select:

```text
Set as Startup Project
```

Run the application again.

---

# Security Considerations

The current project demonstrates a structured CRM architecture and basic permission management.

Production implementations should consider:

* Password hashing
* Secure credential storage
* Parameterized SQL queries
* Role-based access control
* Database access restrictions
* Audit logging
* Secure connection string management

Sensitive database credentials should not be committed to public source control.

---

# Future Improvements

Possible future enhancements include:

* Password hashing and secure authentication
* Advanced role-based access control
* Improved permission management
* Advanced client search and filtering
* Customer interaction history
* Sales and order management
* CRM analytics dashboard
* Business reporting
* Data export functionality
* Improved user interface design
* Audit logging
* Cloud database integration

---

# Contributing

Contributions, feature suggestions, and improvements are welcome.

To contribute:

1. Fork the repository.
2. Create a new feature branch.

```bash
git checkout -b feature/AmazingFeature
```

3. Commit your changes.

```bash
git commit -m "Add AmazingFeature"
```

4. Push the branch.

```bash
git push origin feature/AmazingFeature
```

5. Open a Pull Request.

---

# License

This project's use, modification, and distribution are subject to the license terms provided with the repository.

Review the repository license before using the project in commercial or redistributed software.

---

# About Zynox Tech

Zynox Tech builds modern and scalable software solutions for businesses and organizations.

Our services include:

* Custom Software Development
* Enterprise Applications
* Desktop Applications
* Mobile Applications
* Web Platforms
* AI-Powered Solutions
* Business Automation Systems

We focus on developing reliable, scalable, and user-centered technology solutions.

For custom software solutions and technology partnerships:

**Website:** https://zynoxtech.site
**Email:** [hello@zynoxtech.site](mailto:hello@zynoxtech.site)
**Location:** Abbottabad, Pakistan

---

<div align="center">

### Developed by **Zynox Tech**

**Building Modern Technology Solutions for Businesses and Organizations**

</div>
