# Extract the tar file with the following command:
```
tar -xzvf bluemobius-daemon-linux.tar.gz
tar -xzvf bluemobius-qt-linux.tar.gz
```

# Type the following command to install the daemon and tools for your wallet:
```
sudo mv bluemobiusd bluemobius-cli bluemobius-tx /usr/bin/
```

# Type the following command to open your home directory:
```
cd $HOME
```

# Create the data directory for your coin with the following command:
```
mkdir $HOME/.bluemobius
```

# Open nano.
```
nano $HOME/.bluemobius/bluemobius.conf -t
```

# Paste the following into nano.
```
rpcuser=rpc_bluemobius
rpcpassword=dR2oBQ3K1zYMZQtJFZeAerhWxaJ5Lqeq9J2
rpcbind=127.0.0.1
rpcallowip=127.0.0.1
listen=1
server=1
txindex=1
daemon=1
paytxfee=0.0002
deprecatedrpc=accounts
addresstype=legacy
addnode=node1.bluemobius.eu
```

# Type the following command to start your daemon:
```
bluemobiusd
```

# Type the following command to create a wallet for your daemon:

```
bluemobius-cli createwallet ""
```

# Type the following command to create a new receiving address for your daemon:
```
bluemobius-cli getnewaddress ""
```
