---
title: "Use multicast to deploy Windows over the network with System Center Configuration Manager"
ms.custom: na
ms.date: 12/08/2015
ms.prod: configuration-manager
ms.reviewer: na
ms.suite: na
ms.technology: 
  - configmgr-osd
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 4cafb7fc-380b-41b1-b83e-045aebfb7131
caps.latest.revision: 13
author: Dougeby

---
# Use multicast to deploy Windows over the network with System Center Configuration Manager
Multicast is a network optimization method that you can use in your System Center Configuration Manager environment where multiple clients are likely to download the same operating system image at the same time. When multicast is used, multiple computers simultaneously download the operating system image as it is multicast by the distribution point, rather than having the distribution point send a copy of the data to each client over a separate connection.  
  
 You can deploy operating systems over the network by using multicast in the following operating system deployment scenarios:  
  
-   [Refresh an existing computer with a new version of Windows using System Center Configuration Manager](../../osd/deploy-use/refresh-an-existing-computer-with-a-new-version-of-windows.md)  
  
-   [Install a new version of Windows on a new computer (bare metal) with System Center Configuration Manager](../../osd/deploy-use/install-new-windows-version-new-computer-bare-metal.md)  
  
 Complete the steps in one of the operating system deployment scenarios and then use the following sections to support multicast.  
  
##  <a name="BKMK_Configure"></a> Configure a distribution point to support multicast  
 To use multicast when you   deploy operating systems, you must configure a distribution point to support multicast. For more information, see [Configure distribution points to support multicast](../../osd/plan-design/prepare-site-system-roles-for-operating-system-deployments.md#BKMK_DPMulticast).  
  
## Prepare an operating system image for multicast deployments  
 To configure the operating system image package to support multicast, see [Prepare the operating system image for multicast deployments](../../osd/deploy-use/manage-operating-system-images.md#BKMK_OSImageMulticast).  
  
##  <a name="BKMK_Deploy"></a> Deploy the task sequence  
 Deploy the operating system to a target collection. For more information, see [Deploy a task sequence](../../osd/deploy-use/manage-task-sequences-to-automate-tasks.md#BKMK_DeployTS).  
  
## See Also  
 [Methods to deploy enterprise operating systems using System Center Configuration Manager](../../osd/deploy-use/methods-to-deploy-enterprise-operating-systems.md)
