# Setup on Ubuntu

## These are only required on ubuntu systems.
```
sudo apt update && sudo apt upgrade -y
sudo apt install git curl nginx tmux build-essential pkg-config libssl-dev clang protobuf-compiler -y
```

## Install Rust
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Input **1 + enter** (Proceed with installation (default))
```
source "$HOME/.cargo/env"
```
## Install Docker
```
sudo apt install curl -y && source <(curl -s https://nodesync.top/docker_install)
```
## Madara CLI
### Clone repo
```
git clone https://github.com/karnotxyz/madara-cli
```

### Build repo
```
cd madara-cli && cargo build --release
```
#### Congratulations! You now have a custom madara app running.

### Initialize a new app chain. Please fund the DA account (if applicable)
#### Note: Save da-config.json (seed)
```
./target/release/madara init
```

### Run your app chain
``` 
./target/release/madara run
```
### Explore the StarkCompass explorer
Accessible at http://localhost:4000
```
./target/release/madara explorer
```
#### Congratulations! You now have a custom madara app running.
