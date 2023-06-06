# Chapter: The Shared Responsibility Model in Cloud

In the world of cloud computing, a key concept is the shared responsibility model. Depending on the chosen service model, different aspects of system management and security are shared between the cloud service provider (CSP) and the customer.

## 1. Infrastructure as a Service (IaaS)

An example of an IaaS service is Amazon Web Services (AWS) - Elastic Compute Cloud (EC2). When you use EC2, Amazon provides you with the basic infrastructure - servers, storage, network - and is responsible for its maintenance and security. As a developer, you have the ability to deploy your software on these servers, but you are responsible for its security and proper operation.

In this model, AWS is responsible for "security of the cloud" - the physical infrastructure, servers, the software that serves them, the network, etc. On the other hand, the customer is responsible for "security in the cloud" - the software that runs on these servers, the data it stores, how these data are secured, etc.

## 2. Software as a Service (SaaS)

Examples of SaaS services are Gmail from Google or Office 365 from Microsoft. In the SaaS model, the cloud service provider is responsible not only for the infrastructure, but also for the software and its operation. This means that the provider must ensure not only "security of the cloud", but also "security in the cloud".

As a user of a SaaS service, you are mainly responsible for security at the user level. This includes aspects such as identity and access management, securing user data, password management, using two-factor security, etc.

## 3. Comparison of IaaS and SaaS

From a security perspective, the key difference between IaaS and SaaS is where the responsibility of the cloud service provider ends and the responsibility of the customer begins.

For IaaS, like AWS EC2, the provider's responsibility ends with the infrastructure. The customer must ensure the security of their software and data themselves.

For SaaS, like Gmail or Office 365, the cloud service provider is responsible for everything - both the infrastructure and the software. As a user, you only need to ensure security at the user level.

This comparison shows why the SaaS model places the most responsibility on the cloud service provider. They not only have to provide a secure and reliable infrastructure, but they also have to ensure that the software they provide as a service is secure and operates correctly.