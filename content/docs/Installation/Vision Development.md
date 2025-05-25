---
title: "2. Ni Vision Development Module"
description: "Install the image processing addons for LabVIEW" 
icon: "visibility"
weight: 1000002
draft: false
---

## Licensing

Internally the NI Vision Development Module is structured into multiple libraries. \
OpenLvVision utilizes the core library (`nivissvc.dll`) for fundamental LabVIEW image data type management, and this does **not** require a license. \
In contrast, advanced image processing functions reside within separate, licensed DLLs (like `nivision.dll`). \
OpenLvVision's goal is to offer free, open-source alternatives to these licensed advanced functions.

{{< alert context="success" text= "Core image handling functions for Ni-Vision-Development is license-free, will be used by OpenLvVision"/>}} 

## Installation

{{< tabs tabTotal="2">}}
{{% tab tabName="Ni-Package Manager" %}}

To install the necessary image handling components, use the NI Package Manager with these steps:

1.  **Launch NI Package Manager (as Administrator):**
    * Locate the NI Package Manager application on your system.
    * Right-click on the application icon.
    * Select "Run as administrator."

2.  **Search for the Module:**
    * Once the NI Package Manager is open, use the search bar to find "Vision Development."

	![Search for Vision Development in NI Package Manager](images/VisionDevelopment_Search.png)

3.  **Select Compatible Version:**
    * Carefully select the "Vision Development" package that matches the *exact* version of your installed LabVIEW.
    * Matching the versions is critical to prevent compatibility issues.

4.  **Initiate Installation:**
    * Click the "Install" button next to the correct "Vision Development" package.
    * Follow all the on-screen instructions provided by the NI Package Manager to complete the installation.

![NI Vision Development Module Installation in NI Package Manager](images/VisionDevelopment_Ni-Install.png)

{{% /tab %}}
{{% tab tabName="Manually" %}}

To obtain the necessary files for image handling, visit the National Instruments website to download the NI Vision Development Module installer:
[https://www.ni.com/en/support/downloads/software-products/download.vision-development-module.html](https://www.ni.com/en/support/downloads/software-products/download.vision-development-module.html)

1.  **Select Matching Version:** 
    * Ensure you choose the download for the NI Vision Development Module version that precisely matches the version of LabVIEW you have installed on your system.

2.  **Choose Full Version:** 
     * Select the "Full" version of the module. 
     * The "Runtime" version is only required for deployment on target systems that do not have the full LabVIEW development environment installed and are running your application as an executable. For development purposes, the Full version is necessary.

3.  **Download and Install:** 
    * Click the download button to obtain the installer. 
    * Once downloaded, run the installer and follow the on-screen instructions to install the NI Vision Development Module.
    * **Important:** If you don't see a download button, this version of the module needs to be installed using the NI Package Manager (see previous section).

![NI Vision Development Module Download Page](images/VisionDevelopment_Download.png)

{{% /tab %}}
{{< /tabs >}}