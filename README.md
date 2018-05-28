<html>
<body>
<p>LightPayCoin Core integration/staging repository<br>
=====================================</p>
<p><strong>Quick  installation of the daemon under linux (Ubuntu 16.04, root user):</strong></p>
<ul>
  <li><strong>Installation of libraries:</strong></li>
</ul>
<p>add-apt-repository ppa:bitcoin/bitcoin -y<br>
  apt-get update<br>
  apt-get install -y build-essential libtool  autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils -y<br>
  apt-get install -y libboost-system-dev  libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev  libboost-test-dev libboost-thread-dev<br>
  apt-get install -y libdb4.8-dev libdb4.8++-dev</p>
<ul>
  <li><strong>Cloning the repository and compiling:</strong></li>
</ul>
<p>git clone https://github.com/lpcproject/LightPayCoin.git<br>
  cd LightPayCoin<br>
  ./autogen.sh<br>
  ./configure<br>
  sudo make install<br>
  cd src<br>
  sudo strip lightpaycoind<br>
  sudo strip lightpaycoin-cli<br>
  sudo strip lightpaycoin-tx<br>
  cd ..</p>
<ul>
  <li><strong>Running  the daemon:</strong></li>
</ul>
<p>lightpaycoind </p>
<ul>
  <li><strong>Stopping the daemon:</strong></li>
</ul>
<p>lightpaycoin-cli stop</p>
<ul>
  <li><strong>Demon status:</strong></li>
</ul>
<p>lightpaycoin-cli getinfo<br>
  lightpaycoin-cli mnsync status</p>
</body>
</html>
