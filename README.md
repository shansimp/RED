# How to connect to RED

source: http://www.thehecklers.org/2015/02/27/how-to-connect-raspberry-pi-to-hidden-ssid/

sudo cp /etc/network/interfaces /etc/network/interfaces.orig 
            (this makes a backup copy of your interfaces file)
sudo nano /etc/network/interfaces

 -----------------------------------------------------------------------------------------
FILE = interfaces file
 -----------------------------------------------------------------------------------------
sudo cp /etc/wpa_supplicant/wpa_supplicant.conf /etc/wpa_supplicant/wpa_supplicant.conf.orig 
            (this makes a backup copy of your wpa_supplicant file)

sudo nano /etc/wpa_supplicant/wpa_supplicant.conf

 -----------------------------------------------------------------------------
FILE = wpa_suplpicant.conf
 -----------------------------------------------------------------------------

sudo reboot

ifconfig -a

If it’s working properly, your wlan0 adapter will show a valid IP address, a number of bytes and packets received and sent (RX and TX), and several other useful bits of information.
Look for the wifi icon in the top right corner of screen
