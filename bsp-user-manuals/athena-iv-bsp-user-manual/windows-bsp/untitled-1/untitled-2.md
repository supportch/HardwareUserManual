# 7.3 APPENDIX C: STEPS TO CREATE WINPE BOOTABLE USB DRIVE

Create a bootable pen drive by following Steps in **Appendix A**. Next, Open a deployment tool with administrator privilege in the Windows 10 development System and use the following commands:

* On your development computer, click **Start**, point to **All Programs**, point to **Windows AIK,** right- click **Deployment Tools** **Command Prompt**, and then select **Run as administrator.**
* Create a working copy of the Windows PE files. Specify either x86 or amd64:

        **copype amd64 C:\WinPE\_amd64**

* Install Windows PE to the USB flash drive, specifying the drive letter:

        **MakeWinPEMedia /UFD C:\WinPE\_amd64 F:**



