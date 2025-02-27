---
title: Serverless computing
pcx_content_type: learning-unit
weight: 2
layout: learning-unit
---

Cloudflare Workers allows you to build serverless applications or augment existing ones by writing code that is deployed instantly across the globe. To understand the significance of Workers technology, we begin by understanding the environment in which it was developed.

Workers is a serverless computing provider. [Serverless computing](https://www.cloudflare.com/learning/serverless/what-is-serverless/) refers to a cloud computing model where providers, like Cloudflare, manage servers on behalf of users, allowing developers and businesses to focus entirely on writing and deploying application logic. 

## Cloud computing

[Cloud computing](https://www.cloudflare.com/learning/cloud/what-is-the-cloud/) is defined as hosting computing resources (such as virtual machines, storage, databases, and networking services) on third-party servers. Cloud computing service providers include Amazon Web Services, Microsoft Azure, Gooogle Cloud Platform, and Cloudflare.

### Serverless computing

Serverless computing is a subset of cloud computing. Serverless computing is a method of providing backend services on an as-used basis. A serverless provider allows users to write and deploy code without the hassle of worrying about the underlying infrastructure. Serverless computing has unique characteristics that set it apart from other cloud computing models.

#### Resource management

Cloud computing allows organizations to rent a fixed number of servers or server space. To prepare for seasonal or unplanned spikes in request traffic to their applications, organizations may overpurchase server space to ensure their applications do not go down because of high request volume from end users or customers.

In the serverless computing model, organizations and individuals are not required to calculate how much server space or machines they need to rent. Serverless computing providers take care of server management, and provisioning, allowing developers and organizations to focus on writing and deploying logic.

Serverless computing providers scale automatically to handle surges and low points in request traffic. The serverless computing provider is responsible for the scalability of your application and will work to match resources to the volume of requests your application is receiving, ensuring your application stays online.

#### Execution model

Serverless computing providers differ in their approach to how your application's code is executed. Many serverless computing providers, like Cloudflare, use an event-driven model. When an event (such as an HTTP request or a [Cron Trigger](/workers/configuration/cron-triggers/)) invokes a Worker, the Worker code will execute. The total amount of time from the start to end of an invocation of a Worker is known as [duration](/workers/platform/limits/#duration). The amount of time the CPU actually spends doing work during a given request is known as [CPU time](/workers/platform/pricing/#workers).

#### Billing model

Developers and organizations using serverless computing are billed on a usage model paradigm. Instead of paying for a fixed amount of computing resources that may be underutilized or exceeded, users pay as much as they use in the serverless model. Usage is defined differently per serverless computing provider. Usage in Workers is defined as CPU time.

## Summary

By reading this page, you have:

- Been introduced to the serverless computing concept that is behind Cloudflare Workers.
- Reviewed the differences between legacy on-premise and cloud computing infrastructure.
- Analyzed the key differences between the cloud computing and serverless computing paradigms.

In the next section, you will learn about what makes Workers, a serverless computing platform that is part of the larger Cloudflare Developer Platform, unique in its architecture from other serverless computing providers.