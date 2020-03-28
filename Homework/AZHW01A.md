#### Roxanna Barahona
#### Homework: ISTA 422 ch1A
#### March 22, 2020

1. What are the differences between Iaas, Paas, and Saas?
- IaaS: Infrastructure As A Service
-- An IaaS cloud vendor runs and manages server farms running virtualization software, enabling you to create VMs that run on the vendor’s infrastructure. Depending on the vendor, you can create a VM
4 CHAPTER 1 | Getting started with Microsoft Azure
running Windows or Linux and install anything you want on it. Azure provides the ability to set up virtual networks, load balancers, and storage and to use many other services that run on its infrastructure. You don’t have control over the hardware or virtualization software, but you do have control over almost everything else. In fact, unlike PaaS, you are completely responsible for it.
-- examples: Virtual Machines // Azure VM Scale Sets (VMSS) is built on top of Azure Virtual Machines and provides an easy way to deploy clusters of identical VM

- PaaS: Platform As A Service
-- With PaaS, you deploy your application into an application-hosting environment provided by the cloud service vendor. The developer provides the application, and the PaaS vendor provides the ability to deploy and run it. This frees developers from infrastructure management, allowing them to focus strictly on development.
-- Examples: Azure Cloud Services(Web and Worker Roles)

- SaaS: Software As A Service: SaaS is software that is centrally hosted and managed for the end customer. It usually is based on a multitenant architecture—a single version of the application is used for all customers. It can be scaled out to multiple instances to ensure the best performance in all locations. SaaS software typically is licensed through a monthly or annual subscription.
-- Examples: Microsoft Office 365, Dropbox, WordPress, Amazon Kindle

2. What is the Azure Service Management (ASM) deployment model? What is the Resource Manager
deployment model?
- Azure Service Management (ASM)
-- referred to as "classic" and it is the deployment model that has been used to deploy services
-- deployments happen sequentially

- Resource Manager deployment model
-- modern, more functional replacement for ASM. The Resource Manager deployment model is recommended for all new Azure workloads.
-- With Resource Manager, you deploy these assets into the same resource group and manage and monitor them together. You can deploy, update, or delete all of the resources in a resource group in one operation. Once you are done deploying you Resource manager provides security, auditing, and tagging to help you manage your resources.
- PROS to Resource Manager deployment model
- faster (deployed in parallel)
- you can use powershell cmdlets
- each service has its own service provider and therefore can update independently of the other services
- You can use the new Role-Based Access Control (RBAC) to control access to the resources in the group. For example, you can assign the Owner role to a user, giving that user full administrative privileges to those resources in the group but not to other resources in the subscription.
- advantages continue on page 5

 - BOTH
 -- These deployment models are often referred to as control planes because they are used to control services, not just to deploy them.

3. What is the difference between a control plane and a data plane?
These (resource manager and azure service management) deployment models are often referred to as control planes because they are used to control services, not just to deploy them. This is different from a data plane, which manages the data used by a service.

4. What is Role-Based Access Control?
- allows you to grant either full administrative privileges to everything in a subscription or no access at all

5. Why would you want to create a custom role for role-based access control?
- in case you want to giver a user owner or administrative privileges or if you need to remove someones access

6. Consider the Azure portal. What is the dashboard? What is the hub? What is a blade?
- dashboard: the dashboard is the GUI of the azure portal that the user first comes across when accessing the website.
- hub: hub; it shows you a core set of options such as Resource Groups, All Resources, and Recent
- blade: A blind is similar to a window, when you click a hyperlink it will open a new blade (page/window)


7. Access the conceptual Azure documentation on Github. Search the documentation and answer this
question: What happens when I reach the spending limit?
- The spending limit in Azure prevents spending over your credit amount.
- When your usage results in charges that exhaust your spending limit, the services that you deployed are disabled for the rest of that billing period.

8. Access the Azure samples on Github. Search for an example that will allow you to download an Azure
invoice. Copy the source code to your discussion. (This is Program.cs.)
- LINK: https://github.com/Azure-Samples/billing-dotnet-core-invoice-download/blob/master/Program.cs

9. Access the Azure Resource Manager samples on Github. Search for a quickstart template that will
allow you to set up a free SQL Database for a web application. This template has four files. One file
is a markdown file. What is the type of the other three files?
- LINK: https://docs.microsoft.com/en-us/azure/app-service/samples-resource-manager-templates

- unsure * : JSON, Metadata, azuredeploy.json?
