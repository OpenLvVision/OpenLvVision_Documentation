---
title: "1. LabVIEW"
description: "Setting up the library for use on your system."
icon: "terminal"
draft: false
---


## 1. Download LabVIEW

To begin, you need to download the LabVIEW installer from the National Instruments website.

**Access the Download Page:** You can find the appropriate download page at the following URL: [https://www.ni.com/en/support/downloads/software-products/download.labview.html](https://www.ni.com/en/support/downloads/software-products/download.labview.html)

1. **Identify the Correct Version:**
    * It's crucial to download a compatible version. Ensure that you select LabVIEW 2024 Q1 or a later release.
2. **Choose the Appropriate License:**
    * If you possess a commercial LabVIEW license, proceed with that version.
    * Otherwise, for free, non-commercial use, select and download the Community Edition.
3. **Download the Installer:**
    * Click the download button to obtain the LabVIEW installer package.

![LabVIEW Download Page](images/Labview_Download.png)

## 2. Install LabVIEW

After downloading, follow these steps to install LabVIEW:

* **Mount the ISO (If Applicable):**
    * If the downloaded file is an ISO image, you'll need to mount it. In Windows, you can typically do this by double-clicking the ISO file. This will create a virtual drive.

    ![Mounting the Installer](images/Labview_MountInstaller.png)

* **Run the Installer:**
    * Navigate to the newly created virtual drive (or the location where you extracted the installer files).
    * Locate the `Install.exe` file.
    * **Important:** Right-click on `Install.exe` and select "Run as administrator." This ensures the installer has the necessary permissions.

* **NI Package Manager:**
    * The LabVIEW installer often begins by installing the NI Package Manager. This is a tool that helps manage NI software installations. Follow the on-screen prompts to complete the NI Package Manager installation.

* **LabVIEW Installation:**
    * Once the NI Package Manager is installed, the LabVIEW installation process will start.
    * Carefully follow the on-screen instructions. You may be presented with options to customize the installation (e.g., selecting specific modules or drivers). If you're unsure, the default settings are usually a good starting point.

* **JKI VI Package Manager:**
    * During the LabVIEW installation, you may be prompted to install the JKI VI Package Manager. It is highly recommended that you enable this.The JKI VI Package Manager is a valuable tool for managing LabVIEW libraries and add-ons. **It will later be used to install OpenLvVision.**

    ![JKI VI Package Manager Selection](images/Labview_VIMP.png)

## 3. Activate LabVIEW

After the installation is complete, you'll need to activate LabVIEW:

* **Start LabVIEW:** Launch the LabVIEW application.

* **Initiate Activation:**
    * You'll likely be prompted to activate LabVIEW upon the first launch. If not, there should be an option in the "Help" menu to activate the software.
    * Select the option to "Check my account for licenses."

    ![LabVIEW Activation](images/Labview_License.png)

* **Activate:** Click the "Activate" button to proceed.

* **Log In:** You will be prompted to log in using your National Instruments account credentials. Ensure you use the same account associated with your LabVIEW license (or the Community Edition).

{{< alert context="info" text="It's common that not every single component installed will require a separate license. You might receive notifications about unlicensed components, but these can often be ignored if the core LabVIEW functionality is licensed."/>}}

