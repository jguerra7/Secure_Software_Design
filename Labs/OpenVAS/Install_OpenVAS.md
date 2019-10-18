# Install OpenVAS
In order to be able to complete this section, you will need this:

Console access to your Kali Linux system
Internet access to download and install OpenVAS application

## How to do it...
We will perform the steps necessary to install OpenVAS on Kali:

* If you have not fully updated your Kali Linux installation, you will want to do so now. From the root shell, run the following command. If there are many updates, this may take a while, but be patient. Once the update process is complete, reboot the system, login, and open a root shell again:
```
apt-get update && apt-get dist-upgrade -y
```
From the root shell, use apt-get to download and install OpenVAS: 
```
apt-get install openvas
```
* Once the installation is complete, run the following from the root shell to kick off the setup process. Due to the amount of data needed, it is likely this will take a while even over a fast connection, so be prepared to wait:
```
openvas-setup
```
At the end of this process, you will see the admin password displayed. Write this down so that you are able to log into the OpenVAS portal.
In the event where you forget this password, it can be reset from the command line using the following:
```
openvasmd --user=admin --new-password=[your password here]
```
