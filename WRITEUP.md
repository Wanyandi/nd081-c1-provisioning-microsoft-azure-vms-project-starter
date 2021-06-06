# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

**VMs** Configuration of the application server/framework in the VM. Integration with Azure services. OS patch management. Design and configure the application and infrastructure to handle fluctuating traffic. Seamless platform switching Security configuration. Identify and apply monitoring strategy for application VM Availability SLA upto 99.99% Cost : Virtual Machines 1 D2 v3 (2 vCPUs, 8 GB RAM) x 730 Hours; Windows – (OS Only); Pay as you go; 0 managed disks – S4, 100 transaction units; Inter Region transfer type, 5 GB outbound data transfer from West US to East Asia Monthly: $152.62

**App Service**

Instant deployment. Vertical scaling, without having to redeploy. Support for multiple deployments (like staging and production). Automatic OS upgrades for your infrastructure. Integration capability with Git. Integration capability with MySQL. Higher SLA with two or more instances. Recommended for production environments. Can scale down to zero after job completes. App Service Availability SLA upto 99.95%

**Cost: App Service**

Basic Tier; 1 B1 (1 Core(s), 1.75 GB RAM, 10 GB Storage) x 730 Hours; Windows OS Monthly:$54.75

I will use App service Basic Tier since its easier to deploy, connects with Github where the Code is running, does not requiure any Infrastructure management and has a free option for testing purposes

**Assess app changes that would change your decision.**
*The Limitation for App Service taht would cause to chenge to Azure VM

*You have limited access to the host server, so you are unable to control the underlying OS or install software on the server. *You’re always paying for the service plan, even if your services or application isn’t running. *There are hardware limitations, such as a maximum of 14GB of memory and 4 vCPU cores per instance *While they support multiple languages, as noted in the benefits above, they are limited to just using those languages (as of when this course was built).
