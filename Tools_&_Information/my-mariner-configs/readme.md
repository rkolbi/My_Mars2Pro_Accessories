## Installing mariner + Samba

**Example configuration files can be found [here](https://github.com/rkolbi/My_Mars2Pro_Accessories/tree/main/Tools_&_Information/my-mariner-configs). Mariner GitHub [here](https://github.com/luizribeiro/mariner), author's step-by-step [here](https://l9o.dev/posts/controlling-an-elegoo-mars-pro-remotely/)**.



-Download the latest version of [Raspberry Pi Imager](https://www.raspberrypi.org/downloads/) and install it.

-Connect an SD card reader with the SD card inside.

-Open Raspberry Pi Imager, select CHOOSE OS ->  Raspberry Pi OS (other) -> Raspberry Pi Os Lite.

-Choose your sd-card with CHOOSE SD CARD, then select write.

-Once completed, you should see the contents of the freshly written sd-card.

-Place <u>ssh</u> (this is supposed to be an empty file) & <u>wpa_supplicant.conf</u> files in the sd-card's root directory and then safely eject from OS.

-Insert the sd-card into the rPi and then apply power to the rPi.

-Download and install [Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html). Run the Putty Application. Enter `raspberrypi.local` as the address you wish to connect to in Putty. Click OK/Yes if you get a security warning. When prompted on a black terminal window, enter `pi` as your username and `raspberry` as your password.

$`sudo raspi-config`: system options -> Password (enter a new password), system options -> hostname (enter you printers nick-name), advanced options -> expand filesystem, Finish -> reboot

-Close Putty, wait a few minutes for rPi to reboot, Open Putty, and use your printer's `nick-name.local` as address to connect to, use pi as username and new password as just changed.

$`sudo apt-get update`

$`sudo apt-get upgrade`

$`sudo nano /boot/config.txt` -> add the following lines to the end of the file:
`dtoverlay=dwc2,dr_mode=peripheral`
`enable_uart=1`
Then ctrl+o, ctrl+x

$`sudo nano /boot/cmdline.txt` -> add `modules-load=dwc2` to the end of the line. Remove `console=serial0,115200`
Then ctrl+o, ctrl+x
Should look like: `console=tty1 root=PARTUUID=BLAHBLAHBLAH rootfstype=ext4 elevator=deadline fsck.repair=yes rootwait modules-load=dwc2`

$`sudo dd bs=1M if=/dev/zero of=/piusb.bin count=4096`
*This can take several minutes

$`sudo mkdosfs /piusb.bin -F 32 -I`

$`sudo mkdir /mnt/usb_share`

$`sudo nano /etc/fstab`

Add the following line to the end of the file:
`/piusb.bin            /mnt/usb_share  vfat    users,umask=000   0       2`
Then ctrl+o, ctrl+x

$`sudo mount -a`

$`sudo nano /etc/rc.local`
Add the following before the `exit 0`
`/bin/sleep 5`
`modprobe g_mass_storage file=/piusb.bin removable=1`
`/sbin/iwconfig wlan0 power off`
Then ctrl+o, ctrl+x

$`sudo reboot`

$`sudo systemctl stop serial-getty@ttyS0`

$`sudo systemctl disable serial-getty@ttyS0`

$`sudo apt-get install samba winbind -y`

$`sudo nano /etc/samba/smb.conf`
Add the following to the end of the file:  
[Elegoo]  
   comment = Saturn  
   path = /mnt/usb_share/  
   browseable = Yes  
   writeable = Yes  
   only guest = no  
   create mask = 0777  
   directory mask = 0777  
   public = yes  
   read only = no  
   force user = root  
   force group = root  
  
Then ctrl+o, ctrl+x  

$`wget https://github.com/luizribeiro/mariner/releases/download/v0.1.1-1/mariner3d_0.1.1-1_armhf.deb`

$`sudo apt install ./mariner3d_0.1.1-1_armhf.deb`

$`sudo reboot`

-Once rebooted, open windows file explore and type your printer's nick-name as \\nick-name\
You should now see the USB_Share folder. Right click this and map network drive.



If everything is good, you should be able to access it by opening http://PRINTER_NICKNAME:5000/ on your browser.
