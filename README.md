# Plug-and-play-multi-OS-manager

This was created as a school project exam from the first year of IT network and security.
It was created with the idea of automatize some of the workload for installing OS on devices. This by using a USB stick that had the 
boot flag an Grub configured on it. With the usage of ISO images that we configured to have answer files predetermend so the install would not
be interupted once started, would only need a selection of what OS desiered do all the work.

The USB where given both Windows and Ubuntu workstation and server ISO to illustrate the option of choise, aswell as a DBAN ISO 
that could be used to strip a device of all previouse data for a cleaner installation.


Once the USB is connected to the device, it will become read at a reboot as long as the device is configured to allow USB boot (this is changed in the bootload setup). From here the Grub panel will appear with the selected ISO that is provided. By choosing any of the choises, Grub will reboot the device aswell as point the bootloader towards the selected ISO, starting the automatical installation.


The only issue that occured was with the Windows pointing from Grub, since we did not propelry specify what driver it should look for.
The driver path is different when comparing to a Linux distro.
