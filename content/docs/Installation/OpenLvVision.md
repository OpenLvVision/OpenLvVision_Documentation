---
title: "3. OpenLvVision SDK"
description: "Setting up the library for use on your system."
icon: "terminal"
draft: false
---

\
OpenLVVision is built from several key libraries:

* **[Vision Development Module](/docs/installation/vision-development/)** â€“ Provides core image function implementations in LabVIEW.  
  **Note:** For an executable, you'll need to install the Vision Development runtime.  
* **[Image](/docs/installation/openlvvision/#2-image-module)** â€“ Fundamental open-source image processing functions.  
* **[Overlays](/docs/installation/openlvvision/#3-overlays-module)** â€“ Tools for managing graphics and images placed on top of a base image.  
* **[OpenCV (Preview)](/docs/installation/openlvvision/#4-opencv-preview)** â€“ A widely used, free, open-source library for computer vision and image processing.  

![Overview](images/OpenLvVision_Overview.png)

---

## 1. Installing JKI VIPM

All OpenLvVision packages are distributed via the **[JKI VI Package Manager (VIPM)](https://www.vipm.io/)**.

1. **Download VIPM** from [vipm.io/download](https://www.vipm.io/download/) and install it. 
![Download VIPM](images/VIP_Download.png) 

2. **Enable the LabVIEW VI Server** (required for VIPM to communicate with LabVIEW):  
   - Open **LabVIEW**.  
   - Go to **Tools â†’ Options â†’ VI Server**.  
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

## 4. OpenCv Preview

A free, widely used, open-source library for computer vision and image processing.

{{< alert context="warning" text= "Requires an Internet connection to GitHub and AWS during installation! If this is not possible, please follow the offline installation guide below."/>}}

#### Download Links
- [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_OpenCv/releases)  
- [VIPM Package]() (coming soon)  

#### Offline Installation

If you do not have internet access on the target machine, you can install the module manually.  

1. **Download the required files** from [GitHub Releases](https://github.com/OpenLvVision/OpenLvVision_OpenCv/releases):  
   - The `.vip` file (the package itself)  
   - `DLLs.zip`  
     - Use `DLLs_x64` for **LabVIEW 64-bit**  
     - Use `DLLs_x86` for **LabVIEW 32-bit** or **LabVIEW Community Edition**  

   ![OpenCV Required Files](images/VIP_OpenCvFiles.png)

2. **Install the `.vip` file manually** via VIPM (see instructions in [Installing JKI VIPM](#1-installing-jki-vipm)).  

3. **During installation**, VIPM will display a window *â€œChecking Connectionâ€*.  
   - If the installer cannot connect, it will automatically prompt you to select the downloaded `DLLs.zip`.  
   - If it does **not** prompt automatically:  
     - Press the **Cancel** button next to the download bar.  
     - VIPM will then ask for the DLLs file manually â€” select the downloaded `DLLs.zip`.  

   ![OpenCV Offline Installation Prompt](images/VIP_OpenCvOffline.png)
