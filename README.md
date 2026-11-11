# my-linux-setup

## update and upgrade

```bash
sudo apt update
sudo apt upgrade
```

## Rust

install build-essential and curl

```bash
sudo apt install build-essential
sudo apt install curl
```

install rust using [rustup](https://rustup.rs/)

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Helix

install [helix](https://helix-editor.com/) using snap

```bash
snap install --classic helix
```

### Helix config

run `hx` then quit it

copy [helix config file](./configs/helix/config.toml) to `~/.config/helix`

## Zellij

Install [Zellij](https://github.com/zellij-org/zellij) using cargo

```bash
https://github.com/zellij-org/zellij
```

### Zellij config

run `zellij` and then quit it

copy [zellij code layout](configs/zellij/layouts/code.kdl) to `~/.config/zellij/layouts`

create alias for code layout

```bash
echo 'alias zc="zellij --layout code"' >> ~/.bashrc
source ~/.bashrc
```

### Rust Analyzer

Install Rust Analyzer for Rust LSP

```bash
rustup component add rust-analyzer
```

## Opencode

install [Bun](https://bun.com/docs/installation)

```bash
curl -fsSL https://bun.com/install | bash
```

add bun to path

```bash
echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc
source ~/.bashrc
```

then install [opencode](https://opencode.ai/) using bun

```bash
bun install -g --trust @opencode/cli
```

## Zed

install [zed](https://zed.dev/docs/linux) 

```bash
curl -f https://zed.dev/install.sh | sh
```

## GDB

### GDB config

copy [gdb init file](configs/gdb/.gdbinit) to `~`
