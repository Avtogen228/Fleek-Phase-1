# Fleek-Phase-1
Fleek Phase 1 Node Installation Guide

Minimum requirements for node:
4 CPU 32GB RAM 100GB SSD

## Installation
```
adduser <USERNAME>    
```
## Example:
```
adduser fleek    
```
##
```
usermod -aG sudo <USERNAME>
```

```
su <USERNAME>
```

```
curl https://get.fleek.network | bash
```

```
systemctl start lightning.service
```

Adding Fleek Network as user network in Metamask.

Network Name: ```Fleek Network```

RPC URL: ```https://rpc.testnet.fleek.network/rpc/v0```

Network ID: ```59330```

Currency: ```tFLK ```

Go to https://faucet.testnet.fleek.network/ and connect your wallet.
Make sure that Fleek Network is chosen as current network in Metamask.

Mint test tokens.

Press the "Stake Testnet FLK" button, then copy and paste the keys you will see. Enter your IP and press "stake".

Check your keys:
```
lgtn keys show
```

Approve necessary transaction in Metamask.

Status:
```
systemctl status lightning
```

Logs:
```
tail -f /var/log/lightning/output.log
```

Diagnostic logs:
```
tail -f /var/log/lightning/diagnostic.log
```
