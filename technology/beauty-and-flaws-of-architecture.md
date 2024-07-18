---
description: Project and engineering management best practices to review and consider
---

# Management Strategies

By implementing the following recommendations, technical planning and engineering management processes can benefit from the strengths and avoid the pitfalls identified in the architecture audits we completed. This approach leads to more secure, reliable, and sustainable systems.

## <mark style="background-color:yellow;">**Avoid the need for extensive customization**</mark>

Some solutions require significant customization to fit defined needs, introducing potential risks and complexities. Prioritize solutions that align with your specific requirements to minimize the need for extensive modifications.

In some cases, fully custom solutions are needed, and in that case, solutions such as [Assessment 2: The Open Platform](../partners/partner-assessments/the-open-platform.md) or [Assessment 3: The Custom Software Development Kit](../partners/partner-assessments/the-custom-software-development-kit.md), may be required.

<figure><img src="../.gitbook/assets/1.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Ensure adequate expertise and resources for complex systems**</mark>

Some solutions complexity demands specialized expertise for effective management and maintenance. Allocate the necessary resources and expertise to support the implementation and ongoing operation of such systems.

<figure><img src="../.gitbook/assets/2.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Consider the total cost of ownership**</mark>

Some solutions do not have licensing fees, but may incur additional costs associated with third-party dependencies and specialized expertise. Conduct a thorough analysis to understand the complete financial implications before implementing the system.

[Assessment 1: The Turn-Key Solution](../partners/partner-assessments/the-turn-key-solution.md) and [Assessment 2: The Open Platform](../partners/partner-assessments/the-open-platform.md) are two examples of no cost, or "free and open-source" solutions, that still will require investment in a team and infrastructure to tune, deploy, and manage it.

<figure><img src="../.gitbook/assets/3.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Conduct regular security audits**</mark>

Establish a proactive approach to security by conducting regular audits and promptly addressing any identified vulnerabilities. A comprehensive security audit should include aspcets of [source code security](../process/audit-components-steps-and-timeline/source-code-security.md), [vulnerability scanning](../process/audit-components-steps-and-timeline/vulnerability-scanning.md), and [penetration testing](../process/audit-components-steps-and-timeline/penetration-testing/).

<figure><img src="../.gitbook/assets/4.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Invest in comprehensive documentation**</mark>

One solution's system administrator documentation lacked information on disaster recovery procedures. Prioritize the development of comprehensive documentation covering all aspects of the system, including security practices, deployment guidelines, and disaster recovery plans. You can review our [DevSecOps Checklist](../process/development-and-secure-operations/) for a guide on steps to consider when preparing to launch.

<figure><img src="../.gitbook/assets/5.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Adopt continuous integration and deployment practices**</mark>

Some solutions lack a continuous integration/continuous deployment system for managing the software lifecycle, from testing to production. Implement CI/CD to streamline the development and deployment processes and [facilitate rapid updates and bug fixes](../partners/understanding-identity-and-privacy.md).

<figure><img src="../.gitbook/assets/6.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Publish source code dependencies publicly**</mark>

Some solutions source code dependencies are not publicly available, hindering maintenance and updates. Share all dependencies publicly through a [Software Bill of Materials](../process/software-bill-of-materials.md) to ensure transparency and ease of access for maintenance purposes.

<figure><img src="../.gitbook/assets/7.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Integrate manual and automated testing**</mark>

One solution lacked both manual test plans and automated testing, increasing the risk of undetected defects. Implement a comprehensive testing strategy combining manual and automated testing to ensure the system's quality and reliability. Consider using the [tools and services](../resource-links-and-tools/) we use in the holistic assessment process.

<figure><img src="../.gitbook/assets/8.png" alt=""><figcaption></figcaption></figure>



## <mark style="background-color:yellow;">**Address security concerns promptly**</mark>

Some assessments uncovered several security risks. Prioritize addressing these risks promptly to enhance the system's security posture and protect sensitive data.

<figure><img src="../.gitbook/assets/9.png" alt=""><figcaption></figcaption></figure>



