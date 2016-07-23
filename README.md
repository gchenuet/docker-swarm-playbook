# Ansible HA Docker Swarm Cluster Playbook

This playbook deploy a High Availability Docker Swarm cluster via Consul HA
service.

You can choose how many nodes you want for Manager, Consul and Worker nodes
with the inventory file.

Default is:

* 2 Manager nodes
* 1 Consul node
* 2 Worker nodes

## Requirements

* Ansible 2.1 or newer
* Debian Jessie

## How to use it

1. Fill in inventory file (hosts) with your hosts and variables in
   `group_vars/all`
2. Verify your hosts are recheable via Ansible: `ansible all -i hosts.yml -m ping`
3. Launch the playbook: `ansible-playbook ansible-playbook -i hosts docker-swarm.yml`
