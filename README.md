# Avail Upgrade v1.10.0.0

```**My guide will auto delete old install and old version. **```

## 1. Auto Install use Snap NodeSync
Please change  ```ABCXYX```  is Your Name on Telemetry
```
cd $HOME && yourname=ABCXYX  && sudo apt install curl -y && source <(curl -s https://raw.githubusercontent.com/lthuan2011/Avail/main/auto_install_snap_ns)
```
## 2. Auto Install use Snap Avail
Please change  ```ABCXYX```  is Your Name on Telemetry
```
cd $HOME && yourname=ABCXYX  && sudo apt install curl -y && source <(curl -s https://github.com/lthuan2011/Avail/blob/main/auto_install_snap_avail)
```
## 3. Get Session Keys
```
curl -H "Content-Type: application/json" -d '{"id":1, "jsonrpc":"2.0", "method": "author_rotateKeys", "params":[]}' http://localhost:9944
```
## 4. Goldberg - Validator - Staking
```
https://goldberg.avail.tools/?rpc=wss://goldberg.avail.tools:443/ws#/staking
```
## 5. Avail Telemetry
```
https://telemetry.avail.tools/#list/0x6f09966420b2608d1947ccfb0f2a362450d1fc7fd902c29b67c906eaa965a7ae
```
