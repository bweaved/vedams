Installing custom WebIOPi on Raspberry Pi Running Weaved service :
==================================================================
#Pre-Requisite:
#Install Weaved service along with Push notification support for Raspberry-Pi from Weaved Portal.  

#This Weaved custom WebIOPI service assumes Weaved service is configured to listen on Port 8000. If not,
#update /etc/webiopi/config to reflect the port number corresponding to match weaved service port OR follow
#instructions on how to get the Weaved service configured to listen on webiopi default port setting of 8000.

#To Install:

$ tar xvzf WeavedBerryClipWebIOPi-0.7.0.tar.gz
$ cd WebIOPi-0.7.0
$ sudo ./setup.sh

#Running WebIOPi (Daemon), start/stop the background service as below:

$ sudo /etc/init.d/webiopi start
#$ sudo /etc/init.d/webiopi stop

#Auto start at boot, To setup your system to start webiopi at boot :

$ sudo update-rc.d webiopi defaults

#To remove webiopi start from boot :
#$ sudo update-rc.d webiopi remove
