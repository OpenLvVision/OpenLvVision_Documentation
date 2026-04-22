---
title: "3. OpenLvVision SDK"
description: "Setting up the library for use on your system."
icon: "terminal"
draft: false
---

\
OpenLVVision is built from several key libraries:

* **[Vision Common Resources](/docs/installation/vision-common-resources/)** Provides core image function implementations in LabVIEW.  
* **[Image](/docs/installation/openlvvision/#2-image-module)** Fundamental open-source image processing functions.  
* **[Overlays](/docs/installation/openlvvision/#3-overlays-module)** Tools for managing graphics and images placed on top of a base image.  
* **[OpenCV](/docs/installation/openlvvision/#4-opencv)**  A widely used, free, open-source library for computer vision and image processing.  

![Overview](images/OpenLvVision_Overview.png)

---

## 1. Installing JKI VIPM

All OpenLvVision packages are distributed via the **[JKI VI Package Manager (VIPM)](https://www.vipm.io/)**.

1. **Download VIPM** from [vipm.io/download](https://www.vipm.io/download/) and install it. 
![Download VIPM](images/VIP_Download.png) 

2. **Enable the LabVIEW VI Server** (required for VIPM to communicate with LabVIEW):  
   - Open **LabVIEW**.  
   - Go to **Tools Options VI Server**.  
   - Under **TCP/IP**, check **Enable TCP/IP**.  
   - Leave the **port** at its default value (each LabVIEW version has its own default port).  
   - Restart LabVIEW.  

   ![Enable VI Server](images/VIP_Port.png)

{{< alert context="info" text= "If VIPM cannot connect to LabVIEW, make sure the VI Server is enabled, LabVIEW is running, and your firewall is not blocking TCP connections on the configured port."/>}}


**Choose one of the following methods** to install the OpenLvVision modules:  

{{< tabs tabTotal="3">}}

{{% tab tabName="Inside VIPM" %}}
1. Open VIPM.  
2. Use the search bar to find **OpenLvVision**.  
3. Select the module you want to install.  
4. Click **Install**.  

![VIPM Search](images/VIP_Search.png)
{{% /tab %}}

{{% tab tabName="From .vip Files" %}}
1. Download the `.vip` files from the moduleâ€™s **GitHub Releases** page.  
2. Double-click the `.vip` file, or right-click â†’ **Open with VIPM**.  
3. Follow the installer prompts.  

![Install VIP File](images/VIP_FileInstall.png)
{{% /tab %}}

{{% tab tabName="From the Browser" %}}
1. Go to the moduleâ€™s package page on [vipm.io](https://www.vipm.io/).  
2. Click **Install with VIPM** (this will launch VIPM automatically).  
3. Confirm installation in VIPM.  

![Install VIP File](images/VIP_BrowserInstall.png)

{{% /tab %}}

{{< /tabs >}}

---

## 2. Image Module

An open-source library with fundamental image processing functions.

#### Download Links
- [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_Image/releases)  
- [VIPM Package](https://www.vipm.io/package/openlvvision_lib_openlvvision_image)  

---

## 3. Overlays Module

Provides functions for managing overlays (graphics and annotations) on images.

#### Download Links
- [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_Overlays/releases)  
- [VIPM Package](https://www.vipm.io/package/openlvvision_lib_openlvvision_overlays)  

---

## 4. OpenCv

A free, widely used, open-source library for computer vision and image processing.

{{< alert context="warning" text= "Requires an Internet connection to GitHub and AWS during installation! If this is not possible, please follow the offline installation guide below."/>}}

#### Download Links
- [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_OpenCv/releases)  
- [VIPM Package](https://www.vipm.io/package/openlvvision_lib_openlvvision_opencv/) 

#### Offline Installation

If you do not have internet access on the target machine, you can install the module manually. 

1. **Download the required files:**
   - **OpenCV:** [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_OpenCv/releases)
   - **Dependencies:** [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_OpenCv_Dependencies/releases/)
   - The `.vip` file (the package itself)
   - The associated `.zip` files:
     - Use the `x64` zips for **LabVIEW 64-bit**
     - Use the `x86` zips for **LabVIEW 32-bit** or **LabVIEW Community Edition**

   ![OpenCV Required Files](images/VIP_OpenCvFiles.png)

2. **Install the `.vip` file manually** via VIPM (see instructions in [Installing JKI VIPM](#1-installing-jki-vipm)). 

3. **During installation**, VIPM will display a window checking the connection.
   - If the installer cannot connect, it will automatically prompt you to select the downloaded `.zip` files.
   - If it does **not** prompt automatically:
     - Press the **Use offline files** button next to the download bar.
     - VIPM will then ask for the `.zip` files manually.

   ![OpenCV Offline Installation Prompt](images/VIP_OpenCvOffline.png)
