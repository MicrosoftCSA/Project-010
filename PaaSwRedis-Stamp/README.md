# Deploy a Web App, Azure SQL Database and Redis Cache
This template creates an Azure Web App with SQL Database and Redis Cache. The template requests a SQL connection string. This is currently not used, but will be added to integrate with a SQL database in a future iteration.

This template is intended to work in tandem with the IaaS-Stamp templates (URL below) to deploy an IaaS stamp with SQL Always on Availability Cluster:

Template to deploy the IaaS Stamp:<br>
https://github.com/albertwo1978/Project-010/tree/master/IaaS-Stamp

Below is a logical layout of the resources deployed by the template: 

Click the button below to deploy from the portal:

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Falbertwo1978%2FProject-010%2Fmaster%2FPaaSwRedis-Stamp%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Falbertwo1978%2FProject-010%2Fmaster%2FPaaSwRedis-Stamp%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Notes

+	The templates allows the administrator to select the following parameters at runtime:
    +   Azure Region and Resource Group 
    +   VM sizes and Storage Account Type
    +   Active Directory Domain Name
    +   Domain and SQL Service account name and passwords
    +   Virtual Network Address Ranges
    +   SQL Version and Workload Type
    +   AOAG Listener settings
    +   SQL Patch Windows

## Deploying Sample Templates

You can deploy these samples directly through the Azure Portal.

To deploy the sample using the Azure Portal, click the **Deploy to Azure** button found above.