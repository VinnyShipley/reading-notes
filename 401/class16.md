# Serverless Functions

## What is Serverless?

Serverless ia a cloud application development and execution model that lets devs build and run code without having to worry about server management or pay for idle cloud management. With serverless, devs only need to focus on creating the front end of an application, and then deploy those front end packages to the cloud service provider.

Serverless does not mean no servers, it simply refers yto outsourcing the server side creation and maintenance to a third party (AWS, Azure, Google Cloud, IBM Cloud engine). As needed, the amount of storage and functionality required from these third party server management companies will spin up and down. Because of this, you will only pay for the execution time and resources actually used.

## FaaS

FaaS, or function as a service, is a service that enables devs to run code or containers in response to specific events or requests, without specifying or managing the resources needed to run that code.

## Serverless vs. Platform as a service, containers, and virtual machines

* Provisioning time: Provisioning time is the process of setting up IT structure, as well as the steps required to manage data and resources making them available to users and systems. For serverless thus is measured in milliseconds, and minutes to hours for other systems.

* Administrative burden: Because of the hands off nature when it comes to maintaining a server with serverless for the dev, administrative burden only exists with models other than serverless.

* Maintenance: Similar to Administrative burden, serverless is taken care of by the provider, while other systems require maintenance when it comes to updating or managing systems.

* Scaling: Auto scaling is automatic with serverless, spinning up and down based on the front end usage, while non-serverless systems require auto-scaling code and lack the ability to scale to zero.

* Capacity planning: While some is needed for other systems, none is needed for serverless

* Statelessness: Statelessness is when a piece of code that runs with it's outcomes not being influenced by prior outcomes. This is a non-issue for serverless inherently, other systems keep an open socket or connection for long periods of time, and store state in memory between calls.

* Resource utilization: Inherently serverless has no idle capacity, while other systems will have some amount of idle capacity

## Kubernetes and Knative

Kubernetes is an open-source container orchestration platform that automates deployment, management and scaling of containers. Serverless apps are deployed in containers, but Kubernetes needs a specialized software that integrates Kubernetes into the specific cloud platform's serverless platform. Knative is an open-source extension of Kubernetes that allows any container on any Kubernetes utilizing cloud platform. Knative works by handling the network routing, event triggers and autoscaling of the application.

## Pros and Cons of Serverless

### Pros

* Improved dev productivity: Serverless allows devs to focus on writing code rather than managing infrastructure.

* Pay for execution only: Because of the spinning up nature of serverless, you only pay for exactly what you use.

* Develop in any language: Serverless is language agnostic, which allows the dev to write in whatever language they are comfortable in.

* Streamlined development in the DevOps cycle: Because the server side infrastructure and management is handled by serverless, testing and integration of backend code is essentially outsourced.

* Cost-effective performance: Serverless is can be both faster and more cost-effective than other forms.

### Cons

* Latency in certain programs: Serverless processes in favor of a scaling up and down to zero, which means that they forgo ongoing processes for cold starting, apps that cannot utilize cold starting should not use serverless.

* Higher cost for stable and predictable workloads: Because of the spinning up and down nature of serverless, it is more cost effective when the workload is spiky. When it is stable and constant, serverless isn't as cost effective.
