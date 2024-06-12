---
description: Project and engineering management best practices to review and consider
---

# Management Strategies

By implementing the following recommendations, technical planning and engineering management processes can benefit from the strengths and avoid the pitfalls identified in the architecture audits we completed. This approach leads to more secure, reliable, and sustainable systems.

## <mark style="background-color:yellow;">**Avoid the need for extensive customization**</mark>

Some solution requires significant customization to fit defined needs, introducing potential risks and complexities. Prioritize solutions that align with your specific requirements to minimize the need for extensive modifications.

In some case, fully custom solutions are needed, and in that case, solutions such as [Audit 2: The Open Platform](../partners/partner-audits/audit-2-the-open-platform.md) or [Audit 3: The Custom Software Development Kit](../partners/partner-audits/audit-3-the-custom-software-development-kit.md), may be required.

<figure><img src="https://images.unsplash.com/photo-1502217625004-89c03571bcca?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHx0YWlsb3J8ZW58MHx8fHwxNzE1MjIyMjMzfDA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Ensure adequate expertise and resources for complex systems**</mark>

Some solutions complexity demands specialized expertise for effective management and maintenance. Allocate the necessary resources and expertise to support the implementation and ongoing operation of such systems.

<figure><img src="https://images.unsplash.com/photo-1507679799987-c73779587ccf?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHxleHBlcnR8ZW58MHx8fHwxNzE1MjIyMjc2fDA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Consider the total cost of ownership**</mark>

Some solution do not have licensing fees, but may incur additional costs associated with third-party dependencies and specialized expertise. Conduct a thorough analysis to understand the complete financial implications before implementing the system.

[Audit 1: The Turn-Key Solution](../partners/partner-audits/audit-1-the-turn-key-solution.md) and [Audit 2: The Open Platform](../partners/partner-audits/audit-2-the-open-platform.md) are two examples of no cost, or "free and open-source" solutions, that still will require investment in a team and infrastructure to tune, deploy, and manage it.

<figure><img src="https://images.unsplash.com/photo-1561414927-6d86591d0c4f?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwzfHxtb25leXxlbnwwfHx8fDE3MTUyMjIzMDF8MA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Conduct regular security audits**</mark>

Establish a proactive approach to security by conducting regular audits and promptly addressing any identified vulnerabilities. A comprehensive security audit should include aspcets of [source code security](../process/audit-components-steps-and-timeline/source-code-security.md), [vulnerability scanning](../process/audit-components-steps-and-timeline/vulnerability-scanning.md), and [penetration testing](../process/audit-components-steps-and-timeline/penetration-testing.md).

<figure><img src="https://images.unsplash.com/photo-1550751827-4bd374c3f58b?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHxzZWN1cml0eXxlbnwwfHx8fDE3MTUyMjIzODV8MA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Invest in comprehensive documentation**</mark>

One solution's system administrator documentation lacked information on disaster recovery procedures. Prioritize the development of comprehensive documentation covering all aspects of the system, including security practices, deployment guidelines, and disaster recovery plans.

You can review our [DevSecOps Checklist](development-and-secure-operations.md) for a guide on steps to consider when preparing to launch.

<figure><img src="https://images.unsplash.com/photo-1509475826633-fed577a2c71b?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxkb2N1bWVudGF0aW9ufGVufDB8fHx8MTcxNTIyMjQyMHww&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Adopt continuous integration and deployment practices**</mark>

Some solutions lack a continuous integration/continuous deployment system for managing the software lifecycle, from testing to production. Implement CI/CD to streamline the development and deployment processes and [facilitate rapid updates and bug fixes](../partners/understanding-identity-and-privacy.md).

<figure><img src="https://images.unsplash.com/photo-1612263731558-bbac49f8581a?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHxnZWFyfGVufDB8fHx8MTcxNTIyMjQ0NHww&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Publish source code dependencies publicly**</mark>

Some solutions source code dependencies are not publicly available, hindering maintenance and updates. Share all dependencies publicly through a [Software Bill of Materials](../process/software-bill-of-materials.md) to ensure transparency and ease of access for maintenance purposes.

<figure><img src="https://images.unsplash.com/photo-1541692641319-981cc79ee10a?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxibG9ja3N8ZW58MHx8fHwxNzE1MjIyNDgxfDA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Integrate manual and automated testing**</mark>

One solution lacked both manual test plans and automated testing, increasing the risk of undetected defects. Implement a comprehensive testing strategy combining manual and automated testing to ensure the system's quality and reliability.

Consider using the [tools and services](../resource-links-and-tools.md) we use in the holistic audit process.

<figure><img src="https://images.unsplash.com/photo-1507146153580-69a1fe6d8aa1?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw1fHxyb2JvdHxlbnwwfHx8fDE3MTUyMjI1MjJ8MA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

## <mark style="background-color:yellow;">**Address security concerns promptly**</mark>

Some audits uncovered several security risks. Prioritize addressing these risks promptly to enhance the system's security posture and protect sensitive data.

<figure><img src="https://images.unsplash.com/photo-1509099652299-30938b0aeb63?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxzcGVlZHxlbnwwfHx8fDE3MTUyMjI1NjJ8MA&#x26;ixlib=rb-4.0.3&#x26;q=85" alt=""><figcaption></figcaption></figure>

