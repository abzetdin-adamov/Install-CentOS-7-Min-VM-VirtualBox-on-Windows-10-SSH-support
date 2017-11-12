# Installing a CentOS 7 Minimal VM with VirtualBox on Windows 10 with SSH support

**1. Restart your computer enter to BIOS** 
Depending on your BIOS software, go to Advanced Settings, look for Virtualization (Technology VT), make sure that it's Enabled.

**2. Download and install binary installer appropriate for your platform from**
https://www.virtualbox.org/wiki/Downloads
VBoxManage --version

**3. Downlaod popular SSH client PuTTY.exe from www.putty.org (do not need installation)**

**4. Download to your computer Centos Minimal .ISO image at**
https://site.ada.edu.az/~aadamov/sources/downloads/ 
or http://isoredirect.centos.org/centos/7/isos/x86_64/CentOS-7-x86_64-Minimal-1708.iso 

**5. Run VirtualBox and create new Virtual Machine (VMs)**
Specify Name, type (Linux), version (Red Hat 64) and follow to default paramenters

**6. To assign Centos Image to newly created VM**
- right click on VM 
- select Settings
- select Storage tab
- select Empty under Controller: IDE
- on right side in Attributes click to small disc icon on the right of Optical Drive
- browse and select Centos .ISO Image file

**7. To allow host computer and other computers in the same network to access VM**
    - right click on VM 
    - select Settings
    - select Network tab (Adapter one already assigned to NAT to enamble VM access to host computer's network and Internet)
    - select Adapter 2 
    - check Enable Network Adapter
    - select Bridged Adapter

**8. Select VM and click to Start button to start Centos installation**
    - specify root password and create user (login/password)
    - when installation completed enter to system using login/password

**9. To learn dynamic IP address assigned by DHCP type command "ip addr"**

**10. Run PuTTY**
    - enter IP addres to Host Name (IP address) and click Open button
    - you should be asked to enter login/password

**Congratulation! You've done!**
