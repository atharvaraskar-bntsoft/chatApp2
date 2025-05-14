# chatApp2
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



