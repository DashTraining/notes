# Avbilder Demo Links

Running a real business for free* on Azure services!

These are the links to open during the Avbilderdemo. The narrative file has more context.

* [Public repository](https://github.com/DashTraining/Avbilder/)

## Opening: Free Is Complicated

## What Free Means In Azure

* [Explore free Azure services](https://azure.microsoft.com/en-us/pricing/free-services)
* [Microsoft Entra External ID pricing](https://www.microsoft.com/en-us/security/pricing/microsoft-entra-external-id)
* [Azure Monitor cost and usage](https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/cost-usage)

## Scenarios for Low-Cost Azure services

## Avbilder: The Concrete Example

* [Avbilder user site](https://www.avbilder.no)
* [Avbilder repository](https://github.com/DashTraining/Avbilder/)
* [Repository README](https://github.com/DashTraining/Avbilder/blob/main/README.md)
* [Demo setup documentation](https://github.com/DashTraining/Avbilder/blob/main/docs/setup.md)

## Architecture Setup

* [Architecture documentation](https://github.com/DashTraining/Avbilder/blob/main/docs/architecture.md)
* [Azure Static Web Apps documentation](https://learn.microsoft.com/en-us/azure/static-web-apps/overview)
* [Azure App Service documentation](https://learn.microsoft.com/en-us/azure/app-service/overview)

## User Registration And Booking Workflow

## Studio Approval

* [Avbilder admin app](https://app-avbilder-admin-weu.azurewebsites.net)

## Preview Upload

## Operating The Low-Cost App

* [Log Queries](https://github.com/DashTraining/Avbilder/blob/main/docs/log-queries.md)
* [Diagnostics documentation](https://github.com/DashTraining/Avbilder/blob/main/docs/diagnostics.md)

## Azure Advisor

* [Azure Advisor portal basics](https://learn.microsoft.com/en-us/azure/advisor/advisor-get-started)

## Deployment And Security Story

* [Main Bicep template](https://github.com/DashTraining/Avbilder/blob/main/infra/main.bicep)
* [Main Bicep parameters](https://github.com/DashTraining/Avbilder/blob/main/infra/main.bicepparam)
* [Customer site pipeline](https://github.com/DashTraining/Avbilder/blob/main/site-user/azure-pipelines.yml)
* [Public projects retirement in Azure DevOps](https://learn.microsoft.com/en-us/azure/devops/organizations/projects/public-projects-retirement?view=azure-devops)

## Optional Automation Segment

* [Cleanup runbook](https://github.com/DashTraining/Avbilder/blob/main/infra/automation/Cleanup-ExpiredPreviews.ps1)

## Upgrade Paths And Closing

* [Future ideas and upgrade paths](https://github.com/DashTraining/Avbilder/blob/main/docs/future-ideas.md)
* [FAQ](FAQ.md)

## Failure Fallbacks

* [If admin sign-in behaves oddly](https://app-avbilder-admin-weu.azurewebsites.net/.auth/me)
* [Purge consent here](https://identity.azurestaticapps.net/.auth/purge/aad)
