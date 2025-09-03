# hostsctl

A tiny, safe helper for `/etc/hosts` that can add/remove hostnames idempotently.

## Features
- `add` / `remove` / `exists` / `list` / `backup` / `restore`
- Atomic writes, auto-backup
- Multiple hostnames per IP
- Linux/macOS/WSL
- `HOSTS_PATH` override for testing

## Quick Start
```bash
chmod +x hostsctl
sudo ./hostsctl add [ip] [hostname]
./hostsctl exists [hostname]
```

## Usage
```bash
hostsctl add <ip> <hostname> [more_hostnames...]
hostsctl remove <hostname>
hostsctl exists <hostname>
hostsctl list
hostsctl backup [path]
hostsctl restore <path>
```
