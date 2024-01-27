# Registering an App Id on Avail

Go to https://goldberg.avail.tools/#/accounts and create an account on Avail. Keep the **seed** phrase safe.

Get funds on this new account using the **Avail faucet**.

# Install Node js and Npm using NVM
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```
```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
```
```
nvm -v
```
# Clone this repo Avail and config
```
git clone https://github.com/availproject/avail
```
```
cd $HOME/avail/avail-js/examples/ && npm i
```
```
cd $HOME/avail/avail-js/examples/node-examples/ && npm i
```
## Edit the config.ts file
```
nano $HOME/avail/avail-js/examples/config.ts
```
Change **your seed** and endpoint is **wss://goldberg.avail.tools:443/ws**

## config create-app-id
```
nano $HOME/avail/avail-js/examples/node-examples/src/create-app-id.ts
```
#### Change "YourAppName"

#### Delete line 26 is : process.exit(0)

<img src="https://raw.githubusercontent.com/lthuan2011/Avail/main/Madara%20%7C%20Karnot%20Appchains/appname.JPG">

## Create App ID
```
cd $HOME/avail/avail-js/examples/node-examples
```
```
npm run create-app-id
```
You would see a log like the one below. **164** will be your

**app_id.dataAvailability.ApplicationKeyCreated::["0x5465737420617070206461206173643646173","5Ci3f87otQeRC2y5gitVvbsez6EwCinhJwaK78MU2fCjv6Q5",164]**

If you don't see "ApplicationKeyCreated" on logs, it's error before, Please install again.

# Restart app chain with your APP_ID (Run in tmux)

ctrl +c (stop app)

Change **Your_Chain_Name**
```
nano /root/.madara/app-chains/Your_Chain_Name/da-config.json
```
Find and Change **"app_id":xxx** , xxx is your app id , save them

### Start 
```
./target/release/madara run
```



