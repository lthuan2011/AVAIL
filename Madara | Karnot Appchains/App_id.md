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

## create-app-id
```
cd $HOME/avail/avail-js/examples/node-examples
```
```
npm run create-app-id
```
You would see a log like the one below. **164** will be your
**app_id.dataAvailability.ApplicationKeyCreated::["0x546573742061707020617364736164736164616461206173646173646173","5Ci3f87otQeRC2y5gitVvbsez6EwCinhJwaK78MU2fCjv6Q5",164]**

