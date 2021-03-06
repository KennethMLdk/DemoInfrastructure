# DemoInfrastructure
An automated deployment for building infrastructure to M365 demo tenant

Deploys an isolated VNet and domain controller to your Azure subscription.

This deployment can be expanded with other on-premises services like PKI, NPS, etc, please fork and contribute if you can add to the project.

# Instructions
Connect to Azure subscription using Powershell or Az CLI
Run this cmdlet:

> New-AzSubscriptionDeployment -Name demoTenant -Location eastus -TemplateUri https://raw.githubusercontent.com/KennethMLdk/DemoInfrastructure/main/azuredeploy.json

You will be prompted for the demo tenant prefix parameter (that is the text in front of .onmicrosoft.com) e.g. m365x12345:

cmdlet New-AzDeployment at command pipeline position 1 <br>
Supply values for the following parameters:<br>
tenantPrefix: m365x12345
