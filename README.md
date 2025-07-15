# Nginx redundant setup example 
A simple redundant configuration using Nginx and keepalived only.

## Usage
Prepare two nodes running Debian 12, install there nginx and keepalived packages
```
    sudo apt update
    sudo apt upgrade -y
    sudo apt install -y nginx keepalived
```

Put `nginx.conf` files to `/etc/nginx/` and `keepalived.conf` to `/etc/keepalived/` for both nodes representatively, `check_nginx.sh` to `/usr/local/bin/` on the main node;

modify `interface` and `virtual_ipaddress` parameters in `/etc/keepalived/keepalived.conf` files according your servers;

sure `/usr/local/bin/check_nginx.sh` file is executable.

Demo video is available here: https://youtu.be/koCtExxB-d0
