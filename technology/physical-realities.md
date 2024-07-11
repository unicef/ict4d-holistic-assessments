---
description: How and where your infrastructure and devices are hosted and operated matters
---

# Physical Realities

While many technology startups and services can fully embrace the opaque virtualization of modern cloud service infrastructure, when it comes to personal, private, and health data, and other ICT4D applications, you need to be more careful. Fully considering how and where your infrastructure is hosted, and where physical devices like laptops, tablets, and smartphones will be used is an absolute requirement when launching new technology.



<img src="../.gitbook/assets/file.excalidraw (1).svg" alt="a spectrum of physicality" class="gitbook-drawing">

### Self-Hosted

* **In-Office or "Back Office"**
  * In some cases, deploying and managing server infrastructure in a physically secure office setting is the only option. If done right, it can also be a very good option. The most critical piece in this setting is physical security of the hardware, followed by ensuring reliably power and internet.&#x20;
  * _<mark style="background-color:yellow;">The</mark>_ [_<mark style="background-color:yellow;">Assessment 1: The Turn-Key Solution</mark>_](../partners/partner-assessments/the-turn-key-solution.md) _<mark style="background-color:yellow;">and</mark>_ [_<mark style="background-color:yellow;">Assessment 3: The Custom Software Development Kit</mark>_](../partners/partner-assessments/the-custom-software-development-kit.md) _<mark style="background-color:yellow;">are examples of solutions that could be run in this kind of setting.</mark>_
* **Data Center**
  * If you have the skills and resources to build and run your own data center, then it can be a cost-effective and very secure solution. On top of the considerations from hosting in an office, the physical security of the entire data center room, along with cooling, power, and other physical demands must be considered.
  * _<mark style="background-color:yellow;">The</mark>_ [_<mark style="background-color:yellow;">Assessment 2: The Open Platform</mark>_](../partners/partner-assessments/the-open-platform.md) _<mark style="background-color:yellow;">is an example of a solution that could be run in this kind of setting.</mark>_

### Cloud-Hosted

* **Dedicated Servers**
  * By moving your hosting to a third-party cloud data center, but still using your own physically dedicated servers, you can alleviate some of the risk and load from your team, while still having a large amount of control of your infrastructure. This includes ensuring your server is using full-disk encryption for example.
* **Virtual Private Servers**
  * The cheaper approach to cloud hosting is to have multiple virtual servers share one physical server box. This a cost-affordable solution, but also the least private and secure. Any use of a VPN should require data encryption-at-rest within the database and disk volumes.
* **Elastic or On-Demand Infrastructure**
  * Beyond the basic dichotomy of Dedicated vs Virtual, there is a third category of hosting which could be called "Elastic". This is an approach that allows an image of a service to be created and deployed through automated tools, and for the scale of availability of that infrastructure to be dynamically scaled up and down based on demand and need.

### Software as a Service (SaaS)

Letting someone else manage your application in their own data center or cloud infrastructure is definitely the simplest and fastest path to launching. However, you are not only trusting "someone else's computer", but you are trusting "someone else" with all of your data, reliability, and relationships to the beneficiary. You may also not be able to fully control where your data exists geographically, or ensure it is only stored in legal jurisdictions compatible with your application and beneficiaries expectations.

<mark style="background-color:yellow;">The</mark> [<mark style="background-color:yellow;">Assessment 4: The Cloud SaaS</mark>](../partners/partner-assessments/the-cloud-software-as-a-service.md) <mark style="background-color:yellow;">is an example of a solution that is offered in this way.</mark>

