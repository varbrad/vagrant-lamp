# Vagrant LAMP
LAMP stack for Vagrant.

* Ubuntu Server 14.04 64bit (Trusty Tahr)
* Apache 2.4.7
* PHP 5.5.9
* MySQL 5.5.58
* phpmyadmin
* Git 1.9.1
* Composer 1.5.2
* Node 8.9
* nvm

Access `192.168.33.10` on your machine to access the apache webserver root, server from `www/`. All files within `www/` on your local machine will be synchronized with the contents of the virtual machine.

## Use

First ensure Vagrant is installed and configured on your machine. Simply copy the `Vagrantfile` and `vagrant.sh` files into your project directory, and then `vagrant up` within that directory to setup the VM, install all of the resources and run the server.

From here, you can access `192.168.33.10` from your local machine on a browser such as Google Chrome. You may also wish to edit your local machine hosts folder to setup a virtual host. E.g. `192.168.33.10 local.dev`. This will allow you to visit `local.dev` in a browser.

Once you are finished, simply `vagrant halt` to shut down the VM.

## Why?

I needed a reliable way of emulating a LAMP installation running PHP 5.5 and MySQL 5.5, to ensure I don't accidentally use any fancy new PHP 7 goodies!
