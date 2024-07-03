# Apache Webserver Configuration Using Ansible

## Overview
This project provides Ansible playbooks to automate the installation and configuration of the Apache webserver on a target machine. It ensures a consistent setup of the webserver across different environments.

I am performing this project on Redhat V8 machine.
There will be commands different depending the OS you use.

## Features
Automated installation of Apache webserver
Configuration of virtual hosts
Enabling and disabling Apache modules
Customizable configuration files
Idempotent playbooks ensuring consistent state

## Requirements
Ansible 2.9 or higher: <br />
- You can install ansible using command
```
yum install ansible-core
```
- After installing ansible you can check version of ansible using command
```
ansible  --version
```
SSH access to the target machine(s)
Target machine(s) running a compatible operating system (e.g., Ubuntu, CentOS)
To check hosts are accessible or not you can do SSH to all the hosts and checdk if they are opening or not using SSH.

## Inventory File
Edit the inventory file to specify the target machines where Apache will be installed and configured.<br />
The inventory file will be look like this.
```
[webservers]
192.168.1.100
192.168.1.101
```
