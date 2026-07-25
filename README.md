# Online Examination System

A Java web application for creating, delivering, and grading online examinations. The project provides separate student and faculty experiences, reusable question banks, timed assessments, automated grading, and performance reporting.

## Features

### Faculty workflow

- Create and manage examinations
- Build reusable question banks
- Configure public or private assessments
- Set examination timers and availability rules
- Randomise questions
- Review student attempts and performance statistics

### Student workflow

- Sign in with an institutional account
- View available assessments
- Complete timed examinations
- Receive automatically calculated results
- Review examination history and performance information

## Technology

- Java EE / Jakarta-style Servlets
- JSP
- HTML, CSS, and JavaScript
- Microsoft SQL Server
- Apache Tomcat
- Ant / NetBeans project structure

## Local setup

### Prerequisites

- JDK 8 or later
- Apache Tomcat or another compatible servlet container
- Microsoft SQL Server
- Microsoft JDBC Driver for SQL Server
- Ant or NetBeans

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ICARUSTUDIO/Online-Examination-System.git
   cd Online-Examination-System
   ```

2. Create a SQL Server database named `ExamPortal`.

3. Configure the database connection used by the application. For a production-quality deployment, move connection values out of servlet source code and load them from environment variables or server-managed configuration.

4. Add the Microsoft SQL Server JDBC driver to the project or servlet container.

5. Build and deploy the `ExamPlatform` application to Tomcat.

6. Open the application at a URL similar to:

   ```text
   http://localhost:8080/ExamPlatform/Login.jsp
   ```

## Roles

- **Student:** takes examinations and views results.
- **Faculty:** creates assessments, manages questions, and reviews performance.

Registration is intended to be controlled by authorised staff rather than exposed as unrestricted public self-registration.

## Repository notes

This project uses an older Java web stack to demonstrate servlet routing, JSP rendering, role-based application flows, SQL Server integration, session handling, and automated assessment logic. It is presented as a portfolio and learning project rather than a production examination platform.

Before production use, add centralised configuration, password hashing with a current adaptive algorithm, CSRF protection, stricter authorisation checks, automated tests, audit logging, and a clean build pipeline.

## License

This project is available under the [MIT License](LICENSE).

## Contact

Oluwatobi Obafemi — [tobyfemi55@gmail.com](mailto:tobyfemi55@gmail.com)
