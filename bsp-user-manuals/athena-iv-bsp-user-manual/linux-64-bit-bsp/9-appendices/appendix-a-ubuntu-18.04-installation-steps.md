# Appendix A: Ubuntu 20.04.1 Installation Steps

The chapter will show the steps to be followed to install Ubuntu 20.04.1 LTS 64-bit operating system.

**Step 1: Boot the board from Live CD**

Boot the board from Live CD , load the Ubuntu 20.04.1 live CD into the CD or DVD drive, and switch on the board with the disc still in the drive and watch the initial BIOS screen for a prompt that indicates which key to use for either:

* a boot menu, or
* the BIOS setup utility

The boot menu option is preferable. If you cannot see such a prompt, on many systems, the required key will be, **F2** or **Delete**. Then change boot priority option to boot from drive.

Select the Install Ubuntu button

![Figure 6: Install Ubuntu](../../../../.gitbook/assets/image%20%28181%29.png)

**Step 2:**

Uncheck Download updates while updating and Install this third party section if it is checked

![Figure 7: Uncheck Download Updates](../../../../.gitbook/assets/image%20%28115%29.png)

**Step 3: Installation type selection**

Select “Something else” option and click continue.

![Figure 8: Installation Type Selection](../../../../.gitbook/assets/image%20%28171%29.png)

**Step 4: Creating new empty partition table**

Click the “New Partition Table” and Click “continue”

![Figure 9: Creating new empty partition table](../../../../.gitbook/assets/image%20%28177%29.png)

Select the “free space” and click the “+” button

![Figure 10: Select Free space](../../../../.gitbook/assets/image%20%28135%29.png)

Select “Ext4 journaling file system” option

Select “ / ” for the Mount point and click Ok

![Figure 11: Select Ext4](../../../../.gitbook/assets/image%20%28175%29.png)

Click Install now

![Figure 12: Click Install Now](../../../../.gitbook/assets/image%20%28180%29.png)

**Step 5: Not selecting a partition for use of Swap space**

To increase life-span of M.2 2230 SATA Flash Disk, it is better to not use swap space because the Linux OS access the swap space frequently. The Athena-IV board has 4GB soldered SDRAM and this is enough for better performance. Hence Click “Continue” to avoid allocating a partition for swap space.

![Figure 13: Installation without Swap Space](../../../../.gitbook/assets/image%20%28143%29.png)

**Step 6: Time Zone Configuration**

Select the country by moving around the World map.

After selecting the country, press continue.

![Figure 14: Time Zone Configuration](../../../../.gitbook/assets/image%20%28154%29.png)

**Step 7: Language Selection**

Select the language and press continue.

![Figure 15: Select Language](../../../../.gitbook/assets/image%20%28189%29.png)

**Step 8: Set the user name.**

Provide the user name and password.

For example user name is dscguest, type the user name in the ‘Your name’ section.

For example password is dscguest, type the password in ‘Choose a password ’section.

The given Your name becomes the user account name for the system and also serves as the administrator.

![Figure 16: User name and password](../../../../.gitbook/assets/image%20%28162%29.png)

**Step 9:**

The following screen will be appeared and it will install the OS.

![Figure 17: Installing System](../../../../.gitbook/assets/image%20%28117%29.png)

**Step 10:**

Restart the system to complete Ubuntu 20.04.1 LTS OS installation once the following window is appeared.

![Figure 18: Restart Now](../../../../.gitbook/assets/image%20%28169%29.png)

\*\*\*\*

