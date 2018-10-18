
# Running docker inside Vagrant Virtualbox in Windows 10

This is for folks who want to run docker engine on windows and also be able to use VirtualBox at the same time.

Got tired of trying to make my old vagrant boxes to run with HyperV provider. 

## Requirements
* Vagrant
* VirtualBox

## Quick Start

`vagrant up`

Open http://localhost:8000


To login inside Vagrant box, run

```
vagrant ssh

#vagrant dir is in:
cd /vagrant/docker
```

provision.sh is run once when box is provisioned, it sets up docker engine.
Bootstrap.sh is run on every vagrant start, it contains starting of docker engine. 

## Docker

Docker docker-compose.yml and other stuff is inside Docker directory. Build your docker stack in here.
Contains apache-php

Default document root is in Docker/DocumentRoot folder



I hope this helps.



