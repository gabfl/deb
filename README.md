# deb

Ubuntu repo

## Supported Ubuntu versions

Currently supported Ubuntu versions are:
 - Xenial (16)
 - Bionic (18)

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
