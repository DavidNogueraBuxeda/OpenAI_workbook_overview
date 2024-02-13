# OpenAI_workbook_overview
Workbook to overview the OpenAI instances deployed on Azure.



## Introduction
With this workbook, we want to achieve a comprehensive and easy-to-use dashboard that can help us monitor and manage the openai instances that we have deployed. We want to show various metrics and statistics that can help us identify any issues or opportunities for improvement in our openai usage and performance.
- How many openai instances do we have and what are their statuses?
- How many data models we deployed for each instance? Are we reaching the limit of tokens?
- How much prompt tokens for Data model are we using for each openai instance and how does it compare to the allocated resources?
- How many queries are we sending to each openai instance and what is the average response time and latency?
- What are the most common errors or failures that we encounter with each openai instance?
- How many openAI instances can we need to improve our efficiency and quality?
To answer these questions, we have designed several graphs and tables that display the relevant data and information for each openai instance. In the following sections, we will explain the details of each graph and how to interpret them.

## What do we want to show and why (frequent client asks/problems) -> explain details of each graph
One of the main questions that we want to answer is how many openAI instances can we need to improve our efficiency and quality. This depends on several factors, such as the number of users, the complexity of the queries, the availability of the resources, and the budget constraints. 
To help us estimate the optimal number of openAI instances for our needs, we have created a graph that shows the relationship between the number of instances and the performance metrics, such as accuracy, speed, and performance.
Based on that we can see if we require PTUs to provide a guarantee SLA.

## Requirements
We require 2 different rights to get all the graphs.

a)	Reader access to the OpenAI instances to check azure metrics values from the instances.

b)	Export diagnostic settings (Request and Response Logs)  and reader access to the log analytics instance or at least on the AzureDiagnostics table.

## How to setup things

| Deployment Type | Link |
|:--|:--|
| Azure portal UI |[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#blade/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3A%2F%2Fwww.github.com%2FDavidNogueraBuxeda%2FOpenAI_workbook_overview%2Fmain%2Fblob%2Fworkload%2Farm_template%2FOverviewOpenAI.json/uiFormDefinitionUri/https%3A%2F%2Fwww.github.com%2FDavidNogueraBuxeda%2FOpenAI_workbook_overview%2Fmain%2Fblob%2Fworkload%2Farm_template%2FOverviewOpenAI.json) |



| Azure portal UI |[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#blade/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3A%2F%2Fraw.github.com%2FDavidNogueraBuxeda%2FOpenAI_workbook_overview%2Fmain%2Fworkload%2Farm_template%2FOverviewOpenAI.json/uiFormDefinitionUri/https%3A%2F%2Fraw.githubusercontent.com%2FDavidNogueraBuxeda%2FOpenAI_workbook_overview%2Fmain%2Fworkload%2Farm_template%2FOverviewOpenAI.json) |


https://raw.githubusercontent.com/DavidNogueraBuxeda/OpenAI_workbook_overview/master/workbook/OverviewOpenAI.json

https://www.github.com/DavidNogueraBuxeda/OpenAI_workbook_overview/master/workbook/OverviewOpenAI.json


https://github.com/Azure/azure-quickstart-templates/blob/master/sharepoint-adfs/azuredeploy.json
But somehow now Azure seems to require this format:
https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/sharepoint-adfs/azuredeploy.json

https://github.com/DavidNogueraBuxeda/OpenAI_workbook_overview/blob/main/workbook/arm_template/OverviewOpenAI.json

https://github.com/DavidNogueraBuxeda/OpenAI_workbook_overview/blob/main/workbook/arm_template/OverviewOpenAI.json


https://github.com/DavidNogueraBuxeda/OpenAI_workbook_overview/blob/main/workbook/arm_template/OverviewOpenAI.json


https%3A%2F%2Fraw.githubusercontent.com%2FOpenAI_workbook_overview%2Fmain%2Fworkload%2arm_template%2FOverviewOpenAI.json

https://portal.azure.com/#blade/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3A%2F%2Fraw.githubusercontent.com%2OpenAI_workbook_overview%2Fmain%2Fworkbook%2Farm_template%2FOverviewOpenAI.json/uiFormDefinitionUri/https%3A%2F%2Fraw.githubusercontent.com%2OpenAI_workbook_overview%2Fmain%2Fworkbook%2Farm_template%2FOverviewOpenAI.json

| Azure portal UI |[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#blade/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Favdaccelerator%2Fmain%2Fworkload%2Farm%2Fdeploy-baseline.json/uiFormDefinitionUri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Favdaccelerator%2Fmain%2Fworkload%2Fportal-ui%2Fportal-ui-baseline.json) [![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.us/#blade/Microsoft_Azure_CreateUIDef/CustomDeploymentBlade/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Favdaccelerator%2Fmain%2Fworkload%2Farm%2Fdeploy-baseline.json/uiFormDefinitionUri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Favdaccelerator%2Fmain%2Fworkload%2Fportal-ui%2Fportal-ui-baseline.json)|
| Command line (Bicep/ARM) | [![Powershell/Azure CLI](./workload/docs/icons/powershell.png)](./workload/bicep/readme.md#avd-accelerator-baseline) |
| Terraform | [![Terraform](./workload/docs/icons/terraform.png)](./workload/terraform/greenfield/readme.md) |


