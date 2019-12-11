![JRL Logo](http://jimmyloforti.com/_common/images/jrl_logo2.png)

## Application Name: KaliLinux_Install ##

* Description: Step-by-step instructions on how to install the Kali Linux distribution via flash drive.

### Required Hardware ###

* Flash Drive - > 2GB
* PC to install Kali Linux operating system.

-----------------------------------------------------------------------------------------------

### Step-by-step ###

#### Getting the Software ####

* Doanload and install the Kali Linux distrobution [here](https://www.kali.org/downloads/)
* Download the Universal USB Installer [here](https://www.pendrivelinux.com/universal-usb-installer-easy-as-1-2-3/)
* Add the OS to the pendrive.

#### Installing the OS ####

* Plugin the flash drive.
* Make sure power and an ethernet or WiFi is available.
* Turn on the PC.
* Once the manufacturer logo appears, continously press F12 (or your OEM's boot option key) to access the boot menu.
* From the boot options, select "USB Storage Device".

* Once the Kali Linux installer menu appears, select "Install".
* STOP!  Before proceeding with the next step of the installer (language selection), you need to manually mount the cd-rom.
  * Press 'alt + F2' to open a console.  Press enter when prompted.
  * In the console, execute the following commands:
    * mkdir /cdrom
    * mount -t vfat /dev/sdb1 /cdrom
  * Type 'exit' and press enter to exit the console.
  * Press 'alt + F1' to switch back to the kali linux installer.
  
* Proceed with the installation.
* Select language, keyboard, etc.
* When you get to the network setup step, select the wireless network adapter.
* Next, select your router's SSiD, select WPA/WPA2 PSK for encryption, and enter the router's password.
* Leave the hostname as 'kali'.
* When prompted for a domain name, leave it blank and select 'continue'.
* Setup the root password. Enter it again to confirm.

* Partioning: (select the following options)
  * 'Guided - use full partition'
  * 'All files in one partition'
  * 'Finish partitioning and write changes to disk'
  * When prompted to write the changes to disk, select 'Yes'.
  
* GRUB Boot Loader:
 * Check partitions using 'fdisk -l'
  
  

