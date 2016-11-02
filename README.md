OpenNet
=======
A simulator for Software-Defined Wireless Local Area Network and Software-Defined LTE Backhaul Netowrk  
http://www.slideshare.net/rascov/20140824-open-net  

Feature
-------
* Built on top of Mininet and ns-3
* Complement ns-3 by supporting channel scan behavior on Wi-Fi station (sta-wifi-scan.patch)
* Show CsmaLink and SimpleLink in NetAnim (animation-interface.patch)
* Fix runtime error when access PacketMetadata of CsmaLink, [Submitted](https://www.nsnam.org/bugzilla/show_bug.cgi?id=1787)
* Support SDN-based LTE backhaul emulation

Build OpenNet
-------------
Support Ubuntu 14.04.5

    $ sudo su -
    # apt-get install git ssh
    # git clone https://github.com/dlinknctu/OpenNet.git
    # cd OpenNet
    # ./configure.sh
    # ./install.sh master

After a successful installation, the script will show "OpenNet installation has completed."  

Run OpenNet example script
--------------------------

    $ sudo su -
    # cd OpenNet
    # python mininet/examples/opennet/wifi/two-ap-one-sw.py

Run NetAnim
-----------
Use NetAnim to open the XML file in the directory /tmp/xml  
Click "Play Animation" button can start animation of network activity  

    $ sudo su -
    # cd OpenNet
    # python mininet/examples/opennet/wifi/wifi-roaming.py
    # ./ns-allinone-3.22/netanim-3.105/NetAnim

Reference
---------
* Link modeling using ns-3, [Link](https://github.com/mininet/mininet/wiki/Link-modeling-using-ns-3 "Link modeling using ns-3")

