# net_test
![Alt text](./images/spiderweb.png)

Bash script to test network connectivity.

## Description

***net_test*** is a bash script for testing network connectivity on a Linux host.  The script checks both IPv4 and IPv6 localhost and pings the IPv4 and IPv6 Google address for external network checks.  It will also provide routing information.

All of this information is from the local host perspective.  In other words, this script, when ran, specifically checks localhost loop-back and one external IP from the host device it is ran on.  That's it.  It is NOT performing a scan of other devices.

You do not need to run this script with elevated privileges (root).

## Technologies Used

The script within the "**centos**" directory has been tested in the CentOS Stream 9 distribution, in both graphical and multi-user targets (GUI and Server).  The script within the "**ubuntu**" directory has been tested in the Ubuntu 24.04 LTS distribution, also in both graphical and multi-user targets.

The CentOS version of the script should also work with other similar flavors like Red Hat Enterprise Linux (RHEL), Fedora, Oracle, etc.

The Ubuntu version of the script should also work with similar Ubuntu flavors and Debian based distributions like Kali, Kubuntu, Parrot OS, etc.

## How To Download and Use

###### Method 1: Directly from my GitHub Repository

>	If not already in the repository, access it via the link below:
>		https://github.com/Boardleash/net_test/

>	Click on either "**centos**" or "**ubuntu**" (based on whichever OS you are using)

>	Click on the "**network_test**" file and then click on the download raw file option.

>	After the download is complete, go to where you downloaded the file.  The file will likely have been downloaded as a text file (.txt extension).  Rename the file to "**net_test**" (don't inlcude the .txt extension).

>	Right click the file and click on "**Properties**", then click on the "**Permissions**" tab.  Check the "**Allow executing file as program**" box.

>	After doing the above, you can right click on the file and select the "**Run as a program**" option.  The script will open a terminal session and execute.

###### Method 2: Via the Terminal

>	In your terminal, navigate to the directory that you wish to clone the repository into:
>	`cd <DIRECTORY TO CLONE REPO INTO>`

>	In the directory that you have just changed into, type the following:
>	> `git clone https://github.com/Boardleash/net_test/

>	This should successfully clone the entire **harvest** repository into the directory that you have chosen and you are now able to access the contents locally on your terminal

>	Navigate to where the "harvest" script is located.  By default this should be in `/PATH/TO/net_test/centos/` OR `/PATH/TO/net_test/ubuntu/,` but if this script was moved, then navigate to that appropriate directory.

>	Change file permissions for the script by typing the following:
>		*chmod 755 network_test*

>	Run the script by typing the following:
>		*./network_test*

>	The script will proceed.  It may take a minute, but once complete, you will be asked if you have gotten all that you need.  You can respond appropriately.
