---
layout: post
title: 'Six capabilities modern ISVs need in order to future-proof their SaaS offering'
tags: [SaaS, ISV, Cloud Strategy]
featured_image_thumbnail:
featured_image: 
featured: false
hidden: false
---

Successful software vendors (ISVs) are leveraging public cloud capabilities and becoming SaaS providers. The move to public cloud-based SaaS offering provides ISVs a potential for business growth that cannot be matched with traditional on-premise single-tenant solution. In fact, Gartner estimates that the market size of the SaaS marketplace this year will be $99.7B while growing at the rate of 21% [1].

*(This blog post was originally published on [Nordcloud company Blog](https://www2.nordcloud.com/isvsblog))*

<!--more-->

## ISVs can benefit from moving to SaaS in several different ways 
It helps them to:
1. Unlock new customer segments through lower customer acquisition cost and easier geographical expansion
2. Reduce the total cost of ownership (TCO) through elimination of customer-specific support costs
3. Reduced time-to-market through leveraging built-in components available in all the public cloud platforms
4. Leverage data and insights through a unified data platform 

Moving from a traditional license-based business model to a subscription model also lowers customers’ barrier to buy while improving financial predictability for the ISV. In contrast to the traditional licensing model, subscription models allow customers to use the software without committing to long licensing periods – lowering their barrier to buy. It also smoothens the revenue curve through monthly recurring revenue, resulting in improved financial predictability.

## Successful SaaS providers have built their business around 6 core capabilities
Having worked with many SaaS providers on their cloud migration journey, we have identified a set of capabilities that separates the successful companies from the rest. These capabilities are:

![Six Capabilities](assets/images/posts/2020/six_capabilities.png)

The key for building these six capabilities effectively is to use the capabilities provided by public cloud platforms like AWS, Azure and GCP. I’ll go through each one of these capabilities in some detail below.

## Multi-tenancy
Successful SaaS vendors provide standardised service to all customers through multi-tenancy. This means that they provide a single shared application and data layer to all customers, without customer specific instances.

![Multi-tenancy](assets/images/posts/2020/multitenancy.png)

In contrast, the traditional single tenancy model results in high costs due to maintenance overhead of keeping application instances in sync across the installation base. Your different instances will also easily drift apart from each other in terms code and configuration. 

Some organisations opt for limited multi-tenancy where all the customers share a common application layer, but the data layer is kept in separate customer-specific instances. This can be a useful model for organisations whose customers are following strict data compliancy regulations and must keep their data in a specific geographical region, for instance.

The full multi-tenancy model provides the most value by allowing teams to focus on developing and maintaining a single version leading to lower TCO and easier maintainability. In full multi-tenancy customer specific variations can be built into the software as components that can be turned on or off based on the need.

## Automation
Successful SaaS vendors minimise any manual steps and build end-to-end automation across development, testing, deployment and operations. Automation capabilities and DevOps toolchain can drastically improve delivery quality and speed-to-market. 

For instance, on the infrastructure side companies should use Infrastructure-as-Code (IaC) tools like AWS CloudFormation or Terraform to increase automation and consistency of environments, to templatise and automate infrastructure stack creation. 

Companies should utilise the full DevOps toolchain that automates the workflow from coding to deployment. Automating the whole workflow is very important as any gaps in the automation will effectively become a bottleneck and kill the benefits that you were hoping to achieve. To achieve the end-to-end workflow automation, it is recommended to set up a dedicated team responsible for the DevOps toolchain and way of working.

We recommend our customers is to use a managed DevOps tool service rather than building their own toolchain. For instance, Azure DevOps is a great SaaS service provided by Microsoft that is also compatible with other public cloud platforms like AWS.

As your development teams will have more responsibility in the SaaS model, it is important to perform automated security and compliance tests. Start with automated reporting and compliance checks inserted into CI/CD pipeline complemented with cloud environment best-practices / anti-pattern checks.

## Microservices and Serverless
Microservice architecture and serverless let companies focus on functionality rather than integration. We tell our customers that whenever they start developing something new to their SaaS solution, they should always think if it can be implemented using serverless services like AWS Lambda, Azure Functions or GCP Cloud Functions. If serverless is not an option, they should build new functionality as microservices.

Serverless services allow you to build your functionality as event-driven components that are executed on-demand triggered by specific events, like database change, log activity etc. Serverless functions speed up development and deployment time and can significantly reduce cost as you only pay for the requests, not for the idle time.

Microservices architecture has been around for a while, but it is interesting that so many ISVs are still stuck in the world of traditional monoliths. Microservices are built to separate functionality as independent components, where the functionality is offered through APIs, and that can be developed and maintained without having to worry about dependency issues (given you don’t alter the APIs).

![Microservices](assets/images/posts/2020/microservices.png)

## Data as a Platform
Shared platform allows SaaS vendors to leverage insights from data aggregated across applications. In fact, a shared data layer is fast becoming the number one capability many ISVs and SaaS providers are after and which sets apart the successful providers from the rest. There are still many organisations that are not able to leverage data across their customer instances in an effective way. 

![Data as s Platform](assets/images/posts/2020/data_platform.png)

Public cloud offer unparalleled capabilities to build a consolidated data asset from your service. Even if you’re keeping your customer databases in separate locations, you can still benefit from having a shared data lake for insights and analytics. However, you might have to do anonymization in case of strict data policies. 

Shared data layer for applications is important not only for sharing data and getting platform wide analytics but also for compliance and auditability. Using cloud platform services (e.g. AWS Lakeformation) it is possible to build shared data layer with detailed access controls and audit trail. 

## Single Codebase
Having a single codebase can sound like an obvious thing but maintaining a strict single codebase policy requires dedication. SaaS vendors with multiple different versions of the code end up spending more on change implementation, deployment and maintenance. Instead of building customer specific functionality to different codebases or versions, you should have a single codebase and build customer specific functionality into common build through config options. This is in line with what I already wrote about multitenancy.

![Single Codebase](assets/images/posts/2020/single_codebase.png)

## Velocity of Innovation
The last common capability for successful SaaS vendors based on our experience is enabling velocity of innovation through public cloud. Having the possibility to shoot up a development environment in minutes or building your prototype as a serverless functions utilising cloud-native pre-built components can have a massive impact on the way you introduce new value adding services to your customers. 

We recently worked with a SaaS provider who wanted to create a new mobile service from scratch. Using AWS Lambda, we were able to develop the first prototype overnight, which would potentially have taken them weeks to develop in their old on-premise environment.

