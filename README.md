# deb

Debian/Ubuntu repo

## Repository usage

```
# Add source
add-apt-repository 'deb http://deb.gab.lc /'

# Add GPG key
wget -O - http://deb.gab.lc/keyFile | sudo apt-key add -

# Install a package
apt update
apt install ardb-server # or another package
```

## Build package index

```
./build_index.sh
```