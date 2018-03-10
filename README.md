Requirements:
-------------------------
Generic:
* Bitcoin >=0.11.1
* Python >=2.6
* Twisted >=10.0.0

Linux:
* sudo apt-get install python-rrdtool python-pygame python-scipy python-twisted python-twisted-web python-imaging

Windows:
* Install Python 2.7: http://www.python.org/getit/
* Install Twisted: http://twistedmatrix.com/trac/wiki/Downloads
* Install Zope.Interface: http://pypi.python.org/pypi/zope.interface/3.8.0
* Install python win32 api: http://sourceforge.net/projects/pywin32/files/pywin32/Build%20218/
* Install python win32 api wmi wrapper: https://pypi.python.org/pypi/WMI/#downloads
* Unzip the files into C:\Python27\Lib\site-packages

Running P2Pool:
-------------------------
To use P2Pool, you must be running your own local bitcoind. For standard
configurations, using P2Pool should be as simple as:

    cd lyra2re-hash-python
    git submodule init
    git submodule update
    sudo python setup.py install
    cd ../
    python run_p2pool.py --net vertcoin

Then run your miner program, connecting to 127.0.0.1 on port 9171 with any
username and password.

If you are behind a NAT, you should enable TCP port forwarding on your
router. Forward port 9346 to the host running P2Pool.

Run for additional options.

    python run_p2pool.py --help

Official wiki:
-------------------------
https://en.bitcoin.it/wiki/P2Pool

Alternate web frontend:
-------------------------
* https://github.com/hardcpp/P2PoolExtendedFrontEnd


