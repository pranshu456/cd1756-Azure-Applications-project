# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

After analyzing the application requirements, I selected Azure App Service as the most appropriate deployment resource. Azure App Service provides a fully managed platform that simplifies hosting, scaling, monitoring, and securing web applications without requiring server management. It supports continuous integration and deployment from GitHub, making updates efficient and reliable. Compared to deploying virtual machines, App Service reduces operational overhead and maintenance costs while offering built-in features such as SSL certificates, automatic scaling, backups, and monitoring. This option delivers the best balance of performance, cost-effectiveness, security, and ease of management for a modern cloud-hosted web application.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

If the application requirements change, my deployment decision may also change. For example, if the application requires containerization, microservices architecture, or support for multiple technologies running together, I would consider Azure Kubernetes Service (AKS) instead of Azure App Service. Similarly, if the application needs full control over the operating system, custom software installations, or specialized network configurations, Azure Virtual Machines would be a better choice. Increased performance demands, complex scaling requirements, or stricter compliance and security needs could also influence the selection. Therefore, deployment resources should always be reassessed whenever application functionality, architecture, or operational requirements change.