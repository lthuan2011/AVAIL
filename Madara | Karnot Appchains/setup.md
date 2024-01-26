# Setup on Ubuntu

## These are only required on ubuntu systems.
```sudo apt update && sudo apt upgrade```
sudo apt install git curl tmux build-essential pkg-config libssl-dev clang protobuf-compiler -y```

## Install Rust
```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh```

## Madara CLI
### Clone repo
```git clone https://github.com/karnotxyz/madara-cli```

### Build repo
``` cd madara-cli && cargo build --release```

### nitialize a new app chain. Please fund the DA account (if applicable)
```./target/release/madara init```

### Run your app chain
``` ./target/release/madara run```
