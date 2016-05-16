openstack-ansible-demo
==================

Simple Ansible demo to deploy a machine to an OpenStack cloud

To use this demo you will need:
 - Ansible 2.0:
   http://docs.ansible.com/intro_installation.html
 - Python >=2.7:
   Needed by the os_security_group ansible module
 - OpenStack command line tools:
   http://docs.openstack.org/user-guide/content/install_clients.html
 - Shade: pip install shade
   http://docs.openstack.org/infra/shade/
 - Access to an openstack cloud. For example:
   https://research.csc.fi/pouta-access
 - Your openstack RC file:
   http://docs.openstack.org/user-guide/common/cli_set_environment_variables_using_openstack_rc.html
 - Your SSH public key uploaded to the remote cloud:
   http://docs.openstack.org/user-guide/cli_nova_configure_access_security_for_instances.html

Configuration:

You will need to get some information from your OpenStack account in order to run this demo. See the comments in demo.yml.

To launch the demo:

    ansible-playbook demo.yml
