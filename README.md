# deb

Ubuntu repo

## Supported Ubuntu versions

Currently supported Ubuntu versions are:
 - `xenial` (Ubuntu 16)
 - `bionic` (Ubuntu 18)

## Repository usage

```
# Add source
add-apt-repository "deb http://deb.gab.lc/ubuntu/$(lsb_release -cs) /"

# Add GPG key
wget -O - http://deb.gab.lc/keyFile | sudo apt-key add -

# Install a package
apt update
apt install ardb-server # or another package
```

## Clone me

 - Clone the repository
 - Create an Nginx vhost:

```
server {
    listen 80;

    root /path/to/deb;
    server_name deb.mydomain.com;

    location / {
        # Allow directory listing
        autoindex on;
    }
}
```