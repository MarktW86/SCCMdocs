---
title: "Endpoint Protection | System Center Configuration Manager"
ms.custom: na
ms.date: 07/27/2016
ms.prod: configuration-manager
ms.reviewer: na
ms.suite: na
ms.technology: 
  - configmgr-other
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 76c90f64-d729-456b-8304-01852cd66fb6
caps.latest.revision: 11
author: NathBarn

---
# Endpoint Protection in System Center Configuration Manager
Endpoint Protection in System Center Configuration Manager lets you to manage antimalware policies and Windows Firewall security for client computers in your Configuration Manager hierarchy.  
  
> [!IMPORTANT]  
>  You must be licensed to use Endpoint Protection to manage clients in your Configuration Manager hierarchy.  
  
 When you use Endpoint Protection with Configuration Manager, you have the following benefits:  
  
-   Configure antimalware policies, Windows Firewall settings, and manage Windows Defender Advanced Threat Protection to selected groups of computers  
  
-   Use Configuration Manager software updates to download the latest antimalware definition files to keep client computers up-to-date  
  
-   Send email notifications, use in-console monitoring, and view reports to keep administrative users informed when malware is detected on client computers  
  
Windows 10 computers don't require any additional client for endpoint protection management. On Windows 8.1 and earlier computers, Endpoint Protection installs its own client in addition to the Configuration Manager client. Endpoint Protection can manage. The Endpoint Protection client has the following capabilities:  
  
-   Malware and spyware detection and remediation  
  
-   Rootkit detection and remediation  
  
-   Critical vulnerability assessment and automatic definition and engine updates  
  
-   Network vulnerability detection through Network Inspection System  
  
-   Integration with Microsoft Active Protection Services to report malware to Microsoft. When you join this service, the Endpoint Protection client or Windows Defender can download the latest definitions from the Malware Protection Center when unidentified malware is detected on a computer.  
  
> [!NOTE]  
>  The Endpoint Protection client can be installed on a server that runs Hyper-V and on guest virtual machines with supported operating systems. To prevent excessive CPU usage, Endpoint Protection actions have a built-in randomized delay so that protection services do not run simultaneously.  
  
 In addition, Endpoint Protection in Configuration Manager lets you to manage Windows Firewall settings in the Configuration Manager console.  
  
 [Example scenario: Using System Center Endpoint Protection to protect computers from malware in System Center Configuration Manager](../Topic/Example%20scenario:%20Using%20System%20Center%20Endpoint%20Protection%20to%20protect%20computers%20from%20malware%20in%20System%20Center%20Configuration%20Manager.md) shows how you might configure and manage Endpoint Protection and the Windows Firewall.  
  
## Managing Malware with Endpoint Protection  
 Endpoint Protection in Configuration Manager allows you to create antimalware policies that contain settings for Endpoint Protection client configurations. You can then deploy these antimalware policies to client computers and monitor them in the **Endpoint Protection Status** node in the **Monitoring** workspace, or by using Configuration Manager reports.  
  
 Additional information:  
  
-   [How to create and deploy antimalware policies for Endpoint Protection in System Center Configuration Manager](../../protect/deploy-use/antimalware-policies-for-endpoint-protection.md) - Create, deploy, and monitor antimalware policies with a list of the settings that you can configure  
  
-   [How to monitor Endpoint Protection in System Center Configuration Manager](../../protect/deploy-use/monitor-endpoint-protection.md) - Monitoring activity reports, infected client computers, and more.  
  
-   [How to manage antimalware policies and firewall settings for Endpoint Protection in System Center Configuration Manager](../../protect/deploy-use/antimalware-firewall-settings-for-endpoint-protection.md) - Remediate malware found on client computers  
  
## Managing Windows Firewall with Endpoint Protection  
 Endpoint Protection in Configuration Manager provides basic management of the Windows Firewall on client computers. For each network profile, you can configure the following settings:  
  
-   Enable or disable the Windows Firewall.  
  
-   Block incoming connections, including those in the list of allowed programs.  
  
-   Notify the user when Windows Firewall blocks a new program.  
  
> [!NOTE]  
>  Endpoint Protection supports managing the Windows Firewall only.  
  
 For more information about how to create and deploy Windows Firewall policies for Endpoint Protection, see [How to create and deploy Windows Firewall policies for Endpoint Protection in System Center Configuration Manager](../../protect/deploy-use/create-deploy-windows-firewall-policies-for-endpoint-protection.md).  
  
## Windows Defender Advanced Threat Protection

Starting with the 1606 release of Configuration Manager (current branch), Endpoint Protection can help manage and monitor Windows Defender Advanced Threat Protection (ATP). Windows Defender ATP is a new service that will help enterprises to detect, investigate, and respond to advanced attacks on their networks. See [Windows Defender Advanced Threat Protection](../../protect/deploy-use/windows-defender-advanced-threat-protection.md).

## Endpoint Protection Workflow  
 Use the following diagram to help you understand the workflow to implement Endpoint Protection in your Configuration Manager hierarchy.  
  
 ![Endpoint Protection Workflow](../../protect/deploy-use/media/Endpoint-Protection-Workflow.gif "Endpoint)  
  
## Endpoint Protection Client for Mac Computers and Linux Servers  
 System Center 2012 includes an Endpoint Protection client for Linux and for Mac computers. These clients are not supplied with Configuration Manager; instead, you must download the following products from the [Microsoft Volume Licensing Service Center](https://www.microsoft.com/licensing/servicecenter/default.aspx).  
  
-   System Center 2012 Endpoint Protection for the Mac  
  
-   System Center 2012 Endpoint Protection for Linux  
  
> [!IMPORTANT]  
>  You must be a Microsoft Volume License customer to download the Endpoint Protection installation files for Linux and the Mac.  
  
 These products cannot be managed from the Configuration Manager console. However, a System Center Operations Manager management pack is supplied with the installation files, which allows you to manage the client for Linux by using Operations Manager.  
  
 For more information about how to install and manage the Endpoint Protection clients for Linux and Mac computers, use the documentation that accompanies these products, which is located in the **Documentation** folder.
