HDCH is a P2P value delivery public chain. By offering its blockchain infrastructure and digital resource distribution protocols, it enables third-party developers to explore their own applications over open-source agreements to form a complete ecology of blockchain technology and applications. With the health data blockchain ecosystem, healthcare service providers can analyze human health data, and provide intelligent healthcare applications. With HDCH smart contract, doctors can add medical records, scan test results, and record drug consumption on the blockchain. Patients can obtain healthcare services through awarding doctors tokens. They can give the insurance company limited access of their data to verify the treatments and audit the claim settlements. Patients can obtain tokens by actively following treatments and make progress with their health conditions. Patients can also be rewarded by giving research institutions and pharmaceutical companies time-limited access to health data for medical experiments.

HDCHChain Documentation and Usage Resources
---------------
Resources may be helpful to know about HDCH.

Basic usage resources:

* [Official site](http://www.hdch.io/)
* [Whitepaper](http://www.hdch.io/HDCH_Whitepaper_v1_0.pdf)

General Info about HDCH:

* [Community](http://www.hdch.one/)

What is HDCHChain?
------------------

HDCHChain is a infrastructure chain layer and adopts the mixed consensus mechanism of POW and POS.It supports the intermediate layer and top application layer of the HDCH.
HDCHChain is the infrastructure of the whole ecosystem.

Building HDCHChain
-------------------

### Build on Ubuntu(16.04 LTS)

    git clone https://github.com/hdch-io/hdchain.git

Install dependency

    sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    sudo apt-get install software-properties-common
    sudo add-apt-repository ppa:bitcoin/bitcoin
    sudo apt-get update
    sudo apt-get install libdb4.8-dev libdb4.8++-dev
    sudo apt-get install libminiupnpc-dev
    sudo apt-get install libzmq3-dev

    # QT 5, for GUI
    sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler    
    # optional
    sudo apt-get install libqrencode-dev

Configure and make

    ./autogen.sh
    ./configure
    make -j(number of threads)

### Run

    cd src && ./hdchd -daemon 
    #You can use ./hdch-cli help  to obtain HDCH's commands.

Development Process
-------------------

The master branch is constantly updated and developed, while stable
and versionized executables will be published once mainnet is published.

Issues and commit changes are welcome.

Testing
-------
You can find the unit test cases [here](./src/test).
