---
title: "3. OpenLvVision SDK"
description: "Setting up the library for use on your system."
icon: "terminal"
weight: 1000003
draft: false
---

## Modules

OpenLVVision is built from several key libraries:

* **[Vision Development Module](/docs/installation/vision-development/)**: Provides core image function implementations in LabVIEW. **Note:** For an executable, you'll need to install the Vision Development runtime.
* **[Image](https://github.com/OpenLvVision/OpenLvVision_Image/releases)**: An open-source library offering fundamental image processing functions.
* **[Overlays](https://github.com/OpenLvVision/OpenLvVision_Overlays/releases)**: Manages graphics and images placed on top of a base image.
* **[OpenCV](https://github.com/OpenLvVision/OpenLvVision_OpenCv/releases)**: A free, widely used, open-source library for computer vision and image processing.

![Overview](images/OpenLvVision_Overview.png)

---

## JKI VIPM

All OpenLVVision packages are installed using the **[JKI VI Package Manager (VIPM)](https://www.vipm.io/)**.

1.  **Download VIPM** from [https://www.vipm.io/download/](https://www.vipm.io/download/) and install it.
2.  **Download** the individual `.vip` files for the OpenLVVision modules (linked above).
3.  **Open** the downloaded `.vip` files with VIPM to install them.


