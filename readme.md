## BitDB on BCH testnet
### Install
* git clone https://github.com/SpendBCH/bitdb-testnet.git
* cd bitdb-testnet
* npm install
* npm install -g pm2
* pm2 install pm2-logrotate

### Configure
* Set your bitcoin RPC host, RPC username, and RPC password in process.json
* Set the script location and cwd in process.json
* Set the block height to start syncing from in bitdb.json
  * The default 1190000 will sync 2018 BCH testnet
* Set ports in config.js if using testnet ports, or configure BCH node to use mainnet ports instead

### Run
* pm2 start process.json

### Debug / Monitor
* pm2 logs bitd

Forked from: https://github.com/21centurymotorcompany/bitd