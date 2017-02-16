# Deploy a Web App, Azure SQL Database and Redis Cache
This template creates an Azure Web App with SQL Database and Redis Cache. The template requests a SQL connection string. This is currently not used, but will be added to integrate with a SQL database in a future iteration.

This template is intended to work in tandem with the IaaS-Stamp templates (URL below) to deploy a Vurtual Netowkr with Domain Controllers and SQL Always on Availability Cluster:

Template to deploy the IaaS Stamp:<br>
https://github.com/albertwo1978/Project-010/tree/master/IaaS-Stamp

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
    +   Azure SQL settings
    +   Redis Cache Settings 
+   Future interation will not create Azure SQL and will connect to an existing SQL database based on connection strings provided.

## Deploying Sample Templates

You can deploy these samples directly through the Azure Portal.

To deploy the sample using the Azure Portal, click the **Deploy to Azure** button found above.