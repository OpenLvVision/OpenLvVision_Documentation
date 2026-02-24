---
title: "2. Vision Common Resources"
description: "Install the image processing addon for LabVIEW" 
icon: "visibility"
draft: false
---

## Licensing

OpenLvVision manages fundamental LabVIEW image data types by interfacing with the NI Vision Common Resources package. This driver provides the core libraries necessary for basic image management and display controls across Windows

## Installation

{{< tabs tabTotal="2">}}
{{% tab tabName="Ni-Package Manager" %}}

To install the necessary image handling components, use the NI Package Manager with these steps:

1.  **Launch NI Package Manager (as Administrator):**
    * Locate the NI Package Manager application on your system.
    * Right-click on the application icon.
    * Select "Run as administrator."

2.  **Search for the  Vision Common Resources Module:**
    * Once the NI Package Manager is open, use the search bar to find "Vision Common Resources"

	![Search for Vision Common Resources in NI Package Manager](images/VCR_Search.png)

3.  **Select Compatible Version:**
    * Select the "Vision Common Resources" package that matches the *exact* version of your installed LabVIEW.
    * Matching the versions is critical to prevent compatibility issues.

4.  **Initiate Installation:**
    * Click the "Install" button next to the correct "Vision Common Resources" package.
    * Follow all the on-screen instructions provided by the NI Package Manager to complete the installation.

![NI Vision Common Resources installation in NI Package Manager](images/VCR_Ni-Install.png)

{{% /tab %}}
{{% tab tabName="Manually" %}}

To obtain the necessary files for image handling, visit the National Instruments website to download the NI Vision Common Resources installer:
[https://www.ni.com/en/support/downloads/drivers/download.vision-common-resources.html](hhttps://www.ni.com/en/support/downloads/drivers/download.vision-common-resources.html)

1.  **Select Matching Version:** 
    * Ensure you choose the download for the NI Vision Common Resources version that precisely matches the version of LabVIEW you have installed on your system.

2.  **Download and Install:** 
    * Click the download button to obtain the installer. 
    * Once downloaded, run the installer and follow the on-screen instructions to install the NI Vision Common Resources .

![NI Vision Common Resources Download Page](images/VCR_Download.png)

{{% /tab %}}
{{< /tabs >}}
