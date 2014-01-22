Arch-WiPi
=========

Turn your Raspberry Pi into a wireless router/AP. Arch-WiPi is a tiny Arch Linux ARM + create_ap based setup, packaged into a downloadable image.

Arch Linux Raspberry Pi WiFi AP Minimum Requirements

    Raspberry Pi Model B Revision 2.0
    Power adapter with at least 1500 mA (2 amp recommended)
    Fat32 formated 1GB SD Card (2GB Recommended)
    Wifi USB dongle running rtl871xdrv. Eg. Edimax EW-7811Un. (I just ordered and recommend this one)
    Network Cable with Internet access. (eg. Internet cable from your cable modem)

Installation Instructions

    Download my Arch Linux Wireless Raspberry Pi image: archwipi.img.tar.gz (252MB)
    Extract it. eg:  sudo tar zxf archwipi.img.tar.gz
    Write the extracted image to your SD card. eg: sudo dd if=archwipi.img of=/dev/sdb …change sdb if necessary. Don’t run     this command if unsure!!!
    Optional – extend partition to use all of disk. You can use gparted.
    Plug your internet cable and new Arch WiPi SD card into your Raspberry and power it on.
    Everything is automated so after a minute or so scan for a new network SSID: ArchWiPi
    The wifi password password is: 1010101010
    If you need to login to the Pi the credentials are: root | ArchWiPi. (note that there’s a period “.” at the end)
    You can change the WiFi password to what ever you like by editing: /usr/lib/systemd/system/create_ap.service
    Check the CPU clock speed and temperature using ./cpustatus.sh or browse to this address 192.168.12.1:8080/archwipi       (powered by Monitorix) Example from my stats page…
