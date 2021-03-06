---
title: Supported clients and devices
titleSuffix: Configuration Manager
description: Learn which OS versions Configuration Manager supports for clients and devices.
ms.date: 10/02/2018
ms.prod: configuration-manager
ms.technology: configmgr-other
ms.topic: conceptual
ms.assetid: 87f4e041-67df-4c61-aa98-7444faffe565
author: aczechowski
ms.author: aaroncz
manager: dougeby
---

# Supported OS versions for clients and devices for Configuration Manager

*Applies to: System Center Configuration Manager (Current Branch)*

 Configuration Manager supports installing client software on Windows, Mac, Linux, and UNIX computers.  

#### Requirements and limitations for all clients  

-   Changing the startup type or **Log on as** settings for any Configuration Manager service isn't supported. This change can prevent key services from running correctly.    

-   Installing or running the Configuration Manager client for Linux or UNIX or the client for Mac on computers under an account other than root isn't supported. Doing so can prevent key services from running correctly.  



##  Windows computers  

 To manage the following Windows OS versions, use the client that's included with Configuration Manager. For more information, see [How to deploy clients to Windows computers](/sccm/core/clients/deploy/deploy-clients-to-windows-computers).  


### Supported client OS versions

-   **Windows 10**  

    For more detailed information, see [Support for Windows 10](/sccm/core/plan-design/configs/support-for-windows-10).  

-   **Windows 8.1** (x86, x64): Professional, Enterprise    

-   **Windows 7 with SP1** (x86, x64): Professional, Enterprise, and Ultimate    


### Supported server OS versions

