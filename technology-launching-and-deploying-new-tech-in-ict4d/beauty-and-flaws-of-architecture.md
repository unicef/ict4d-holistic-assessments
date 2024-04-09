# Beauty and Flaws of Architecture

**Recommendations:**

* **Avoid the need for extensive customization.**
  * DHIS2 requires significant customization to fit UNICEF's CRVS needs, introducing potential risks and complexities.
  * Prioritize solutions that align with your specific requirements to minimize the need for extensive modifications.
* **Ensure adequate expertise and resources for complex systems.**
  * OpenCRVS's complexity demands specialized expertise for effective management and maintenance.
  * Allocate the necessary resources and expertise to support the implementation and ongoing operation of such systems.
* **Consider the total cost of ownership.**
  * OpenCRVS does not have licensing fees, but it may incur additional costs associated with third-party dependencies and specialized expertise.
  * Conduct a thorough analysis to understand the complete financial implications before implementing the system.
* **Conduct regular security audits.**
  * DHIS2's security audits are limited to individual implementers' reports.
  * Establish a proactive approach to security by conducting regular audits and promptly addressing any identified vulnerabilities.
* **Invest in comprehensive documentation.**
  * DHIS2's system administrator documentation lacks information on disaster recovery procedures.
  * Prioritize the development of comprehensive documentation covering all aspects of the system, including security practices, deployment guidelines, and disaster recovery plans.
* **Adopt continuous integration and deployment practices.**
  * DGIT lacks a continuous integration/continuous deployment system for managing the software lifecycle.
  * Implement CI/CD to streamline the development and deployment processes and facilitate rapid updates and bug fixes.
* **Publish source code dependencies publicly.**
  * DGIT's source code dependencies are not publicly available, hindering maintenance and updates.
  * Share the dependencies publicly to ensure transparency and ease of access for maintenance purposes.
* **Integrate manual and automated testing.**
  * DGIT lacks both manual test plans and automated testing, increasing the risk of undetected defects.
  * Implement a comprehensive testing strategy combining manual and automated testing to ensure the system's quality and reliability.
* **Address security concerns promptly.**
  * DGIT's audit uncovered several security risks.
  * Prioritize addressing these risks promptly to enhance the system's security posture and protect sensitive data.

By implementing these recommendations, organizations can benefit from the strengths and avoid the pitfalls identified in the architecture audits of DHIS2, OpenCRVS, and DGIT, leading to more secure, reliable, and sustainable systems.
