# Hubic Linux Configuration

Version used: Linux 2.1.0.53 (deb package)

Sources:

* https://forums.hubic.com/showthread.php?272-hubiC-for-Linux-beta-is-out-!
* http://doc.ubuntu-fr.org/hubic
* http://mir7.ovh.net/ovh-applications/hubic/hubiC-Linux/2.1.0/


## Download & install the package

    $ wget http://mir7.ovh.net/ovh-applications/hubic/hubiC-Linux/2.1.0/hubiC-Linux-2.1.0.53-linux.deb
    $ sudo dpkg -i hubiC*.deb
    $ sudo apt-get install -f

## Export DBUS session information

    $ export DBUS_SESSION_BUS_ADDRESS=`dbus-daemon --session --fork --print-address`

## Configure Hubic Linux

Login:

    $ hubic login email@address.com ~/hubic

Exclude a folder:

    $ hubic exclude add ~/hubic/Documents

List excludes:

    $ hubic exclude list

Remove an exclude:

    $ hubic exclude remove /home/pi/hubic/Videos
