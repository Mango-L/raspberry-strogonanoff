Raspberry Strogonanoff
======================

A Raspberry Pi Remote Mains Switcher, to switch these

http://www.maplin.co.uk/remote-controlled-mains-sockets-5-pack-348217

with one of these

http://proto-pic.co.uk/434mhz-rf-link-transmitter/

using the awesome reverse engineering detailed here

http://www.fanjita.org/serendipity/archives/53-Interfacing-with-radio-controlled-mains-sockets-part-2.html

Installation
------------

Requires WiringPi-Python

    git clone https://github.com/WiringPi/WiringPi-Python.git
    cd WiringPi-Python/
    git submodule update --init
    sudo apt-get install python2.7-dev
    sudo apt-get install python-setuptools
    sudo python setup.py install

Running
-------

Needs to be run as root - 

    sudo python strogonanoff_sender.py --channel 1 --button 3 --gpio 8 on 
    
where the GPIO pin numbers are the big ones on this diagram ![](http://pi4j.com/images/p1header-large.png)
