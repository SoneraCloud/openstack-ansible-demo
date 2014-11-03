pouta-ansible-demo
==================

Simple Ansible demo to deploy a machine to Pouta

To use this demo you will need:
 - Ansible:
   http://docs.ansible.com/intro_installation.html
 - OpenStack command line tools:
   http://docs.openstack.org/user-guide/content/install_clients.html
 - Access to pouta:
   https://research.csc.fi/pouta-access
 - Your Pouta openstack RC file:
   https://research.csc.fi/pouta-install-client

To launch the demo:

1. `ansible-playbook create-instance.yml`
2. `ansible-playbook -i demo.hosts setup-instance.yml`
