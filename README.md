! It is not possible to upgrade to PocketVJ 3.0 !
# PocketVJ Control Panel 2.0

http://www.pocketvj.com

This file is used to control the PocketVJ over the webbrowser.

Clone everything into the `/var/www/` directory.

This file is only useful if you use the omxplayer-sync https://github.com/turingmachine/omxplayer-sync script.
Read turingmachines installation instructions and get the custom build of omxplayer.

##Instruction

Add www-data to your sudoers list with: `visudo` add this line at the end: `www-data ALL=(ALL) NOPASSWD: ALL`

Allow php with: `sudo lighty-enable-mod fastcgi-php`

The videofiles have to be stored in `/media/internal/video`
The imagefiles have to be stored in `/media/internal/images`

We recommend to use your RPi as a Hotspot, setup as described here: http://elinux.org/RPI-Wireless-Hotspot

###To do list:
https://github.com/magdesign/PocketVJ-CP-v2/blob/master/roadmap.txt


###Dependencies to install:

apt-get -y install lxde-core lxterminal lxappearance xinit lightdm ntfs-3g python-pexpect vim figlet git-core firmware-ralink hostapd isc-dhcp-server lighttpd samba samba-common-bin php5-common php5-cgi php5 php5-mysql screen fbi ttf-mscorefonts-installer mediainfo gparted php5-cli iptables xtightvncviewer imagemagick dosfstools exfat-utils exfat-fuse hfsplus hfsprogs hfsutils xdotool expect expect-dev avahi-daemon libavahi-compat-libdnssd-dev feh libjpeg8 libjpeg8-dev libao-dev avahi-utils libavahi-compat-libdnssd-dev libva-dev youtube-dl python-smbus mpg321 mpg123 libreoffice-impress rc-gui python-pip iceweasel python-dbus xpdf x11-xserver-utils libncurses5-dev

pip install pjlink

pip install python-osc

...


If you want to use PiMapper you must install openframeworks v0.8.4: http://forum.openframeworks.cc/t/raspberry-pi-2-setup-guide/18690
and then install and compile PiMapper https://github.com/kr15h/ofxPiMapper, then you have to simulate a fake keyboard to unleash the remote control, see here: 
http://www.fsays.eu/Blogging/Blog/Details/23

...

If you want to use TCPSClient, download it here: http://techlife.sg/TCPSClient/index.html
put it to `/usr/bin` and make `chmod u+x TCPSClient.bin`
Read the copyrights on their websites and make a donation!

...

For using the snapshot function:
git-clone https://github.com/info-beamer/tools.git
Go into tools/screenshot/ and type make
then move the screenshot folder to /opt/

...

For using the airplay function, install rplay as described here:
http://www.instructables.com/id/AirPlay-Mirroring-without-Apple-TV-using-RPi/?ALLSTEPS)
(Airplay support will be removed in future version, since the protocol is no supported anymore on newer devices, if someone knows a solution, please post)

...

For using raspberry cast (https://github.com/vincent-lwt/RaspberryCast):
wget https://raw.githubusercontent.com/vincent-lwt/RaspberryCast/master/setup.sh && sudo sh setup.sh

(Raspberry cast will be removed in future versions...)

...


Sync Script and Omxplayer fork written by: Simon Josi, http://www.yokto.net

Pi-Mapper written by: Krisjanis Rijnieks, https://github.com/kr15h/

Virtual Keyboard written by: Erwin van Dijk, http://www.fsays.eu/

TCPSyphon written by: Nozomu Miura, http://techlife.sg/

Clock written by: xorg62, https://github.com/xorg62/tty-clock

Projector Power Script by: Marco Schmalz

Testmovie by: Manuel Berner, http://towerbus.ch/

Testaudio by: Marcel Bieri, https://facebook.com/casashowband

Idea, support and concept by: Marc-André Gasser, http://magdesign.ch/


Copyright by http://magdesign.ch

Please support this project! http://www.pocketvj.com
