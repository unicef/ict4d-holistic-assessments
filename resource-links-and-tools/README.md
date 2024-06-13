---
description: The tools and service we used to complete the holistic audit process
cover: ../.gitbook/assets/UNI272563-Bahaji.jpg
coverY: 101
---

# Resource Links & Tools

### Generating Software Bill of Materials (SBOM)

We used the open-source tool [**syft**](https://github.com/anchore/syft) to create a Software Bill of Materials for entire code repositories and also for each Docker image produced from that repository. The advantage of the former is that we get an overview of all packages used in any core code or microservices. With the latter we can look at only the packages that appear in the final Docker image for a given microservice.&#x20;

_"Syft is a powerful and easy-to-use open-source tool for generating Software Bill of Materials (SBOMs) for container images and filesystems. It provides detailed visibility into the packages and dependencies in your software, helping you manage vulnerabilities, license compliance, and software supply chain security."_

The Github service also offers [software supply chain features for checking dependencies](https://github.com/features/security/software-supply-chain).

_"Keep your dependencies up-to-date and optimized and get updates on new vulnerabilities affecting your specific dependencies with Dependabot."_

• Product page:[ https://github.com/features/security/software-supply-chain](https://github.com/features/security/software-supply-chain)

• SBOM export docs: [https://docs.github.com/en/code-security/supply-chain-security/understanding-your-software-supply-chain/exporting-a-software-bill-of-materials-for-your-repository](https://docs.github.com/en/code-security/supply-chain-security/understanding-your-software-supply-chain/exporting-a-software-bill-of-materials-for-your-repository)

• Enabling Dependabot docs: [https://docs.github.com/en/code-security/dependabot/dependabot-security-updates/configuring-dependabot-security-updates](https://docs.github.com/en/code-security/dependabot/dependabot-security-updates/configuring-dependabot-security-updates)\


### **Open-Source Software (OSS) Vulnerability Scanning**

We used the open-source tool [**grype**](https://github.com/anchore/grype) to check the source and Docker images for vulnerabilities.&#x20;

_"A vulnerability scanner for container images and filesystems. Easily install the binary to try it out. Works with Syft, the powerful SBOM (software bill of materials) tool for container images and filesystems."_

Docker also offers their own [Docker Scout solution](https://www.docker.com/products/docker-scout/).\
\
_"Docker Scout generates signals across the software supply chain that inform improved development workflows. Developers are guided by contextual recommendations right where they work, leveraging data collected from a wide range of integrations."_

• Product page: [https://www.docker.com/products/docker-scout/](https://www.docker.com/products/docker-scout/)

• Docs: [https://docs.docker.com/scout/](https://docs.docker.com/scout/)



### **Static Application Security Testing (SAST) Scanning**

We used the open source SAST scanner [**semgrep**](https://semgrep.dev/) to perform an automated analysis of codebases.

_"Semgrep guides developers towards secure by default practices. Manage SAST, secrets, and supply chain security in a single platform that eliminates developer friction."_

### Dynamic Application Security Testing (DAST) Services

We utilized cloud-based testing suites and services, alongside human teams, that offer a variety of capabilities and options for one-time and ongoing scanning and testing. While fully bespoke and custom security audits are always a valuable service, they come at a very high cost in both money and time. Our approach for this evaluation was to use tools and techniques that are both within the realm of the available budget, and provided a more dynamic, ongoing approach for uncovering vulnerabilities. We recommend this approach for use not only in the evaluation stage, but also as part of the ongoing monitoring of production deployments.

#### [Intruder.io](https://www.intruder.io/): fast, cheap automated vulnerability scanning service, with multiple vantage points; Less feature rich, but still a good tool for initial “smoke test” results.

_"Emergent Threats performs automated, nearly daily additional ongoing, focused scans based on newly identify threats and vulnerabilities added to the Astra database. Nessus Agents extend scanning to run within server-infrastructure from the “inside out” uncovering vulnerabilities and configuration issues that an attacker may take advantage of if they compromise a network."_\


#### [Astra](https://www.getastra.com/): Powerful tool+service providing Automated, Vetted, and Emergent Threats vulnerability scanning

_"Automated is machine-only scripted testing of a comprehensive set of known vulnerabilities; Vetted builds on the Automated result, then adds human review and verification of identified potential vulnerabilities to add more detail, and identity and label “false positives”._\


\
