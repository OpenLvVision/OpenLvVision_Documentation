---
title: "Read image file"
description: "convert an Image into an array" 
icon: "save"
draft: false
---

This LabVIEW snippet demonstrates a fundamental image loading and display sequence using OpenLvVision functions.

1.  **Create Image Reference:** 
    * The "OLVCreate" function (1) initializes a new, empty image reference.
    * In LabVIEW, image data is handled by references, meaning the wire carries a pointer to the image data's location in memory, not the image data itself.
    * This is a crucial distinction, as image references do not adhere to LabVIEW's standard dataflow paradigm where data is copied between functions.

2.  **Read Image File:** 
    * The "OLVReadFile" function (2) loads an image from the specified file path.
    * When the "UseFilePartImageType" input is set to TRUE (as indicated by the constant), the appropriate image file format reader is automatically selected, simplifying the loading process.

3.  **Draw Image to Control:**
    * Draws the image onto a control.
    * Note: If the control is configured for snapshots, it will retain a copy of the image; otherwise, the image will be lost after disposal.

4.  **Dispose Image:** 
    * Finally, the "OLVDispose" function (5) releases the memory allocated for the image data referenced by the initial "OLVCreate" function.
    * It is essential to dispose of image references when they are no longer required to prevent memory leaks and ensure efficient memory management within your LabVIEW application.

![ReadImageFile](images/Example_ReadImageFile.png)
