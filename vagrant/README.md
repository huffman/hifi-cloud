Vagrant Environments
==================

###Initial Setup

> - Install VirtualBox (https://www.virtualbox.org/wiki/Downloads)
> - Install Vagrant (https://www.vagrantup.com/downloads.html)

###Loading an environment

```
~/hifi-cloud$ cd vagrant/hifi-ubuntu-dev
~/hifi-cloud/vagrant/hifi-ubuntu-dev$ vagrant up
~/hifi-cloud/vagrant/hifi-ubuntu-dev$ vagrant ssh
```

###Destroying an environment

```
~/hifi-cloud/vagrant/hifi-ubuntu-dev$ vagrant destroy
```

Environments
===========

###**hifi-ubuntu-dev**
Ubuntu 14.04 development and staging environment for backend High Fidelity Stack.
You will get the master highfidelity/hifi repo cloned in the vagrant's user ~. There is no need to set any environment variables, simply:

```
~$ mkdir master-hifi/build
~$ cd master-hifi/build
~$ cmake ..
~$ make
```
