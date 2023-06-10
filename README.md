curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

rustup toolchain uninstall stable-x86_64-unknown-linux-gnu

rustup toolchain install stable-x86_64-unknown-linux-gnu

rustup target add wasm32-unknown-unknown

cargo install --locked --version 0.8.0 soroban-cli

cargo build --target wasm32-unknown-unknown --release
