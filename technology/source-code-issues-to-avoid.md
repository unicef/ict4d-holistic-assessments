# Source Code Issues to Avoid

### Lack of Automated and Manual Testing

Multiple sources mention the absence of both automated and manual testing in the source code, raising concerns about the robustness and reliability of the software.

### Unsanitized Query Inputs

Some query inputs are not sanitized or insufficiently sanitized, creating the possibility of SQL injection attacks.

### Hard-Coded Credentials

The source code contains hard-coded credentials, presenting a security risk.

### Inadequate Exception Handling

Exception handling is not properly configured for log auditing, reducing the chances of detecting intrusions and other errors.

### Supply Chain Attacks

The source code lacks measures to mitigate supply chain attacks, such as using tools to control access to dependencies.

### Unsafe Database Access

The application logs directly into the database instead of using a separate append-only microservice, allowing for manipulation of the log if attackers gain write access to the database.

### Unsafe Authentication Access

The application directly accesses the database of Keycloak, bypassing the security benefits of using Keycloak as an authentication microservice.

### Embedded Credentials and Proprietary Dependencies

Embedded credentials and proprietary dependencies in the Gradle build configuration elevate the risk of unauthorized access and manipulation.

**Recommendations to Mitigate:**

* Develop Manual Test Plans and Implement Automated Testing: Create manual test plans and implement automated testing to improve code quality and identify vulnerabilities.
* Sanitize All Query Inputs: Ensure all query inputs are properly sanitized to prevent SQL injection attacks.
* Remove Hard-Coded Credentials: Eliminate hard-coded credentials from the source code to reduce security risks.
* Improve Exception Logging: Configure exception handling for proper log auditing to facilitate intrusion detection and error identification.
* Implement Defenses against Supply Chain Attacks: Employ tools and practices to control access to dependencies and mitigate supply chain attacks.
* Address Unsafe Database Access and Authentication Service Access: Establish a separate append-only microservice for database logging and avoid direct access to the Keycloak database to enhance security.
* Remove Embedded Credentials and Proprietary Dependencies: Eliminate embedded credentials and proprietary dependencies to reduce the risk of unauthorized access and manipulation.
