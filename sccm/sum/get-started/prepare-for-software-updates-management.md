---
# required metadata

title: Prepare for software updates management | System Center Configuration Manager
description:
keywords:
author: dougeby
manager: angrobe
ms.date: 9/27/2016
ms.topic: article
ms.prod: configuration-manager
ms.service:
ms.technology:
  - configmgr-sum
ms.assetid: 01907900-e28b-4cd7-9479-42906416707b

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer:
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Prepare for software updates management
Before the compliance assessment data of the software update displays in the System Center Configuration Manager console and before you can deploy software updates to client computers, you must complete the steps in the following sections.

## Step 1: Install and configure a software update point  
The software update point is required on the central administration site and on the primary sites to enable the software updates compliance assessment and to deploy software updates to clients. The software update point is optional on secondary sites. For details, see [Install and configure a software update point](install-a-software-update-point.md)  

## Step 2: Synchronize Software Updates
Software updates synchronization is the process of retrieving the software updates metadata that meets the criteria that you configure. Software updates are not displayed in the Configuration Manager console until you synchronize software updates. For details, see [Synchronize Software Updates](synchronize-software-updates).   

## Step 3: Configure classifications and products to synchronize
Perform this configuration on the central administration site or stand-alone primary site. After you synchronize software updates the first time, Configuration Manager retrieves an updated list of classifications and products. Now, you can select from the new options in the Software Update Point Component properties. After you configure the new classifications and products, repeat step 2 to start software updates synchronization to retrieve software updates metadata for the new criteria. For details, see [Configure classifications and products to synchronize](configure-products-and-classifications.md).

## Step 4: Manage software updates settings
After you synchronize software updates, verify Configuration Manager client settings, group policy configurations, and software updates settings before you deploy software updates. For details, see [Configure classifications and products to synchronize](configure-products-and-classifications.md).