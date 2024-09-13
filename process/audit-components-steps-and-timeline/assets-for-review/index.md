---
description: What you need to have in order to know!
---

# Assets for Review

In order to fully assess a solution, you need the right set of inputs. The following is a list and description of the recommended assets to requests from any solution provider.

### **Product and architecture documents, diagrams, specifications**

These materials should outline the overall structure and design of the software, showing the interrelationships between various components and layers within the architecture. Diagrams should include both high-level overviews and detailed breakdowns of specific subsystems. Specifications should cover both functional and non-functional requirements of the software, providing clear insight into its intended behavior, performance metrics, security features, and integration capabilities. This documentation will enable us to assess the software’s design robustness, maintainability, and compliance with best practices and relevant standards.

### **User stories, personas, threat models, needs assessments, and other user experience and feature design inputs**

To gain a comprehensive understanding of the user experience and feature design of your software solution, an audit requires all relevant materials that detail [user stories](https://www.atlassian.com/agile/project-management/user-stories), [personas](https://www.interaction-design.org/literature/topics/personas), [threat models](../../threat-and-risk-assessment.md), needs assessments, and other user experience inputs. [User stories](https://www.atlassian.com/agile/project-management/user-stories) should describe the functionality of the software from an end-user perspective, illustrating typical tasks and user objectives.

<figure><img src="../../../.gitbook/assets/userstoryexample.png" alt="" width="100%"><figcaption><p>A <a href="https://www.parabol.co/blog/user-story-examples/">user story example</a> from Parabol.co</p></figcaption></figure>

[Personas](https://www.interaction-design.org/literature/topics/personas) should provide detailed profiles of user types, including their goals and challenges, and usage which inform the design and functionality of your product.

<figure><img src="../../../.gitbook/assets/td-service safaris-persona.webp" alt="" width="100%"><figcaption><p><a href="https://www.interaction-design.org/literature/topics/personas">Persona example</a> from the Interaction Design Foundation</p></figcaption></figure>

[Threat models](../../threat-and-risk-assessment.md) that outline potential security vulnerabilities from a user perspective, including how these threats are mitigated, are also useful. Needs assessments should detail the research conducted to identify what users require from the software, including how these needs have driven the design decisions made.&#x20;

### **Source code for all tiers of the application**

Access to all the source code for all tiers of the application, including but not limited to the front-end, back-end, and any middleware or services that interact between these layers, is necessary for a true holistic audit. The solution provider should offer complete, up-to-date source code repositories for each component of the application, preferably with version control histories, if available. This should also include any build scripts, dependencies, and third-party libraries used within the application, along with documentation that describes the build process, environment configuration, and deployment procedures.&#x20;

### **Access to ticketing systems, discussion boards, wikis, and other public development infrastructure**

For a comprehensive understanding of the development process and ongoing maintenance of your software solution, the assessment team should have access to all related development infrastructure. This includes ticketing systems, discussion boards, wikis, and any other platforms used for public development communication and documentation.&#x20;

<figure><img src="../../../.gitbook/assets/dhis2community.png" alt="" width="100%"><figcaption><p>DHIS2 has a <a href="https://community.dhis2.org/">robust community forum</a></p></figcaption></figure>

Access to these resources will allow for review of how features and bugs are tracked, prioritized, and resolved, providing insights into a team’s workflow and responsiveness to issues. Additionally, it is important to examine the collaborative aspects of the development process by looking into how information is shared and decisions are made, as documented in discussion boards and wikis. This review helps to assess the effectiveness of a development practices, the alignment of ongoing work with user needs and security practices, and the overall health and sustainability of the project's development environment.

### **Inputs to and results from any other security audits**

To ensure a comprehensive evaluation of a software solution's security posture, detailed documentation pertaining to any previous security audits conducted should be requested. This includes both the inputs provided for these audits, such as scopes, specifications, configurations, and any specific areas of concern, as well as the results or findings from the audits, including detailed reports, vulnerability assessments, risk analysis, and recommendations made.

<figure><img src="../../../.gitbook/assets/opencrvssecurity.png" alt="" width="100%"><figcaption><p><a href="https://documentation.opencrvs.org/technology/security">OpenCRVS</a> offers robust and transparent <a href="https://documentation.opencrvs.org/technology/security">public security information</a></p></figcaption></figure>

Additionally, any follow-up actions taken or remediations implemented as a result of these audits should also be included. Access to this historical audit information will allow the audit team to gauge the evolution of the software's security measures over time, understand recurring issues or vulnerabilities, and evaluate the effectiveness of previous remediation efforts. This will be instrumental in identifying potential areas of vulnerability, assessing risk levels, and recommending further improvements to enhance the software’s security and compliance with industry standards.

### **Prerequisites for installation, deployment, use, access**

To ensure the assessment team has a smooth installation, deployment, and usage of the software solution, request detailed documentation outlining all prerequisites and necessary conditions. This documentation should include specific hardware and software requirements, such as operating systems, database systems, third-party libraries, and any necessary software dependencies. Additionally, any guides detailing the installation process, including step-by-step instructions and any scripts or automation tools used, should be provided.

<figure><img src="../../../.gitbook/assets/opencrsvinstall.png" alt="" width="100%"><figcaption><p>OpenCRVS provides <a href="https://documentation.opencrvs.org/setup/3.-installation/3.1-set-up-a-development-environment/3.1.1-install-the-required-dependencies">detailed information on dependencies and installation</a>.</p></figcaption></figure>

For deployment, request to have provided configurations, environmental setup details, and best practices to ensure representational and optimal performance and security. Information on access requirements, such as necessary credentials, user role configurations, and security protocols for gaining entry to different parts of the system, should also be included. This information will enable the audit team to replicate a solution's deployment environment accurately, ensuring that the holistic technical assessment reflects the real-world operation and integration of the solution.

### **Operational deployment images, tools, and/or scripts for configuration management**

For a thorough examination of the operational aspects of your software solution, request detailed documentation and actual deployment artifacts including operational deployment images, tools, and scripts used for configuration management. This includes any container images, virtual machine snapshots, or other deployable artifacts that represent the production or staging environments of the solution. Additionally, request access to the tools and scripts used for managing configurations, deploying updates, and maintaining the infrastructure. This should include automation scripts for provisioning, deployment scripts, configuration templates, and any relevant documentation that describes how these tools and scripts are used in the daily operations of the application.

This information will enable the assessment team to understand the deployment processes, configuration management practices, and operational workflows used to maintain the application. It will also allow them to assess the efficiency, reliability, and security of the deployment and configuration management strategies employed. By replicating the operational environment, the assessment can more accurately identify potential operational vulnerabilities, ensure compliance with industry standards, and suggest improvements to enhance system stability and security.

{% file src="../../../.gitbook/assets/Requested Assets.pdf" %}
List of assets requested from each vendor
{% endfile %}
