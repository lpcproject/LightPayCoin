LightPayCoin Core integration/staging repository
================================================

Quick installation of the LightPayCoin daemon under linux.

Installation of libraries:

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling:

    git clone https://github.com/lpcproject/LightPayCoin.git
    cd LightPayCoin
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip lightpaycoind
    sudo strip lightpaycoin-cli
    sudo strip lightpaycoin-tx
    cd ..

Running the daemon:

    lightpaycoind 

Stopping the daemon:

    lightpaycoin-cli stop

Demon status:

    lightpaycoin-cli getinfo
    lightpaycoin-cli mnsync status
