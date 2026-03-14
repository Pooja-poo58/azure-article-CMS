# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

_For **both** a VM or App Service solution for the CMS app:_

- _Analyze costs, scalability, availability, and workflow_
- _Choose the appropriate solution (VM or App Service) for deploying the app_
- _Justify your choice_

### Cost

When using a Virtual Machine in Azure, the user has to manage the operating system, updates, storage and other infrastructure components. Because of this,the cost can be higher depending on the VM size and resources used.
Azure App Service is usually more cost-effective for web applications. The platform manages most of the infrastructure automatically which reduces management effort and operational cost.

### Scalability

Virtual Machines can be scaled by changing the VM size or using multiple VMs with load balancing. However, this requires manual setup and configuration by the developer.
Azure App Service provides easier scalability. It allows applications to scale automatically depending on traffic or resource usage. This makes it more convenient for handling increased demand.

### Availability

In a Virtual Machine setup, the developer must configure availability sets, backups, and load balancing to maintain application availability. This requires additional setup and monitoring.Azure App Service provides built-in high availability. Microsoft manages the infrastructure to ensure the application remains accessible with minimal downtime.

### Workflow

Deploying applications on a Virtual Machine requires setting up the server, installing required software and managing updates manually. This process takes more time and effort.Azure App Service simplifies the workflow by allowing direct deployment from repositories or local environments. The platform automatically handles the runtime environment and infrastructure management.

## Selected Solution

For this CMS application, Azure App Service is the better option. It simplifies deployment, reduces infrastructure management and provides built-in scalability and availability. Because the application is a web-based system, using App Service allows developers to focus on the application itself instead of managing servers.

### Assess app changes that would change your decision.

_Detail how the app and any other needs would have to change for you to change your decision in the last section._

## Assess App Changes

The current CMS application works well with Azure App Service because it is a simple web application and does not require full control over the server environment. App Service manages most of the infrastructure automatically, which makes deployment and scaling easier.
However, if the application required custom server configurations, special software installations, or deeper control over the operating system, then using an Azure Virtual Machine might be a better choice. In those cases, a VM would provide more flexibility to configure the environment according to specific application requirements.
