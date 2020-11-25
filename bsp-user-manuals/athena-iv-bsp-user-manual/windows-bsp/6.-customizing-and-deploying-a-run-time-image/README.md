# 6.	CUSTOMIZING AND DEPLOYING A RUN-TIME IMAGE

       ****[**6.1 TO ADD DRIVER TO AN OFFLINE IMAGE BY USING DISM TOOL** ](6.1-to-add-driver-to-an-offline-image-by-using-dism-tool.md)\*\*\*\*

       ****[**6.2 TO REMOVE DRIVER FROM AND OFFLINE IMAGE BY USING DISM TOOL** ](6.2-to-remove-driver-from-and-offline-image-by-using-dism-tool.md)\*\*\*\*

        ****[**6.3 TO FIND AVAILABLE WINDOWS FEATURE IN IMAGE** ](6.3-to-find-available-windows-feature-in-image.md)\*\*\*\*

        ****[**6.4 TO ENABLE WINDOWS FEATURE** ](6.4-to-enable-windows-feature.md)\*\*\*\*

        ****[**6.5 TO DISABLE WINDOWS FEATURE**](6.5-to-disable-windows-feature.md) ****

        ****[**6.6 CREATING A USB INSTALLATION MEDIA** ](6.6-creating-a-usb-installation-media.md)\*\*\*\*

      ****[  **6.7 EXTRACTING WIM FILE**](6.7-extracting-wim-file.md) ****

       ****[ **6.8 FLASHING WINDOWS 10 BSP IMAGE** ](6.8-flashing-windows-10-bsp-image.md)\*\*\*\*

        ****[**6.9 USING THE FINAL IMAGE**](6.9-using-the-final-image.md) ****

        ****[**6.10 BOOTING TO WINDOWS WELCOME MODE.** ](6.10-booting-to-windows-welcome-mode..md)\*\*\*\*

#### 6. CUSTOMIZING AND DEPLOYING A RUN-TIME

* To customize the Windows 10 image, follow the instructions below. Download Windows Assessment and Deployment Kit for Windows 10 version 1809 LTSC and install in the development machine.
* At an elevated command prompt, locate the Windows Assessment and Deployment Kit \(Windows ADK\) servicing folder, and type the following command to retrieve the name or index number for the image that you want to modify. For example, create a folder as test in C directory. Inside test folder, create a folder as images and put the install.wim.

           **Dism /Get-ImageInfo /ImageFile:C:\test\images\install.wim**

* Take the install.wim from the source folder of Windows 10 bootable image.

![](../../../../.gitbook/assets/image%20%2851%29.png)

* Download Windows Assessment and Deployment Kit for Windows 10 version 1809 LTSC from the below mentioned path.

        [https://docs.microsoft.com/en-us/windows-hardware/get-   started/adk-install](https://docs.microsoft.com/en-us/windows-hardware/get-started/adk-install)





