# Monero Library
Monero Library built with PHP and some coffee by SerHack!

## How it works
Monero Library (aka Monero_Payments.php) will try to connect to your Monero RPC Daemon (monero-wallet-rpc, See section how to use for more information).
Monero RPC Daemon has a json api that can communicate with Monero Library. Automatically Monero Library will know your address and others things.

## Preview
![Preview](http://i.imgur.com/fyfRCOS.png)

## Configuration
### Requirements
 - PC + internet
 - Ubuntu or Debian
 - Monero daemon
 - PHP server like XMPP; Apache or ngix
 
###

Step 1: Start the Monero Daemon as Testnet
```bash
monerod --testnet --detach
```

Step 2: Start the Monero Wallet RPC
```bash
monero-wallet-rpc --testnet --rpc-bind-port 28080 --disable-rpc-login --wallet-file /path/walletfile
```

Step 3: Edit example.php with your ip (127.0.0.1 for localhost) and port of Monero Wallet RPC (in the example it's 127.0.1 and 28080 port)


Step 4: Open your browser with your ip of XMPP, apache or nginx server and execute example.php. If library works. it will print your address
