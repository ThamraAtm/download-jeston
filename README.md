# download-jeston

# remove Chromium and OpenCV
$ sudo apt-get remove --purge chromium-browser chromium-browser-l10n
# refresh your system
$ sudo apt-get update
# need nano for editing some files
$ sudo apt-get install nano
$ sudo apt-get upgrade
$ sudo apt-get autoremove

$ sudo nano /etc/update-manager/release-upgrades

# refresh your system again
$ sudo apt-get update
$ sudo apt-get dist-upgrade
$ sudo reboot

# upgrade to Ubuntu 20.04
$ sudo do-release-upgrade

# check and editing some files
$ sudo nano /etc/gdm3/custom.conf
$ sudo nano /etc/X11/xorg.conf
$ sudo nano /etc/update-manager/release-upgrades
$ sudo reboot

# remove icd.d
$ sudo rm -rf /usr/share/vulkan/icd.d

# prepare your system
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get autoremove
# remove circular symlink
$ sudo rm /usr/share/applications/vpi1_demos
# remove distorted nvidia logo in top bar
$ cd /usr/share/nvpmodel_indicator
$ sudo mv nv_logo.svg no_logo.svg

# install gcc and g++ version 8
$ sudo apt-get install gcc-8 g++-8
# setup the gcc selector
$ sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-9 9
$ sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-8 8
# setup the g++ selector
$ sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-9 9
$ sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-8 8
# if you want to make a selection use these commands
$ sudo update-alternatives --config gcc
$ sudo update-alternatives --config g++
