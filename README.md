Open Droplet Hub - EmonCMS
==========================

This repo is meant to be used to setup a development environment for the open droplet emoncms fork. It is a wrapper around emoncms to be able to setup a Vagrant development environment. It uses the ```iilab/droplet-hub-config``` repo for ansible configuration management and the ```iilab/emoncms``` fork.

See [Open Droplet Hackpad - Software section](https://hackpad.com/Open-Droplet-TwGzhpxVHQB#:h=Software)

# Devops

Prerequisite
  * Vagrant 1.6.3+
  * Ansible 1.7+

To install the development environment run.

  * ```git clone https://github.com/opendroplet/droplet-hub-config.git```
  * ```git clone https://github.com/iilab/emoncms.git```
  * ```git clone https://github.com/opendroplet/droplet-hub-emoncms.git```
  * ```cd droplet-hub-emoncms```
  * ```vagrant up```
  * (```vagrant provision```) Only necessary if you modify the playbook or need to provisioning an existing and running vagrant VM.

You can then access emoncms at ```http://localhost:8088``` and register the admin user the first time.