---
title: "Image to Array"
description: "Copies an Image into an array" 
icon: "data_array"
draft: false
---

This LabVIEW example copies form an image the selected pixel data into an array.

1.  **Create Image Reference:**

    * The "OLVCreate" function (1) initializes a new, empty image reference.
    * In LabVIEW, image data is handled by references, meaning the wire carries a pointer to the image data's location in memory, not the image data itself.
    * This is a crucial distinction, as image references do not adhere to LabVIEW's standard dataflow paradigm where data is copied between functions.

2.  **Read Image File:**

    * The "OLVReadFile" function (2) loads an image from the specified file path (`CandCan 00.png`).
    * When the "UseFilePartImageType" input is set to TRUE (as indicated by the constant), the appropriate image file format reader is automatically selected, simplifying the loading process.

3.  **Get Last Event (Image Control):**

    * The "GetLastEvent Methode" (3) retrieves information about the most recent user interaction with the "Image" control.
    * In this context, it is likely configured to trigger when a "Mouse Up" event occurs.
    * This event signifies that the user has completed drawing a region of interest (ROI) on the displayed image.

4.  **Extract ROI as Array:**

    * Within the "Image: Mouse Up" event structure, the "OLVImageToArray" function (4) extracts the pixel data contained within the user-defined ROI.
    * The "Pixel" output provides the image data within the ROI as an array, enabling further analysis or processing.

5.  **Dispose Image:**

    * Finally, the "OLVDispose" function (5) releases the memory allocated for the image data referenced by the initial "OLVCreate" function.
    * It is essential to dispose of image references when they are no longer required to prevent memory leaks and ensure efficient memory management within your LabVIEW application.

![ImageToArray](images/Example_ImageToArray.png)
