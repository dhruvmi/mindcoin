Mindcoin integration/staging tree
================================

http://www.mindinventory.com

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2017-2018 Mindcoin Developers

What is Mindcoin?
----------------

Mindcoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Bitcoin.
 - 20 coins per block
 - 2018 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Mindcoin client sofware, see http://www.mindinventory.com

License
-------

Mindcoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Mindcoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/mindcoin-project/mindcoin/tags) are created
regularly to indicate new official, stable release versions of Mindcoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

				sudo apt-get update
				$sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev
				$sudo apt-get install libboost-all-dev git npm nodejs nodejs-legacy libminiupnpc-dev redis-server

				$sudo apt-get install libdb-dev libqrencode-dev qt4-qmake libqtgui4 libqt4-dev
				$sudo apt-get install libminiupnpc-dev libminiupnpc8 libboost1.48-all-dev


				$sudo apt-get install curl ntp unzip libdb++-dev libboost-all-dev libqrencode-dev aptitude && aptitude install miniupnpc

				$sudo add-apt-repository ppa:bitcoin/bitcoin
				$sudo apt-get update
				$sudo apt-get install libdb4.8-dev libdb4.8++-dev

				$sudo curl https://raw.githubusercontent.com/creationix/nvm/v0.16.1/install.sh | sh
				$source ~/.profile
				$nvm install 0.10.25
				$nvm use 0.10.25

				$git clone https://github.com/malvikiran/mindcoin.git


				$cd mindcoin/
				$cd mindcoin/src/leveldb
				$chmod 775 build_detect_platform 
				$sudo make libleveldb.a libmemenv.a
				$cd ..
				$make -f makefile.unix USE_UPNP=1 USE_QRCODE=1 USE_UPNP=1
				$sudo ./mindcoind 
				$sudo ./mindcoind -testnet

				You will get a message stating there is no configuration file.
				$sudo gedit ~/.mindcoin/mindcoin.conf

				rpcuser=youruser
				rpcpassword=yourpassword
				rpcallowip=*
				rpcport=9332
				daemon=1
				server=1
				gen=0
				addnode= 91.134.120.210
				addnode= 185.122.58.10
				addnode= 136.243.40.220


				$sudo ./mindcoind


