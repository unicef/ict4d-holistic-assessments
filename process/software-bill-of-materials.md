# Software Bill of Materials

One area to discuss with vendors, especially if they are not open-source, is if they are able to product a Software Bill of Materials (SBOM). This can be a way they can share their technical building blocks, without having to expose their intellectual property.&#x20;

Processes and Tools

We used the open-source tool ‘syft’ to create a Software Bill of Materials for the entire opencrvs-core repository and also for each Docker image produced from that repository. The advantage of the former is that we get an overview of all NPM packages used in any of the microservices. With the latter we can look at only the packages that appear in the final Docker image for a given microservice. \
\
