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
