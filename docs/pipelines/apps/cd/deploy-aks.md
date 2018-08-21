---
title: Deploy a Docker container app to an Azure Kubernetes Service (AKS)
description: Set up continuous deployment (CD) of a Docker-enabled app to an Azure Kubernetes Service (AKS) from Azure Pipelines
ms.assetid:
ms.prod: devops
ms.technology: devops-cicd
ms.topic: quickstart
ms.manager: douge
ms.author: ahomer
author: alexhomer1
ms.date: 04/09/2018
monikerRange: 'vsts'
---

# Deploy to an Azure Web App for Containers

We'll show you how to set up continuous deployment of your containerized application to an Azure Kubernetes Service (AKS) using
Azure Pipelines.

After you commit and push a code change, it is be automatically built and then deployed. The results will automatically show up on your site.

## Example

If you want some sample code that works with this guidance, import (into VSTS or TFS) or fork (into GitHub) this repo:

```
https://github.com/adventworks/dotnetcore-k8s-sample

```


## Define your CI build process

You'll need a continuous integration (CI) build process that publishes a container image to any container registry (for example: Azure Container Registry) and a Helm chart.
To set up a CI build process, see:

* [Build Docker image and publish Helm chart](../../languages/docker.md).

## Prerequisites

You'll need an Azure subscription. You can get one free through [Visual Studio Dev Essentials](https://visualstudio.microsoft.com/dev-essentials/).

[!INCLUDE [create-azure-webapp-to-host-container](../_shared/create-azure-webapp-to-host-container.md)]

[!INCLUDE [create-release-azure-webapp-container](../_shared/create-release-azure-webapp-container.md)]

## Next steps

* [Set up multi-stage release](../../release/define-multistage-release-process.md)
