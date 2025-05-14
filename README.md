# chatApp2
The Admin Portal is a secure, web-based administrative console that provides a user-friendly interface for configuring, managing, and monitoring various components of the R-Switch payment platform. It serves as a centralized hub for administrators, enabling them to efficiently perform key tasks such as adapter setup, workflow and routing rule management, system configuration, deployment scheduling, and real-time system monitoring—all from a single point of access.

Through this intuitive portal, users can easily configure L1 (inbound) and L3 (outbound) adapters, define complex workflows and routing rules, schedule and deploy changes, and oversee the entire system’s performance. The Admin Portal also provides access to real-time transaction logs, system dashboards, and import/export tools, facilitating operational transparency, compliance, and faster troubleshooting.

Designed with ease of use and scalability in mind, the Admin Portal streamlines administrative operations, reduces configuration complexity, and empowers users with complete control over the R-Switch ecosystem—without the need for manual scripts or backend interventions.

Key Features:

Dashboard: Visualize transaction trends and system performance through interactive charts.

Monitoring: Track real-time health of adapters, engines, and security components.

Transaction Logs: Audit and filter past transactions for analysis and compliance.

Configuration Management: Set up BINs, tags, lookup values, and adapter parameters.

Import/Export & Backup: Backup, migrate, or restore settings across environments.
# 🏢 switch-admin-portal
The **Rswitch Admin Portal** is a web-based platform that allows administrators to manage configurations, monitor transactions, and control user access. It features a user-friendly UI for the Rswitch system, built with a Spring Boot backend and an Angular frontend, enabling seamless system management and real-time monitoring.

---

## 📦 Project Structure

This project is divided into below  modules:


## Admin Portal Modules

### 1. HsbcMvpAdminAngularBackend
- **Technology:** Spring Boot  
- **Description:** Handles all backend operations for the admin portal, including:
  - Business logic processing
  - Data management
  - Integration with internal services and databases

### 2. HsbcMvpAdminAngularFrontend
- **Technology:** Angular  
- **Description:** Provides a responsive and user-friendly web interface for administrators to:
  - Monitor system activity
  - Manage users and settings
  - Perform admin-specific operations via a secure UI


---

## 🛠️ Tools Needed

Make sure you have the following tools installed:

| Tool | Version |
|------|---------|
| Java | JDK 21 |
| Node.js | 18.20.7 |
| Angular CLI | 15.2.11 |
| MySQL | Latest |
| Git | Latest |
| IDE | VS Code / IntelliJ / any other preferred IDE |

---

## 🏗️ Build Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/BNT-Cennox/switch-admin-portal.git
```

### 2. Open the Project in IDE
- Open your IDE (VS Code / IntelliJ)
- Load the project folder
  
### 3. Build Backend Project
Open your terminal and navigate to the root project directory (switch-admin-portal).

- Open terminal and Navigate to the ```root project/``` directory.(switch-admin-portal).
- Build the  project using:
```bash
gradle clean build
 ```
---

## 🚀 Run Instructions

### 1. Create MySQL Database
Open MySQL Workbench or CLI and execute:
```bash
CREATE DATABASE rswitchadminportal;
```
_⚠️Ensure MySQL is running and accessible.

### 2. Configure Database 

Navigate to the ``` switch-admin-portal\HsbcMvpAdminAngularBackend\src\main\resources\application.properties``` directory.
Locate the application.properties or application.yml file.

_⚠️Verify that the MySQL database credentials (username, password, port, database name) in this configuration file match your local MySQL setup. Update them if necessary to connect to the renoatmserver database you just created.

### 3. Run Backend Project (HsbcMvpAdminAngularBackend)
- After a successful Step 2, Navigate to the ```switch-admin-portal\HsbcMvpAdminAngularBackend``` directory and to excecute below commands:
```bash
./gradlew bootRun
```
-Alternatively,Run the main class of the Spring Boot application.



### 4. Run Frontend Project
- Navigate to the **switch-admin-portal\HsbcMvpAdminAngularFrontend** directory.
- Install dependencies:
```bash
npm install
```
- Start Angular App
```bash
ng serve
```
- Access the UI in your browser:
👉 http://localhost:4200



