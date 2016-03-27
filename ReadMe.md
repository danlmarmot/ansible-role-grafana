An Ansible role for installing grafana on Ubuntu 15.10.

### Default versions

Ubuntu 15.10
grafana 2.6.0

### Testing

A Vagrant/VirtualBox environment is provided in the /examples directory.  To get started:

1. Install Vagrant, Virtualbox, and Ansible
1. Change your directory into 'examples'
1. Run 'vagrant up' to bring up the VM.

### Additional notes

- For Vagrant installs, the install packages for grafana are downloaded once and cached locally.
- Each role in this Ansible playbook will check the version of each application before installing, and will not re-install if the installed version is the desired version.  This speeds up reprovisioning.
- To reprovision, use the 'vagrant provision' command.
