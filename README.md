# Ansible Playbook for a Docker Swarm demo platform

This playbook deploy a High Availability Docker Swarm cluster with:

* 2 Manager nodes
* 1 Consul node
* 2 Worker nodes

## Requirements

* Ansible 1.2 or newer
* Debian Jessie

## How to use it

1. Fill in inventory file (hosts) with your hosts
2. Verify that your hosts are recheable: `ansible all -i hosts.yml -m ping`
3. Launch the playbook: `ansible-playbook ansible-playbook -i hosts docker-swarm.yml`