-  **Windows Server 2019**: Standard, Datacenter <sup>[Note 1](#bkmk_note1)</sup>  
    (Starting with Configuration Manager version 1806.)

-  **Windows Server 2016**: Standard, Datacenter <sup>[Note 1](#bkmk_note1)</sup>  

-   **Windows Storage Server 2016**: Workgroup, Standard  

-   **Windows Server 2012 R2** (x64): Standard, Datacenter <sup>[Note 1](#bkmk_note1)</sup>    

-   **Windows Storage Server 2012 R2** (x64)    

-   **Windows Server 2012** (x64): Standard, Datacenter <sup>[Note 1](#bkmk_note1)</sup>    

-   **Windows Storage Server 2012** (x64)    

-   **Windows Server 2008 R2 with SP1** (x64): Standard, Enterprise, Datacenter <sup>[Note 1](#bkmk_note1)</sup>    

-   **Windows Storage Server 2008 R2** (x86, x64): Workgroup, Standard, Enterprise    

-   **Windows Server 2008 with SP2** (x86, x64): Standard, Enterprise, Datacenter <sup>[Note 1](#bkmk_note1)</sup>    


#### Server Core
The following versions specifically refer to the Server Core installation of the OS. <sup>[Note 3](#bkmk_note3)</sup>  

Windows Server semi-annual channel versions are Server Core installations, such as, Windows Server, version 1809. As a Configuration Manager client, they're supported the same as the associated Windows 10 semi-annual channel version. For more information, see [Support for Windows 10](/sccm/core/plan-design/configs/support-for-windows-10).


-   **Windows Server 2019** (x64) <sup>[Note 2](#bkmk_note2)</sup>  

-   **Windows Server 2016** (x64) <sup>[Note 2](#bkmk_note2)</sup>   

-   **Windows Server 2012 R2** (x64) <sup>[Note 2](#bkmk_note2)</sup>     

-   **Windows Server 2012** (x64) <sup>[Note 2](#bkmk_note2)</sup>     

-   **Windows Server 2008 R2** with no service pack, or with SP1 (x64)     

-   **Windows Server 2008 SP2** (x86, x64)   

#### <a name="bkmk_note1"></a> Note 1
 Configuration Manager tests and supports Windows Server Datacenter editions, but isn't officially certified for Windows Server. Configuration Manager hotfix support isn't offered for issues that are specific to Windows Server Datacenter Edition. For more information on the Windows Server certification program, see [Windows Server Catalog](https://www.windowsservercatalog.com/). 

#### <a name="bkmk_note2"></a> Note 2
 To support [client push installation](/sccm/core/clients/deploy/plan/client-installation-methods#client-push-installation), add the File Server service of the File and Storage Services server role. For more information about installing Windows features on Server Core, see [Install roles, role services, and features by using Windows PowerShell cmdlets](https://docs.microsoft.com/windows-server/administration/server-manager/install-or-uninstall-roles-role-services-or-features#BKMK_installwps).  

#### <a name="bkmk_note3"></a> Note 3
 The new Software Center app isn't supported on any version of Windows Server Core.<!--SCCMDocs issue 683-->



##  Windows Embedded computers  

 Manage Windows Embedded devices by installing the Configuration Manager client on the device. For more information, see [Planning for client deployment to Windows Embedded devices](/sccm/core/clients/deploy/plan/planning-for-client-deployment-to-windows-embedded-devices).  


### Requirements and limitations

-   All client features are supported on Windows Embedded systems that don't have write filters enabled.  

-   Clients that use one of the following are supported for all features except power management:  

    -   Enhanced Write Filters (EWF)    

    -   RAM File-Based Write Filters (FBWF)    

    -   Unified Write Filters (UWF)  

-   The Application Catalog isn't supported for any Windows Embedded device.  


### Supported OS versions  

-   **Windows 10 Enterprise** (x86, x64)  

-   **Windows 10 IoT Enterprise** (x86, x64)  
    This version includes the long-term servicing channel (LTSC). For more information, see [Overview of Windows 10 IoT Enterprise](https://docs.microsoft.com/windows/iot-core/windows-iot-enterprise).<!--SCCMDocs issue 560-->  

-   **Windows Embedded 8.1 Industry** (x86, x64)    

-   **Windows Embedded 8 Standard** (x86, x64)    

-   **Windows Thin PC** (x86, x64)    

-   **Windows Embedded POSReady 7** (x86, x64)    

-   **Windows Embedded Standard 7 with SP1** (x86, x64)    



## Windows CE computers

 Manage Windows CE devices with the Configuration Manager mobile device legacy client that is included with Configuration Manager.  


### Requirements and limitations  

-   The mobile device client requires 0.78 MB of storage space for installation. Sign-in can require up to 256 KB of additional storage space.    

-   Features for these mobile devices vary by platform and client type. For information about which management functions are supported, see [Choose a device management solution](/sccm/core/plan-design/choose-a-device-management-solution).  


### Supported OS versions  

-   Windows CE 7.0 (ARM and x86 processors)  

#### Supported languages include

-   Chinese (simplified and traditional)    

-   English (US)    

-   French (France)    

-   German    

-   Italian    

-   Japanese  

-   Korean  

-   Portuguese (Brazil)  

-   Russian  

-   Spanish (Spain)  



## Mac computers  

 Manage macOS computers with the Configuration Manager client for Mac.  

 The Mac client installation package isn't supplied with the Configuration Manager media. Download the **Clients for Additional Operating Systems** from the [Microsoft Download Center](http://go.microsoft.com/fwlink/?LinkID=525184).  

 For more information, see [How to deploy clients to Macs](/sccm/core/clients/deploy/deploy-clients-to-macs).  


### Supported versions

-   **Mac OS X 10.6** (Snow Leopard)

-   **Mac OS X 10.7** (Lion)

-   **Mac OS X 10.8** (Mountain Lion)

-   **Mac OS X 10.9** (Mavericks)

-   **Mac OS X 10.10** (Yosemite)  

-   **Mac OS X 10.11** (El Capitan)  

-   **Mac OS X 10.12** (macOS Sierra)

-   **Mac OS X 10.13** (macOS High Sierra)

- **macOS Mojave (10.14)** 


##  Linux and UNIX servers  

> [!Important]  
> As of March 22, 2018, the Linux and UNIX clients for Configuration Manager are deprecated. For more information, see [Deprecation announcement for Linux and Unix client support](/sccm/core/plan-design/changes/whats-new-in-version-1802#deprecation-announcement-for-linux-and-unix-client-support).  

 Manage Linux and UNIX servers with the Configuration Manager client for Linux and UNIX.  

 The Linux and UNIX client installation packages aren't supplied with the Configuration Manager media. Download the **Clients for Additional Operating Systems** from the [Microsoft Download Center](http://go.microsoft.com/fwlink/?LinkID=525184). In addition to client installation packages, the client download includes the script that manages the installation of the client on each computer.  


### Requirements and limitations

-   To review OS file dependencies for the client for Linux and UNIX, see [Prerequisites for client deployment to Linux and UNIX servers](/sccm/core/clients/deploy/plan/planning-for-client-deployment-to-linux-and-unix-computers#BKMK_ClientDeployPrereqforLnU).  

-   For an overview of supported management capabilities for Linux or UNIX, see [How to deploy clients to UNIX and Linux servers](/sccm/core/clients/deploy/deploy-clients-to-unix-and-linux-servers).  

-   For supported versions of Linux and UNIX, the listed version includes all subsequent minor versions. For example, CentOS version 6 includes  CentOS 6.3. Similarly, support for an OS that uses service packs (such as SUSE Linux Enterprise Server 11 SP1) includes subsequent service packs for that OS version.  

-   For information about client installation packages and the Universal Agent, see [How to deploy clients to UNIX and Linux servers](/sccm/core/clients/deploy/deploy-clients-to-unix-and-linux-servers).  


### Supported versions

The following versions are supported by using the indicated .tar file.  

#### AIX  

|Version|TAR file|  
|-|-|  
|Version 6.1 (Power)|ccm-Aix61ppc.&lt;build\>.tar|  
|Version 7.1 (Power)|ccm-Aix71ppc.&lt;build\>.tar|  

#### CentOS  

|Version|TAR file|  
|-|-|  
|Version 5 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 5 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 6 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 6 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 7 x64|ccm-Universalx64.&lt;build\>.tar|  

#### Debian  

|Version|TAR file|  
|-|-|  
|Version 5 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 5 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 6 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 6 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 7 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 7 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 8 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 8 x64|ccm-Universalx64.&lt;build\>.tar|  

#### HP-UX  

|Version|TAR file|  
|-|-|  
|Version 11iv3 IA64|ccm-HpuxB.11.31i64.&lt;build\>.tar|  

#### Oracle Linux  

|Version|TAR file|  
|-|-|  
|Version 5 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 5 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 6 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 6 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 7 x64|ccm-Universalx64.&lt;build\>.tar|  

#### Red Hat Enterprise Linux (RHEL)  

|Version|TAR file|  
|-|-|  
|Version 5 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 5 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 6 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 6 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 7 x64|ccm-Universalx64.&lt;build\>.tar|  

#### Solaris  

|Version|TAR file|  
|-|-|  
|Version 10 x86|ccm-Sol10x86.&lt;build\>.tar|  
|Version 10 SPARC|ccm-Sol10sparc.&lt;build\>.tar|  
|Version 11 x86|ccm-Sol11x86.&lt;build\>.tar|  
|Version 11 SPARC|ccm-Sol11sparc.&lt;build\>.tar|  

#### SUSE Linux Enterprise Server (SLES)  

|Version|TAR file|  
|-|-|  
|Version 10 SP1 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 10 SP1 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 11 SP1 x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 11 SP1 x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 12 x64|ccm-Universalx64.&lt;build\>.tar|  

#### Ubuntu  

|Version|TAR file|  
|-|-|  
|Version 10.04 LTS x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 10.04 LTS x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 12.04 LTS x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 12.04 LTS x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 14.04 LTS x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 14.04 LTS x64|ccm-Universalx64.&lt;build\>.tar|  
|Version 16.04 LTS x86|ccm-Universalx86.&lt;build\>.tar|  
|Version 16.04 LTS x64|ccm-Universalx64.&lt;build\>.tar|  



##  <a name="bkmk_OnpremOS"></a> On-premises mobile device management  

 Configuration Manager has built-in capabilities for managing devices that are on-premises without installing client software. For more information, see [Manage mobile devices with on-premises infrastructure](/sccm/mdm/understand/manage-mobile-devices-with-on-premises-infrastructure).  


### Requirements and limitations

-   Configure the **Service connection point** at the top-tier site of your hierarchy.  


### Supported operating systems

- **Windows 10 Pro** (x86, x64)  

- **Windows 10 Pro Enterprise** (x86, x64)  

- **Windows 10 IoT Enterprise** (x86, x64)  
    This version includes the long-term servicing channel (LTSC). For more information, see [Overview of Windows 10 IoT Enterprise](https://docs.microsoft.com/windows/iot-core/windows-iot-enterprise).<!--SCCMDocs issue 560-->  

- **Windows 10 Mobile**  

- **Windows 10 Mobile Enterprise**  

- **Windows 10 IoT Mobile Enterprise**  

- **Windows 10 Team for Surface Hub**  



##  <a name="bkmk_ExSrvConOS"></a> Exchange Server connector  

Configuration Manager supports limited management of devices that connect to your Exchange Server, without installing the Configuration Manager client. For more information, see [Manage mobile devices with Configuration Manager and Exchange](/sccm/mdm/deploy-use/manage-mobile-devices-with-exchange-activesync).  


### Supported versions of Exchange Server

- **Exchange Online (Office 365)**: This version includes Business Productivity Online Standard Suite  

- **Exchange Server 2016** (starting with version 1802)  

- **Exchange Server 2013**  

- **Exchange Server 2010 SP1** or **Exchange Server 2010 SP2** 
