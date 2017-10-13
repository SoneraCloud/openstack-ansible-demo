openstack-ansible-demo
======================

Simple Ansible demo to deploy an instance and simple webserver to an OpenStack cloud

Configuration:

Create a (Python virtenv)[http://docs.python-guide.org/en/latest/dev/virtualenvs/#lower-level-virtualenv] and install the dependancies.

```
mkvirtualenv example
pip install -r requirements.txt
```

To launch the demo:

```
ansible-playbook demo.yml
```

Pointers:

To use this demo you will need:
 - Access to an openstack cloud. For example:
   https://research.csc.fi/pouta-access
 - Your openstack RC file:
   http://docs.openstack.org/user-guide/common/cli_set_environment_variables_using_openstack_rc.html
 - Your SSH public key uploaded to the remote cloud:
   http://docs.openstack.org/user-guide/cli_nova_configure_access_security_for_instances.html
   The code assumes you name the key the same as your local user account ... but you can override that.

 The `requirements.txt` pulls down what you need, but the dependancies are:
 - Ansible 2.4:
   http://docs.ansible.com/intro_installation.html
 - OpenStack command line tools:
   http://docs.openstack.org/user-guide/content/install_clients.html
 - Shade:
   http://docs.openstack.org/infra/shade/

