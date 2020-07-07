# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

The deployment process is very much easy in the App Service rather than the VM. The cost is an important factor when a service is choosed. And, I find Azure App service cheaper than the Azure Virtual machine (VM). Region availability is same for both products. You can get full control in the Virtual Machine, however for deplyoying this kind of application does not need any major control. As per the azure pricing calculator, 1 Instance of app service running 730 hours with 10 gb storage and 1.75 gb RAM with 2 Cpu Cores is costing aroung $54.75. But For VM with 2 CPU Cores it is costing me around 152$.

 Both are scalable but, the apps need to be redeployed after scaling up/down in case of VM. This is not the case with App Service, we dont have to restart the apps while scaling while scaling up and down. We can deploy multiple apps in App Service but in one VM Server we can only deploy one app. VM deployed app run simultaneously at 2 regions at a time, making it available 99.95% available. In App service it depends if we have multiple instances activated or not and also if they are in different regions.Even the deplyements are much faster in App service, so down time is less and app can become easily and quickly available.

In Azure app services, we can directly deploy the code from visual studio. Also, there is a recommendation from the Azure itself to use APP Service if deploying a Web app. I have attach that screenshot in the images folder.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

 I found App Service as a better choice because i found it easy to use, the cost was also less and it got easliy configured with my VSCode and application management. Even the deployement was automated and easy when I used App Service. Generally, Virtual machines are slow than actual machines. Also cost of esatblishing a server is very high, setting up all the infra is very high if we dont have cloud. 
VM would be good option if we need any immediate modifications and changes in the environment. 
Also VM requires more time for maintence which actually is not required in the project.
If we can make this better by using azure then its great.