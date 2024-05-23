---
description: Four examples of partner solutions that were evaluated, and what we learned
---

# Evaluations Outcomes

{% embed url="https://youtu.be/pDPiwviyt4k" %}

Evaluations were conducted on four software projects that provide solutions in the realm of ICT4D. These projects were evaluated to assess their fitness for purpose, readiness for enhancement, maintainability, performance, and security.

Our team has extensive experience working with, testing, building on, and deploying open-source projects and platforms. Behind these efforts are diverse teams with varying scales, experiences, qualities, reliability, visions, and commitments. Achieving a usable, dependable solution requires balancing creativity and experience, innovation, and reliability. Some developers can quickly demonstrate the feasibility of an idea but lack the follow-through to implement all necessary features. Conversely, others may be meticulous but inflexible in updating and improving their work. Additionally, building a solution involves decisions on whether to write everything from scratch or rely on and support a rich ecosystem of open-source modules, libraries, and services. There is no definitive answer, only a path forward shaped by specific requirements and expectations.

## <mark style="color:purple;">Evaluation 1: "The Turn-Key Solution"</mark>

We found the first solution we evaluted to be stable and ready for implementation. It has excellent documentation for implementers, is interoperable with many e-government solutions, and focuses on real-world workflows with a supportive team. The reliance on third-party dependencies is commonplace, and the choice of microservices makes for a flexible and extensible solution. While there are areas for improvement outlined in the document, they do not detract from the overall positive evaluation. As a relatively new entrant to the market, the product may not be as flexible or feature-rich as other solutions but benefits from a focused functionality, modern architecture, and well-run public open-source project. The concept of a single unified upstream codebase that can be improved and updated, then pushed out to downstream instances, is particularly attractive and beneficial for global deployment and maintenance.

During the first evaluation, we encountered vulnerabilities within the source code, the version of nodeJS it is built upon, and the security of deployment configurations. These issues were expected at this stage of the project.&#x20;

### **We were pleasantly surprised by how engaged and positive the team was in reviewing and addressing these issues**.&#x20;

Fixes were implemented, nodeJS was updated, and deployment configurations were improved, indicating a healthy project ready to face real-world challenges. Despite these positive developments, we have concerns about improving the documentation to enable self-service deployment. To scale up effectively, it is essential to ensure the solution can be deployed in a repeatable, reliable, private, and secure manner by qualified individuals. The commitment to open, quality documentation is evident, but some confusing aspects need to be clarified, additional pieces provided, and improved scripts and deployment tools developed.

## <mark style="color:purple;">Evaluation 2: "The Open Platform"</mark>

We found the second evaluated solution to be stable and ready for implementation. It is a free, open-source software platform designed for reporting, collecting, analyzing, and disseminating individual-level and aggregated data. Although not specifically designed for CRVS, it can integrate with CRVS systems or be extended to include CRVS-related features. Implementing interoperability can be costly in terms of both initial integration and long-term operation and maintenance. We also evaluated the additional costs associated with combining this software with a CRVS system.

The software, provided as a global public good to support sustainable development goals, includes a suite of visualization and analysis tools, making it effective for linking data for reporting and tracking purposes. It can be hosted locally on various devices or in the cloud and is most commonly used for health data. It integrates with various other software and tools through its Application Programming Interface (API) and is deployed in 75 low- and middle-income countries, with over 100 NGOs having implemented it.&#x20;

### **The solution fits many contexts and use cases, such as logistics, education, COVID-19 vaccine tracking, agriculture projects, e-governance, food and nutrition, and more**.&#x20;

The evaluation involved reviewing publicly available documentation, attending virtual meetings, leveraging resources on YouTube and their community resources page, and testing a local cluster using the command line tool. We deployed an instance to test vulnerabilities and dependencies, created a Software Bill of Materials (SBOM) for the codebase, audited the architecture deployed in AWS, and conducted various vulnerability scans and penetration tests. Despite some scheduling difficulties, the team has been responsive and engaged, providing feedback and clarity.

## <mark style="color:purple;">Evaluation 3: "The Custom Software Development Kit"</mark>

This evaluation provided a detailed analysis of a legal identity system and software development kit designed to enhance civil registration services. The solution was adaptable to various government systems such as voter registration and passports, has been successfully implemented in countries like Malawi and Honduras, facilitating millions of ID card distributions and supporting government services. Despite its versatility and potential, the system required significant technical expertise for successful deployment and maintenance, addressing complex workflows and ensuring interoperability with other registries.

The evaluation highlighted the system's microservices architecture, along with client applications for Windows and Android. However, concerns were raised about the limited human capacity for post-deployment maintenance, the lack of integration into an ongoing software lifecycle, and several security vulnerabilities.&#x20;

### Issues identified included hard-coded credentials, inadequate testing, and insufficient defenses against supply chain attacks.&#x20;

Recommendations for improvement include developing manual and automated test plans, removing hard-coded credentials, and enhancing database access safety. The report also noted challenges in accessing publicly available code and documentation, emphasizing the need for direct partnership with the project team for a secure and successful implementation

## <mark style="color:purple;">Evalulation 4: "The Cloud Software-as-a-Service"</mark>

_coming soon..._
