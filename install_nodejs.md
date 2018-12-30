# How to setup node.js

## Installation

### Sources

- [Installation of node on Ubuntu from nodesrc](https://github.com/nodesource/distributions/blob/master/README.md)
- [From Ubuntu repository](https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/#install-node-js-and-npm-from-the-ubuntu-repository), [from Node Source Repo](https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/#install-node-js-from-the-nodesource-repository), [using NVM](https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/#install-node-js-and-npm-using-nvm)
- [How to Install Node.js on Ubuntu 18.04 Bionic Beaver Linux](https://linuxconfig.org/how-to-install-node-js-on-ubuntu-18-04-bionic-beaver-linux)
- [Digital Ocean: nodejs and nginx](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-ubuntu-18-04)

### Decisions
- Use NVM
- Install latest stable version LTS (v11.6.0 (npm v6.5.0-next.0) as of 2018 12 30)

### Instructions
- Install NVM - see the steps on [https://github.com/creationix/nvm](https://github.com/creationix/nvm):

``` bash
cd ~
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash

# reload bash:
source ~/.profile
source ~/.bashrc


# verify  version:
nvm --version
```

- Installing node.js

``` bash
# Install latest version:
nvm install node

# Seems to be the same as stable:
nvm install stable
```

- [switching between versions](https://blog.pm2.io/install-node-js-with-nvm/)

``` bash
nvm use version_number 
# or
nvm use name_of_alias
```

- list versions: `nvm ls`
- make specific version default: `nvm alias default 10.13.0`

## First simple app


