# Deploy a three node SQL Always on Availability Group w/ Virtual Network and Domain Controllers
This template will create a standalone Windows Server Domain with two Domain Controllers (primary and secondary) and three node SQL Always on Availability Group.

In addition to the servers, the template creates the underlying Azure Virtual Network with isolated subnets for management, applications and sql. Finally, the template also creates a Virtual Network Gateway with client IP pool for connection to an Azure App Service Plan. This template is intended to work in tandem with the PaaSwRedis-Stamp templates (URL below) to deploy an App Service with Redis cache and a SQL database backend:

Template to deploy App Service Plan with Redis Cache:<br>
https://github.com/albertwo1978/Project-010/tree/master/PaaSwRedis-Stamp

Below is a logical layout of the resources deployed by the template: 

+   Azure Region - 
    +   Virtual Network - 
        +   GatewaySubnet - Standard VPN Gateway w/ VPN Client IP pool (192.168.0.0/24) 
        +   mgmtSubnet    - Two Windows Server 2016 Domain Controllers in an Azure Availability Set 
        +   appSubnet     - EMPTY 
        +   sqlSubnet     - Three node SQL Always on Availability Group in an Azure Availability Set (templates allows selection between SQL 2012, 2014 and 2016) 

Click the button below to deploy from the portal:

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Falbertwo1978%2FProject-010%2Fmaster%2FIaaS-Stamp%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Falbertwo1978%2FProject-010%2Fmaster%2FIaaS-Stamp%2Fazuredeploy.json" target="_blank">
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
