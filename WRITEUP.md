# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

Azure App Service was chosen because it provides a managed hosting environment, automatic patching, built-in monitoring, and simplified deployment for a Flask web application. This reduces operational overhead and allows development efforts to focus on application functionality rather than infrastructure management. My decision would change if the application's requirements evolved to include custom operating system configurations, third-party software that cannot be installed on App Service, specialized security controls, or complex networking dependencies. A Virtual Machine would also become a more suitable option if the application required complete administrative control, advanced performance tuning, or support for additional services running alongside the web application. Although this would increase management responsibilities and costs, the added flexibility would better support those expanded requirements.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

Cost Analysis

When comparing Azure App Service and Azure Virtual Machines, cost was an important factor in the decision-making process. Azure App Service provides a managed hosting platform where operating system maintenance, patching, monitoring, and platform updates are handled by Microsoft. This reduces operational costs and minimizes the administrative effort required to manage the application environment. In contrast, an Azure Virtual Machine requires management of the operating system, security updates, backups, and ongoing maintenance activities. While both services incur Azure hosting costs, a Virtual Machine often results in higher overall operational costs due to the additional infrastructure management responsibilities. For the relatively small Article CMS application, Azure App Service offers a more cost-effective solution.

Scalability Analysis

Scalability is another important consideration for web applications. Azure App Service provides built-in scaling capabilities, making it easy to increase or decrease resources based on demand. Additional instances can be added quickly without significant infrastructure changes, allowing the application to handle increased user traffic efficiently. On the other hand, scaling a Virtual Machine environment typically requires manual resizing of the VM, deployment of additional VMs, and configuration of load balancing solutions. Since the Article CMS application is expected to have moderate usage, Azure App Service provides sufficient scalability while requiring less effort to manage.

Availability Analysis

Azure App Service offers high availability through Microsoft's managed platform infrastructure. Platform updates, maintenance activities, and service reliability are largely handled automatically, reducing the risk of downtime. Although Azure Virtual Machines can also provide high availability, additional configurations such as availability zones, load balancers, backup solutions, and disaster recovery planning must be implemented and maintained by the administrator. For this project, Azure App Service provides a simpler and more reliable approach to maintaining application availability.

Workflow and Management Analysis

The application deployment workflow is significantly simpler with Azure App Service. The platform supports automated deployment through Azure DevOps, GitHub Actions, deployment centers, and Azure CLI, allowing developers to focus on application development rather than infrastructure maintenance. Azure handles server patching, runtime updates, and underlying platform management. In contrast, deploying the application on a Virtual Machine would require manual installation and configuration of Python, Flask, web servers, security updates, and ongoing system administration. While a VM provides greater flexibility and control, it also increases the operational workload.

Selected Resource Option

After evaluating cost, scalability, availability, and workflow considerations, Azure App Service was selected as the preferred deployment option for the Article CMS application. The application is a standard Flask-based web application that does not require extensive customization of the operating system or infrastructure. Azure App Service provides a managed environment that simplifies deployment, reduces operational overhead, offers built-in scaling capabilities, and improves overall reliability. These benefits make it the most appropriate and cost-effective solution for this project.

Assess App Changes That Would Change This Decision

My decision would change if the application requirements evolved to require a higher level of infrastructure control or specialized server configurations. For example, if the application needed custom operating system settings, third-party software installations, specialized networking configurations, or advanced performance tuning that is not supported by Azure App Service, then an Azure Virtual Machine would become the preferred deployment option. Similarly, if future business requirements demanded full administrative control over the hosting environment or integration with applications that require direct server access, a Virtual Machine would provide the necessary flexibility despite the additional management effort and cost. In such scenarios, the increased control offered by a VM would outweigh the operational advantages of Azure App Service.