# APPENDIX H: QNX IMAGE RE-FLASHING

If SATADOM is corrupted, try the steps given in [trouble shooting section](6.-troubleshooting/) to recover the QNX OS.

If the QNX OS could not recover, follow this section to re-flash the QNX image. The following files are present in DVD which received along with Aries SDK kit

**Files required**

* QNX BSP files

ARS\_QNX7.0\_32-Bit\_32GB folder with following files

![](../../../.gitbook/assets/49.png)

* clonezilla-live-2.5.0-25-i686– CloneZilla OS
* tuxboot-0.8.3.exe – To make a pen drive CloneZilla OS bootable

**Setup Requirements**

* SATADOM of 16GB – Target media
* Two 8 GB pen drives
* First 8 GB pen drive – To have ARS\_QNX7.0\_32-Bit\_32GB folder
* Second 8 GB pen drive – To have CloneZilla OS bootable
* A development PC with windows 7 OS – To make a pen drive as CloneZilla OS bootable

**Make an 8 GB pen drive as CloneZilla OS bootable:**

* Connect the 8 GB pen drive to a windows PC
* Run tuxboot-0.8.3.exe and it will show the pen drive in bottom.

![](../../../.gitbook/assets/image%20%2811%29.png)

* Select disk image and browse “clonezilla-live-2.5.0-25-i686” file and click ok.

![](../../../.gitbook/assets/image%20%2831%29.png)

* It will start copying files as follows

![](../../../.gitbook/assets/image%20%2852%29.png)

* Finally it will show the following screen, click exit and now the pen drive is CloneZilla OS bootable

![](../../../.gitbook/assets/image%20%2829%29.png)

**Store QNX BSP image to new/corrupted SATADOM using CloneZilla OS**

* Copy ARS\_QNX7.0\_32-Bit\_32GB folder to a pen drive
* Connect SATADOM to Aries board
* Connect CloneZilla bootable pen drive to Aries board
* Connect pen drive which has ARS\_QNX7.0\_32-Bit\_32GB folder to Aries board
* Power on the board and boot to BIOS setup \(by continuously pressing DEL key during boot up\)
* Go to Boot-&gt;Hard disk priorities then choose CloneZilla pen drive as first boot device
* Press F4 and save.
* It will boot to CloneZilla OS as follows and select first option and press enter

![](../../../.gitbook/assets/55.jpeg)

* Choose language

![](../../../.gitbook/assets/56.jpeg)

* The default keyboard layout is US keyboard, therefore if you are using US keyboard, just press enter \(i.e. use the option "Don't touch keymap"\)

![](../../../.gitbook/assets/57.png)

* Select following option

![](../../../.gitbook/assets/58%20%281%29.png)

* Attach pen drive which is having Aries QNX 32 bit image. Select following option

![](../../../.gitbook/assets/59.jpeg)

* Select following option

![](../../../.gitbook/assets/60.jpeg)

* Press Enter to continue

![](../../../.gitbook/assets/61.jpeg)

* Wait until the pen drive which has ARS\_QNX7.0\_32-Bit\_32GB\_BSP\_Image folder is detected, once it detects then press “Ctrl+C”. \(Remove ARS\_QNX7.0\_32-Bit\_32GB\_BSP folder contained pen drive and note pen drive name for reference.\)

![](../../../.gitbook/assets/62.jpeg)

* Select the pen drive which has ARS\_QNX7.0\_32-Bit\_32GB\_BSP Image folder, the following is an example, so Choose the pen drive correctly

![](../../../.gitbook/assets/63%20%281%29.jpeg)

* Select “ARS\_QNX7.0\_32-Bit\_32GB\_BSP\_IMAGE” option and click onto “Done” using “Tab” button.

![](../../../.gitbook/assets/64.jpeg)

* Press enter to continue for next step.

![](../../../.gitbook/assets/65.jpeg)

* Select following option.

![](../../../.gitbook/assets/66.png)

* Select following option

![](../../../.gitbook/assets/67.png)

* Select following option

![](../../../.gitbook/assets/68.jpeg)

* Select the SATADOM to restore/copy the QNX 32-bit BSP image

![](../../../.gitbook/assets/69.jpeg)

* Select following option.

![](../../../.gitbook/assets/70%20%281%29.jpeg)

* Select following option.

![](../../../.gitbook/assets/71%20%281%29.jpeg)

* Press Enter to continue

![](../../../.gitbook/assets/72.jpeg)

* Type “y” to continue.

![](../../../.gitbook/assets/73%20%281%29.jpeg)

* Then it will start copying the image to SATADOM.

![](../../../.gitbook/assets/74%20%281%29.jpeg)

![](../../../.gitbook/assets/75.png)

* Once Copying is done, press enter to continue.

![](../../../.gitbook/assets/76%20%281%29.jpeg)

* Select Power off.

![](../../../.gitbook/assets/77.png)

* Now the SATADOM is ready to boot to Aries QNX 32 bit.

![](../../../.gitbook/assets/78%20%281%29.jpeg)

