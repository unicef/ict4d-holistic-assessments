---
description: Risky and vulnerability-prone areas of concern for software source code
---

# Source Code Conundrums

### Supply Chain Attacks

The source code lacks measures to mitigate supply chain attacks, such as using tools to control access to dependencies.

### Unsanitized Query Inputs

Some query inputs are not sanitized or insufficiently sanitized, creating the possibility of SQL injection attacks.

### Hard-Coded Credentials

The source code or configuration files contain hard-coded credentials, presenting a security risk.

### Inadequate Exception Handling

Exception handling is not properly configured for log auditing, reducing the chances of detecting intrusions and other errors.

### Unsafe Database Access

The application logs directly into the database instead of using a separate append-only microservice, allowing for manipulation of the log if attackers gain write access to the database.

### Unsafe Authentication Access

The application directly accesses the database of Keycloak, bypassing the security benefits of using Keycloak as an authentication microservice.

### &#x20;Proprietary Dependencies

Proprietary dependencies in the Gradle build configuration elevate the risk of unauthorized access and manipulation.
