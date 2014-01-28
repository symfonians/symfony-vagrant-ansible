symfony-vagrant-ansible
=======================

This project allow to easily start a symfony project using Vagrant and Ansible for environment and provisioning setup

## Before you start

This project demonstrate the ability of installing Symfony with Vagrant and Ansible. It is mostly suitable for a development environment, but could be adapted for a production environment. Feel free to contribute and to fix the mistakes.

## Prerequisites

This project do not cover the installation and introduction to Vagrant and Ansible. It suppose you've already tried both tutorials and that you have installed the following softwares on your computer:

- VirtualBox (https://www.virtualbox.org/)
- Vagrant (http://www.vagrantup.com/)
- Ansible (http://www.ansible.com/home)

## Installation

After you have installed the prerequisites softwares, just clone this repository on your computer, and from there, execute the following command:

``` bash
$ vagrant up
```

## Configuration

This project is pre-configured to install an Ubuntu Precision 64bits with PHP-FPM, Postgresql, Nginx and the standard symfony version 2.4.*. It also create a network interface with the IP 192.168.100.100 and allows the app_dev.php to be accessible from your local machine.

To modify the Vagrant configuration and IP address just edit the Vagrant configuration:


    Vagrantfile


To ajust the Ansible parameters, database and some flavors, edit the playbook global variables:


    provisioning/group_vars/all

Enjoy!