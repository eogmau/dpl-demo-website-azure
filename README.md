---
topic: HTML Hello World
languages:
  - HTML
products:
  - Azure App Service
  - Azure Web Apps
---

# Dublin Pharmaceutical Limited Demo HTML Hello World website

This sample demonstrates a tiny Hello World HTML app for [App Service](https://docs.microsoft.com/azure/app-service).

# Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


## Download the sample

In the Cloud Shell, create a quickstart directory and then change to it.

```bash
mkdir quickstart

cd $HOME/quickstart
```

Next, run the following command to clone the sample app repository to your quickstart directory.

```bash
git clone https://github.com/eogmau/dpl-demo-website-azure.git
```
## Update or edit the webapp from Azure Shell

In the Cloud Shell, type `nano index.html` to open the nano text editor.
```bash
cd dpl-demo-website-azure

nano index.html
```

## Create a web app

Change to the directory that contains the sample code and run the `az webapp up` command.

In the following example, replace <app_name> with a unique app name.

```bash
az webapp up --location northeurope --name <app_name>
```

## Clean up resources

In the preceding steps, you created Azure resources in a resource group. If you don't expect to need these resources in the future, delete the resource group by running the following command in the Cloud Shell. Remember that the resource group name was automatically generated for you in the [create a web app](#create-a-web-app) step.

```bash
az group delete --name appsvc_rg_Windows_northeurope
```
