ansible-marathon
=============
[![Build Status](https://travis-ci.org/AnsibleShipyard/ansible-marathon.svg?branch=master)](https://travis-ci.org/AnsibleShipyard/ansible-marathon)

Marathon role for Ansible. Marathon is installed with HA mode activated [(see command line options)](https://github.com/mesosphere/marathon#command-line-options).

## Requirements

* Ansible-Java, or Java installed on the host machine

## Role Variables

See ```defaults/main.yml``` for a full list. The most important settings are:

* ```zookeeper_hostnames: "localhost:2181"``` The path to Zookeeper which Marathon can use to find the Mesos masters and use as a state store.
* ```mesos_zookeeper_path: "/mesos"``` The path to Mesos in the Zookeeper cluster
* ```marathon_zookeeper_path: "/marathon"``` The path to Marathon in the Zookeeper cluster 
