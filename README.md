# kali-boot_trouble
informative if your kali OS is stuck in boot trouble, on update / upgrade.


#if your kali OS is not booting and stuck blank screen for a long while, here you can find helpful.
#get into the recovery mode(advanced setup) at bootloader


;enter your root password at password prompt
#you may need to connect to the internet via wlan0 or usb0 for the next to steps on force recovery else skip it apart
#steps you may find helpful to connect to internet are given at label "connectivity instruction."


;apt-get dist-upgrade
;apt-get autoremove
#if no access to the internet, just try the only command below


;dpkg --configure -a
;systemctl reboot



"connectivity instructions......"
;ifconfig wlan0 up
;iwlist scan
#note down the essid after scan


;iwconfig wlan0 essid <essid-name> key <password>
#by now it would have connected to the internet.
