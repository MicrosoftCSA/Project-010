# Create a complete SQL HA IaaS Stamp w/ Virtual Network and Domain Controllers
This template will create a standalone Windows Server Domain with two Domain Controllers (primary and secondary) and three node SQL 2016 Always on Availability Group.

In addition to the servers, the template creates the underlying Azure Virtual Network with isolated subnets for management, applications and sql. Finally, the template also creates a Virtual Network Gateway with client IP pool for connection to an Azure App Service Plan. This template is intended to work in tandem with the PaaSwRedis-Stamp templates (URL below) to deploy an App Service with Redis cache and a SQL database backend:

Template to deploy App Service Plan with Redis Cache:

https://github.com/albertwo1978/Project-010/tree/master/PaaSwRedis-Stamp

Click the button below to deploy from the portal:

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Falbertwo1978%2FProject-010%2Fmaster%2FIaaS-Stamp%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Falbertwo1978%2FProject-010%2Fmaster%2FIaaS-Stamp%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>
