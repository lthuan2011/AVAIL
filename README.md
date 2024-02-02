# Avail Upgrade v1.10.0.0
## Auto Install use Snap NodeSync
Please change  ```ABCXYX```  is Your Name on Telemetry
```
cd $HOME && yourname=ABCXYX  && sudo apt install curl -y && source <(curl -s https://raw.githubusercontent.com/lthuan2011/Avail/main/auto_install_snap_ns)
```
## Auto Install use Snap Avail
Please change  ```ABCXYX```  is Your Name on Telemetry
```
cd $HOME && yourname=ABCXYX  && sudo apt install curl -y && source <(curl -s https://github.com/lthuan2011/Avail/blob/main/auto_install_snap_avail)
```
### Get Session Keys
```
curl -H "Content-Type: application/json" -d '{"id":1, "jsonrpc":"2.0", "method": "author_rotateKeys", "params":[]}' http://localhost:9944
```
