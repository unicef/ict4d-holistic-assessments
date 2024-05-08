# Our Iterative Process

An iterative process is a way of working through a project by repeatedly refining and improving upon it through a series of cycles or iterations. In software development, this process is often used as a way to manage the complexity of creating large, complex software systems. Using an iterative process allows the team to focus on small, manageable chunks of work at a time, which helps to reduce the risk of errors and makes it easier to manage the complexity of the project. It also allows the team to gather feedback from stakeholders and users throughout the process, which can be used to refine and improve the project as it progresses.&#x20;

Some of the guidelines we will follow to achieve this are:

1. Be transparent and engaged with all stakeholders through open systems and communication
2. Share results and outputs, early and often for feedback
3. Debrief and reflect upon the quality of outcomes and outputs, to inform, revise, and improve subsequent iterations of the work



## Audit Steps and Timeline

Our iterative evaluation approach follows a set of tasks and engagements that include the vendor to foster transparency and accuracy of produced and shared findings. Many of these tasks happen in parallel. We begin with introductions and laying a foundation of trust.&#x20;

* Initial introduction email (our PM Lead introduces us to the vendor contact)
* Schedule a kickoff call with the vendor and demo of the solution when possible
* Create an established communications channel and share asset request list with vendor
  * _Tip: It is helpful to choose a communication channel that already exists in the vendor workflow to ease any burden of communication_
* &#x20;Create a shared google drive folder for ease of document uploading and sharing of Assets and any additional resources the vendor deem useful (case studies, security audits, SBOM, independent reports, etc.).

Furthermore, is important to us that we engage with vendors regarding found vulnerabilities or bugs. After each step in the process we share an evaluation update with the vendor and UNICEF and allow feedback so the process can be iterative and accurately reflect a relevant and up-to-date solution.&#x20;

Our disclosure approach includes:&#x20;

* Ethically disclose vulnerabilities or bugs to vendors&#x20;
  * After each Step (Assessment/Audit), Guardian Project will disclose any vulnerabilities or bugs found to the vendor through an agreed upon communication channel (email, slack, Signal, Github or issue tracker).
  * This will be done in a secure, confidential manner agreed upon by the vendor and auditor (Guardian Project)
* Negotiate with vendors regarding the complexity of a fix and timeline
* Based on the complexity, determine how Guardian Project will update their evaluation report accordingly (ie- a vulnerability is disclosed, but not fixed, a fix is in process, a resulting evaluation of a fix)



## Audit Steps

* **Step 1: Request Access to Source Code, Design Documents (10 days)**
  * Begin our deep dive into publicly available documentation and resources (website, githubs, case studies, install guides, etc)
* **Step 2: Initial Assessment Results (5 days)**
  * A narrative report on background information and history, which includes a Threat & Risk Assessment portion.&#x20;
  * _Share Evaluation & Report any issues to vendor_
* **Step 3: Source Code Security Audit (15 days)**
  * _Share Evaluation & Report any issues to vendor_
* **Step 4: Application Architecture Audit (10 days)**
  * _Share Evaluation & Report any issues to vendor_&#x20;
* **Step 5: Penetration Testing Audit (10 days)**
  * _Share Evaluation & Report any issues to vendor_&#x20;
    * Schedule a call to discuss severe issues if necessary&#x20;
* **Step 6: DevSecOps Analysis (15 days)**
  * _Share Evaluation & Report any issues to vendor_&#x20;
* **Step 7: Report of fFndings and Recommendations (10 days)**
  * _Share Evaluation & Report any issues to vendor_&#x20;
* **Step 8: Review Vendor Updates**
  * 8 weeks after sharing of initial report the Evaluator will review any fixed issues and remaining timeline of the vendor, and share a follow-on report of statuses and final assessment.

_Note: Some of these Steps may run in parallel depending upon availability of resources and status of dependencies._

_Note: If the vendor for some reason determines a fix isn’t necessary and Guardian Project feels it is a severe issue, they have a moral obligation to then take action. This action step will be shared with UNICEF and the vendor prior to action._&#x20;

### Requested Assets

In order to fully evaluate the CRVS solution, the Evaluation Team asks the CRVS Solution Vendor to provide the following assets in digital form:

**Product and architecture documents, diagrams, specifications**

* [ ] Documentation in HTML, DOCX, PDF, TXT, etc

**User stories, personas, threat models, needs assessments, and other user experience and feature design inputs**

* [ ] Documentation in HTML, DOCX, PDF, TXT, etc

**Source code for all tiers of the application**

* [ ] Ideally, shared through access to  source code management system (git repository, etc)
* [ ] Zip / Tarball also acceptable, but not ideal

