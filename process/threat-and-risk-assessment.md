---
description: Threats and Risk exist; What matters is how you are prepared to respond!
---

# Threat Modeling and Mitigations

<i>Most relevant for 🔥 [Advisors](../get-started.md#advisors) and 🔍 [Technical Evaluators](../get-started.md#technical-evaluators)</i>

As discussed in the [introduction to this section](holistic-audits-for-ict4d.md), threat modeling is a process of identifying, analyzing, and prioritizing the potential security threats and vulnerabilities in a software system. In response to those threats, risk mitigation offers a process of designing, implementing, and otherwise taking steps to reduce or eliminate identified risks (threats and vulnerabilities!) in a software development project or technology solution.

#### A Wide Variety of Approaches

While we took a specific approach to this work in our technical assessments, there is a long history of diverse approaches to understanding threat and risk. Here are a few outside links to broader, useful resources on the web.&#x20;

* ["Threat Modeling for Measurement and Analytics"](https://docs.cleaninsights.org/docs/threat-modeling/) - a [15 minute video](https://www.youtube.com/watch?v=nt6ac3WoogA) and [presentation](https://docs.google.com/presentation/d/1RsikxjM9SxLkEK68WT4sgywA68LeL2m3o9T37LcjRCY/edit?usp=sharing)
* ["Microsoft Threat Modeling Tool Threats"](https://learn.microsoft.com/en-us/azure/security/develop/threat-modeling-tool-threats)
* [OWASP Community - Threat Modeling](https://owasp.org/www-community/Threat\_Modeling)

#### Sample Threat Model

Below is an example of a threat modeling process performed on a [recently reviewed solution](../partners/partner-assessments/). The Threat, Likelihood, Impact, and Severity columns listed below are in reference to the world, and specific places where solutions are implemented, and not specific to the vendor, platform, or solution itself. This gives the reader an idea of what kind of mitigations could be put in place for a solution.

Likelihoods range from <mark class="blue">Unlikely</mark> to <mark style="color:red;">Likely</mark>, while Severity can be <mark class="blue">Minor</mark> to <mark style="color:red;">Critical</mark>.\

<style>
table, th, td {
  border: 1px solid;
}</style>
<table><thead><tr><th width="167">Threat</th><th width="119">Likelihood</th><th width="181">Impact</th><th width="108">Severity</th><th>Mitigations</th></tr></thead><tbody><tr><td><em>Describe the potential threat, attack vector, bad actor</em></td><td><em>How likely is it that this could happen?</em> </td><td><em>What will happen if the threat/attack is successful?</em></td><td><em>How severe will the impact be?</em></td><td>How does the solution reduce the risk, impact, and severity of the attack?</td></tr><tr><td>Identity theft or fraud</td><td><mark style="color:red;">Likely</mark></td><td>Personal data, including that of children, is increasingly in demand by identity thieves</td><td><mark style="color:purple;">Moderate</mark></td><td>(1) Encryption and decryption of fields stored in the database (2) Support for OpenID Connect(OIDC) Identity Layer with access controls and flexible deployment of authentication systems</td></tr><tr><td>Privacy Violation</td><td><mark style="color:orange;">Moderately likely</mark></td><td>Digital transmission, networked storage and increased sharing of birth data may expose personal information to individuals and uses that are against the wishes of families participating in registration</td><td><mark style="color:purple;">Minor</mark></td><td><p>(1) Encryption of data on the network and at rest<br>(2) Multiple Access Control roles that limit the scope of access to data and capabilities.</p><p>(3) Data retention policies and features</p><p>(4) Training, education, and guidance provided by community</p></td></tr><tr><td>Targeting based on personal characteristics</td><td><mark style="color:purple;">Very unlikely</mark></td><td>The ability to rapidly gather and process large amounts of population data could contribute to targeted advertising, other forms of exploitation, and targeted physical threats and violence.</td><td><mark style="color:orange;">Severe</mark></td><td><p>(1) Multiple roles that limit the scope of access to data and capabilities</p><p>(2)  Limit in user experience for mass search and export</p></td></tr><tr><td>Personal security violation or exploitation</td><td><mark style="color:orange;">Moderately likely</mark></td><td>Registration happening outside a controlled institutional environment, such as a hospital or registrar’s office, could place families at risk of physical violence and economic or other exploitation by registration agents.</td><td><mark style="color:orange;">Severe</mark></td><td><p>(1) Easy access to mobile interface, even with limited connectivity, keeps as much data reporting “in the system” and private as possible</p><p>(2) Focus on defined user roles, control who has access to accounts can help fight corruption and exploitation</p></td></tr><tr><td>Incorrect or Insecure Deployment*</td><td><mark style="color:orange;">Moderately likely</mark></td><td>Deployment of services by unqualified staff or into unvetted or untested environments could lead to data exfiltration, watering hole attacks, and other harms to the users and administrators</td><td><mark style="color:red;">Critical</mark></td><td><p>(1) Availability of deployment docs, training, and support</p><p>(2) “Platform” approach creates potential for an ecosystem of certified/trusted partners for deployment<br>(3) Transparency of open-source and iterative development means vulnerabilities and updates can be fixed and deployed quickly</p><p><br></p></td></tr></tbody></table>



\
