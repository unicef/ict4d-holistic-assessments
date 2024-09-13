---
description: Risky and vulnerability-prone areas of concern for software source code
---

# Source Code Conundrums

{% hint style="success" %}
Most relevant for 🔍 [Technical Evaluators](../get-started.md#evaluating)
{% endhint %}

The insights below on how best to protect and secure data, inputs, and actions through source code development best practices, were aggregated from the results of the [4 holistic assessments on partner solutions](../partners/partner-assessments/) performed as part of this process.

## _<mark style="background-color:yellow;">Without proper access controls or vetting mechanisms, malicious code could be introduced into the software through compromised or unsafe dependencies.</mark>_&#x20;

Source code can lack measures to mitigate supply chain attacks, such as using tools to control access to dependencies. Supply chain attacks occur when an attacker exploits vulnerabilities in the supply chain network to gain unauthorized access to systems or data. One common entry point for such attacks in software development is through external libraries or dependencies that the software relies on. This could happen if dependencies are automatically updated to compromised versions without prior security checks or if dependencies are sourced from unverified or insecure repositories.

Effective mitigation strategies could include [implementing tools](../resources-links-and-tools/) that enforce strict version control and [dependency review](../process/software-bill-of-materials.md) (SBOM!) processes. These tools can automate the tracking of each dependency's origin, monitor its integrity, and ensure that it has not been tampered with before integration into the main codebase. Setting up a secure, curated list of approved libraries and enforcing digital signatures for any code changes or updates can further protect against such attacks. These measures not only prevent unauthorized access but also help in maintaining a clean, secure development environment.&#x20;

## _<mark style="background-color:yellow;">When query inputs are not properly sanitized, these malicious inputs can bypass security mechanisms.</mark>_

The lack of sufficient input sanitization in some query mechanisms significantly heightens the risk of SQL injection attacks, a critical security vulnerability in database-driven applications. SQL injection involves the insertion of malicious SQL statements into an entry field for execution, typically with the intent to manipulate or exploit the database. When query inputs are not properly sanitized, these malicious inputs can bypass security mechanisms, allowing attackers to access, modify, or delete data, potentially exposing sensitive information or corrupting the database contents.

Sanitizing inputs involves checking, cleaning, and confirming that each input adheres strictly to the expected format, thus preventing any part of the input from being interpreted as SQL code. Implementing parameterized queries is one effective method of sanitization, where SQL code is defined first and user inputs are then passed as parameters, never as raw SQL code. Additionally, employing web application firewalls (WAFs) and regular security audits can further shield databases from SQL injection attacks by detecting and mitigating possible injection attempts and vulnerabilities.&#x20;

## _<mark style="background-color:yellow;">Hard-coded credentials are essentially fixed usernames and passwords embedded directly into application code or configuration settings.</mark>_

The presence of hard-coded credentials, whether passwords or API keys, within source code or configuration files presents a serious security risk, as it compromises the integrity and confidentiality of the system. They can easily be extracted by malicious actors, especially if the code is exposed or leaked. This practice creates a vulnerability point that can be exploited to gain unauthorized access to systems, databases, or network devices, bypassing security mechanisms designed to protect sensitive data and operations.

Instead, credentials should be stored in secure, encrypted configuration files or secure vaults that are accessed dynamically by the application at runtime. Additionally, the use of environment variables to manage credentials securely outside the application's codebase can also be an effective strategy. These measures not only help in safeguarding access to the system but also facilitate easier management of credentials, such as updates or revocations, without the need to modify the source code directly.&#x20;

## _<mark style="background-color:yellow;">When exceptions are not adequately logged, vital clues that could indicate a security breach or system malfunction might be missed.</mark>_&#x20;

The improper configuration of exception handling within log auditing systems significantly undermines the effectiveness of security measures, reducing the likelihood of timely detection of intrusions and other critical errors. Log auditing is a fundamental component of cybersecurity, as it provides a historical record of events that can be analyzed to detect anomalous behavior or unauthorized access attempts.&#x20;

This can leave the system vulnerable to continued exploitation without detection, as security teams lack the necessary data to identify and respond to threats effectively. The resolution involves setting up robust logging mechanisms that capture all exceptions, including detailed stack traces and contextual information that can help in diagnosing issues. Furthermore, these logs should be regularly reviewed and analyzed using automated tools that can flag unusual patterns or signs of potential security incidents. Implementing such practices not only aids in the early detection of issues but also helps in maintaining system integrity and availability by enabling prompt and informed responses to various operational and security challenges.

## _<mark style="background-color:yellow;">By logging in directly to a database that allows read and write operations, the application essentially leaves a backdoor open for potential manipulation, undermining the reliability of the logs as a tool for forensic analysis and compliance.</mark>_

Logging directly into a database instead of using a dedicated, append-only microservice for log management can introduce significant security vulnerabilities, particularly if attackers gain write access to the database. In such scenarios, the integrity of the logs is compromised as malicious actors could alter or delete logs to cover their tracks, making it difficult to trace unauthorized actions or breaches. This approach lacks the robustness of an immutable logging system where once data is entered, it cannot be changed, ensuring a higher degree of accountability and traceability.&#x20;

To address this vulnerability, implementing an append-only microservice for handling logs can significantly enhance security. This method ensures that logs are stored in a manner where they cannot be altered or deleted once written. Such a microservice acts as a protective layer that isolates log data from the operational databases and enforces strict controls on how log data is handled and accessed. Moreover, using a microservice for logging can also improve scalability and performance by offloading the data-intensive task of log management from the main database, allowing both systems to operate more efficiently. Integrating comprehensive logging practices with robust access controls and regular audits can further solidify the security framework, ensuring that the logs remain an accurate and reliable source of information for detecting and investigating security incidents.

## _<mark style="background-color:yellow;">Without an Application Programming Interface (API) intermediary, the application exposes itself to a higher risk of data breaches, as the underlying database becomes a direct target for attacks.</mark>_&#x20;

Directly accessing the database of an authentication server rather than interfacing through an API as an authentication microservice presents significant security risks. This practice bypasses the layers of security that APIs provide, such as rate limiting, authentication, and encryption, which are designed to protect data integrity and confidentiality. APIs serve as a controlled gateway for data access, ensuring that only valid and authorized requests are processed.&#x20;

Additionally, direct database access can complicate compliance with data protection regulations, which often require stringent data access controls and auditing capabilities that APIs are better equipped to handle. Implementing an API-based microservice architecture would not only enhance security but also improve the scalability and maintainability of the system by clearly defining access protocols and reducing direct dependencies on the database structure.

## _<mark style="background-color:yellow;">Proprietary component dependencies can often be black boxes with undisclosed vulnerabilities, which malicious actors could exploit to compromise the build process or the application itself.</mark>_&#x20;

The use of proprietary dependencies in a build configuration can significantly increase the risk of unauthorized access and manipulation, as these dependencies might not undergo the same level of scrutiny and security testing as open-source counterparts.&#x20;

Moreover, reliance on proprietary dependencies limits transparency and makes it challenging to perform comprehensive security audits. It is essential for developers to implement strict access controls and continuously monitor these dependencies for any security updates or patches. Additionally, wherever possible, substituting proprietary dependencies with well-supported, open-source alternatives can enhance security by leveraging the broader community for security vetting and faster vulnerability resolution.