**Access to ticketing systems, discussion boards, wikis, and other public development infrastructure**

* [ ] Web link, login credentials

**Inputs to and results from any other security audits**

* [ ] PDF files, contact information for auditor

**Prerequisites for installation, use, access**

* [ ] PDF files, Web-based guide, README, etc

**Operational deployment images, tools, and/or scripts for configuration management**

* [ ] Docker, Ansible, Terraform, install scripts, etc.
* [ ] Installation Guides (PDF Files, README txt)



#### Software Bill Of Materials

One area to discuss with closed-source vendors, is if they are able to product a Software Bill of Materials (SBOM). This can be a way they can share their technical building blocks, without having to expose their intellectual property. Also, while they mention penetration testing, we should learn more about their “secure by design” methods. This is where standards related to OWASP and SAST tools can play a role - if they adopt these themselves, and can produce the report outputs, then we may not need to direct analyze their source code.



#### Source Code Security Audit

A source code security audit is a crucial step in ensuring that a web and mobile application is secure and protected from potential vulnerabilities that can be exploited by attackers. The following is a specification of a source code security audit for a web and mobile application:

* Scope: The audit should cover all components of the application, including the server-side code, client-side code, and any third-party libraries or plugins used.
* Objective: The objective of the audit is to identify potential security vulnerabilities that could be exploited by attackers, such as injection attacks, cross-site scripting (XSS), authentication and authorization issues, and data leakage.
* Methodology: The audit should follow a methodology that includes both manual and automated testing, such as code review, static analysis, and penetration testing. The methodology should be comprehensive and cover all possible attack vectors.
* Tools: The auditor should use a variety of tools to perform the audit, including automated scanners, such as Burp Suite and OWASP ZAP, as well as manual testing tools like Postman, cURL, or browser extensions.
* Reporting: The auditor should provide a detailed report that outlines the findings and recommendations for fixing any identified security issues. The report should include a list of vulnerabilities, their severity, and recommendations for remediation.
* Compliance: The audit should ensure that the application complies with relevant security standards and best practices, such as OWASP Top 10, PCI-DSS, and HIPAA.
* Timeline: The audit should be completed within a reasonable timeframe, with a minimum of two weeks to allow for thorough testing and analysis of the source code.
* Follow-up: After the audit is completed, it is important to follow up with the development team to ensure that the recommended fixes have been implemented and that the application is now secure. It is also recommended to conduct periodic security audits to stay ahead of emerging threats and to maintain the security of the application over time.\
  \


#### Penetration and Dynamic Application Security Testing

Penetration Testing, also known as "pen testing," is a form of security testing that involves simulating a real-world attack on a system to identify vulnerabilities and potential exploits. The goal of penetration testing is to assess the security posture of a web and mobile application and to identify any weaknesses that could be exploited by an attacker. The penetration tester attempts to exploit vulnerabilities, typically using a combination of automated and manual techniques, to gain access to sensitive data or functionality within the application. The testing is typically conducted in a controlled environment, such as a test or staging environment, to prevent any unintended impact on the production system.

\


Dynamic Application Security Testing (DAST) is a type of security testing that focuses on the dynamic analysis of the application while it is running. DAST testing involves analyzing the behavior of the application during runtime to identify vulnerabilities that could be exploited by attackers. DAST tools typically simulate a user interacting with the application, sending various inputs to the system to see how it responds. DAST testing is particularly useful for identifying vulnerabilities related to input validation, authentication, and authorization.

\


During a penetration testing engagement, the tester attempts to identify and exploit vulnerabilities in the application, using a range of techniques including vulnerability scanning, manual testing, and social engineering. The penetration tester attempts to gain access to the system, escalate privileges, and access sensitive data or functionality within the application. The testing can be performed from various perspectives, such as an external attacker or an insider threat, to identify vulnerabilities from different angles.

\


On the other hand, DAST testing is focused on identifying vulnerabilities that can be discovered by analyzing the running application. DAST tools scan the application for vulnerabilities such as XSS, SQL injection, and CSRF attacks, and typically use a black-box approach where they have no knowledge of the application's internal workings. DAST tools can be used to identify a wide range of vulnerabilities, but they may miss some issues that can only be identified through manual testing or other specialized testing techniques.

\


In conclusion, penetration testing and DAST testing are both important types of security testing for web and mobile applications. Penetration testing simulates a real-world attack on the system to identify vulnerabilities and potential exploits, while DAST testing analyzes the behavior of the application during runtime to identify vulnerabilities that could be exploited by attackers. By combining both types of testing, an organization can identify and remediate vulnerabilities in their applications, improving the overall security posture of their systems.

\


