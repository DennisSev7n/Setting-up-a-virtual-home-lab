<h1>KALI-LINUX Virtual Box</h1>


<h2>Setting up a Kali-linux OS on your Virtual Machine (using Oracle Virtual Box)</h2>
In this guide, I’ll walk you through downloading and installation of Kali Linux on VirtualBox. It is quite easy. Just follow the following steps and your Kali-Linux OS should be working just fine on your vitual machine.
<h4> Note: </h4> I assume that you already have Oracle Virtual Box downloaded and all set up on your PC

<h2>Step One: Download Kali-Linux ISO </h2>
Click <a href="https://www.kali.org/get-kali/#kali-platforms">here</a>  to download the Kali-Linux ISO. Click on the Installer Images as shown in the image below.

<img src = "Folder/kali 1.png">
After that, select the 'Installer 64 ISO'. It should automatically begin to download.
<img src = "Folder/kali download installer.png">

<h2>Step Two: Create a new virtual machine</h2>
On your Virtual Box, click on <b>'New</b>'.

Next, Name your virtual machine (e.g., "Kali Linux"), choose "Linux" as the Type, and select "Ubuntu (64-bit)" as the Version if using the 64-bit ISO.

<h4>Memory Size</h4>
Allocate a minimum of 4096 MB of memory for your virtual machine; however, 8192 MB (8 GB) or more is recommended for better performance. For the processor, assign at least 4 CPUs if available.

<h4>Virtual Hard Disk</h4>
Allocate at least 20 GB of storage for Kali Linux, though you can choose a larger size if you have sufficient disk space.

<h4>VM Settings</h4>
Choose your virtual machine and click "Settings". Navigate to the "Storage" section, then click the empty CD icon under "Controller: IDE". Next, select "Choose a disk file..." and locate the Kali Linux ISO file you previously downloaded. This process attaches the ISO to your virtual machine for installation.

<h4>VM Network Settings </h4>
Make sure your network settings are properly configured. It is recommended to use the Bridged Adapter setting, which allows your virtual machine to function as a separate device on your physical network.

The VM will receive its own unique IP address either dynamically from the network’s DHCP server or through manual static configuration. This setup enables the virtual machine to interact seamlessly with other devices on your network, just like a physical computer. The Bridged Adapter option ensures better connectivity and access to network resources, making it ideal for scenarios that require full network integration for testing or communication purposes.


<h2>Step Three: Start up your new virtual machine</h2>
Click <b>"Start"</b> to boot the VM. Once booted, log in using the default credentials:
Username: kali
Password: kali

<h2>Step Four: Updating your Kali OS</h2>
Launch a terminal and execute the command:
sudo apt update

This ensures your system's package list is updated with the latest repositories.

-----
Once the update is complete, run the command:
sudo apt upgrade -y

This upgrades your Linux system to the latest available packages and enhancements.
-
