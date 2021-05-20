# Installing the Prisma VPN on Linux
This is a short how-to for people on Linux at the University of Nebraska Omaha to install the Prisma VPN.

# Method 1: Script Install
Download the script from https://github.com/UNO-IST-Support/installPrismaVPNLinux-UNO/blob/main/installVPN.sh
<br/>
You may need to copy paste it into a .sh file.
<br/>
Once the file has downloaded/been created, run the script: ./installVPN.sh
Note: You may need to run chmod +x to make it executable.
<br/>
This should install the dependencies and the VPN. This will also give you the command to launch the UI after it is installed.
<br/>
<br/>
# Method 2: Manual Install
Run this command: wget https://github.com/UNO-IST-Support/installPrismaVPNLinux-UNO/raw/main/GlobalProtect_UI_deb-5.2.6.0-18.deb
<br/>
Run the next command: sudo apt-get install -y libqt5webkit5
<br/>
Once that finishes, run the last command: sudo dpkg -i GlobalProtect_UI_deb-5.2.6.0-18.deb
<br/>
This will go through the process of installation and will bring up the connect UI for the first time.
<br/>
After this, you will need to use the following command to open the UI at any other point if you need to disconnect/reconnect. 
<br/>
Command: globalprotect launch-ui
<br/>

If you have any issues, please contact us in the Systems Office.

