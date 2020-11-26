# 7.6 APPENDIX F: WINDOWS 10 IMAGE RE-FLASHING

If M.2 2230 SATA is corrupted, try the steps given in troubleshooting section to recover the Windows 10 OS. 

If the Windows 10 OS could not recover, follow this section to re-flash the Windows 10 image. The following files are present in DVD which received along with Athena-IV SDK kit.

**Files required** 

* Windows 10 64bit BSP files

        ****ATHENA-IV\_Windows10\_64bit\_BSP\_32GB\_Image folder with following files

![](../../../../.gitbook/assets/image%20%2819%29.png)

* clonezilla-live--2.5.0-25-i586.iso – CloneZilla OS 
* tuxboot-0.8.3.exe – To make a pen drive CloneZilla OS bootable 

**Setup Requirements**

* M.2 2230 SATA of 32GB – Target media 
* Two 8 GB pen drives 
* First 8 GB pen drive – To have the ATHENA-IV\_Windows10\_64bit\_BSP\_32GB\_Image folder 
* Second 8 GB pen drive – To have CloneZilla OS bootable 
* A development PC with windows 7 OS – To make a pen drive as CloneZilla OS bootable 

**Make an 8 GB pen drive as CloneZilla OS bootable:**

* Connect the 8 GB pen drive to a windows PC  
* Run tuxboot-0.8.3.exe and it will show the pen drive in the bottom.

![](../../../../.gitbook/assets/image%20%2867%29.png)

* Select disk image and browse “clonezilla-live-2.5.0-25-i586.iso” file and click ok. 

![](../../../../.gitbook/assets/image%20%2827%29.png)

* It will start copying files as follows 

![](../../../../.gitbook/assets/image%20%288%29.png)

* Finally, it will show the following  screen, click exit and now the pen drive is CloneZilla OS bootable

![](../../../../.gitbook/assets/image%20%2865%29.png)

**Store Windows 10 BSP image to new/corrupted M.2 2230 SATA using CloneZilla OS**

* Copy ATHENA-IV\_Windows10\_64bit\_BSP\_32GB\_Image folder to a pen drive 
* Connect M.2 2230 SATA to Athena-IV board 
* Connect CloneZilla bootable pen drive to Athena-IV board
* Connect pen drive which has ATHENA-IV\_Windows10\_64bit\_ BSP\_32GB\_Image folder on Athena-IV board
* Power on the board and boot to BIOS setup \(by continuously  pressing DEL key during boot up\)
* Go to  Boot-&gt;Hard disk priorities then choose CloneZilla pen drive as the first  boot device 
* Press F10 and save.
* It will boot to CloneZilla OS as follows and select first option and press enter

![](../../../../.gitbook/assets/image%20%2853%29.png)

* Choose language

![](../../../../.gitbook/assets/image%20%2839%29.png)

* The default keyboard layout is US keyboard, therefore if you are using US keyboard, just press enter \(i.e. use the option "Don't touch keymap"\)

![](../../../../.gitbook/assets/image%20%2848%29.png)

* Select following option 

![](../../../../.gitbook/assets/image%20%2814%29.png)

* Attach pen drive which is having Athena-IV Windows 10 image. Select following option 

![](../../../../.gitbook/assets/image%20%2859%29.png)

* Select following option 

![](../../../../.gitbook/assets/image%20%2821%29.png)

* Press Enter to continue

 

![](../../../../.gitbook/assets/image%20%2837%29.png)

* Wait until the pen drive which has ATHENA-IV\_Windows10\_ 64bit\_BSP\_32GB\_Image folder is detected, once it detects then press “Ctrl+C”. \(Remove ATHENA-IV\_Windows10\_64bit\_ BSP \_32GB folder contained pen drive and note pen drive name for reference.\) 

![](../../../../.gitbook/assets/image%20%2820%29.png)

* Select the pen drive which has ATHENA-IV\_Windows10\_ 64bit\_BSP\_32GB\_Image folder, the following is an example, so Choose the pen drive correctly  

![](../../../../.gitbook/assets/image%20%2810%29.png)

* Select following option 

![](../../../../.gitbook/assets/image%20%2824%29.png)

* Press enter to continue for next step.

![](../../../../.gitbook/assets/image%20%2860%29.png)

* Select following option.

![](../../../../.gitbook/assets/image%20%2815%29.png)

* Select following option.

![](../../../../.gitbook/assets/image%20%2840%29.png)

* Select following option.

![](../../../../.gitbook/assets/image%20%286%29.png)

* Select the SATA to restore/copy the Windows 10 BSP image 

![](../../../../.gitbook/assets/image%20%2842%29.png)

* Select following option

![](../../../../.gitbook/assets/image%20%2833%29.png)

* Select following option 

![](../../../../.gitbook/assets/image%20%2845%29.png)

* Press Enter to continue

![](../../../../.gitbook/assets/image%20%2812%29.png)

* Type “y” to continue.

![](../../../../.gitbook/assets/image%20%2841%29.png)

* Then it will start copying the image to M.2 2230 SATA

![](../../../../.gitbook/assets/image%20%289%29.png)

![](../../../../.gitbook/assets/image%20%2866%29.png)

* Once Copying is done, press enter to continue.

![](../../../../.gitbook/assets/image%20%2838%29.png)

* Select Power off.

![](../../../../.gitbook/assets/image%20%2825%29.png)

* Now the M.2 2230 SATA is ready to boot to Athena-IV Windows 10. 















