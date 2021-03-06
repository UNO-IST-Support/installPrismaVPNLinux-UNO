# Installing the Prisma VPN on Linux
This is a short how-to for people on Linux at the University of Nebraska Omaha to install the Prisma VPN.
<br/>
The address for the VPN is now: nu-vpn.nebraska.edu

# Method 1: Script Install
Download the script from https://github.com/UNO-IST-Support/installPrismaVPNLinux-UNO/blob/main/installVPN.sh
<br/>
`wget https://raw.githubusercontent.com/UNO-IST-Support/installPrismaVPNLinux-UNO/main/installVPN.sh`
<br/>
You may need to copy paste it into a .sh file.
<br/>
Once the file has downloaded/been created, run the script: `./installVPN.sh`
<br/>
Note: You may need to run chmod +x to make it executable.
<br/>
This should install the dependencies and the VPN. This will also give you the command to launch the UI after it is installed.
<br/>
If you get an error stating it cannot connect to the GDP process after installation, a quick reboot usually does the trick. Try this after pretty much any error you may receive. 
<br/>
<br/>
# Method 2: Manual Install
Run this command:
<br/>
`wget https://github.com/UNO-IST-Support/installPrismaVPNLinux-UNO/raw/main/GlobalProtect_UI_deb-5.2.6.0-18.deb`
<br/>
Run the next command: `sudo apt-get install -y libqt5webkit5`
<br/>
Once that finishes, run the last command: `sudo dpkg -i GlobalProtect_UI_deb-5.2.6.0-18.deb`
<br/>
This will go through the process of installation and will bring up the connect UI for the first time.
<br/>
If you get an error stating it cannot connect to the GDP process after installation, a quick reboot usually does the trick. Try this after pretty much any error you may receive. 
<br/>
After this, you will need to use the following command to open the UI at any other point if you need to disconnect/reconnect. 
<br/>
Command: `globalprotect launch-ui`
<br/>
<br/>
## If you need to uninstall this software, please run the following highlighted command: `sudo dpkg -P GlobalProtect`

If you have any issues, please contact us in the Systems Office.

