The Stack
=========
This repository contains a (very) opinionated ansible implementation of
[OpenStack Installation Guide for Ubuntu](http://docs.openstack.org/liberty/install-guide-ubuntu/) (Version: Ubuntu 14.04 / OS Liberty).

It is in no way meant to be generic or in any way high available. The goal
is to improve / extend this code as my Ansible / OpenStack experience grows.

The current system this setup will be deployed on has the following specs:
* 6 core Intel(R) Core(TM) i7-3930K CPU @ 3.20GHz
* 64 GB memory
* 2x 3TB HDD
* 1x 120GB SSD
* 1x Intel NIC

TODOs
-----
* refactor as hell, there is lots of code duplication (espacially regarding the config files)
  * move keystone service/user/endpoint...creation to their respective roles
* security (no SSL so far, internal services listening on 0.0.0.0)
