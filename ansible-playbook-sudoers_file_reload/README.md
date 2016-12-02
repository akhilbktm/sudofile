ANSIBLE PLAYBOOK TO RELOAD SUDOERS FILE
============================================
### Platform
Ansible
### Authors
akhil.baby@reancloud.com

### Implementation
This playbook is to reload sudoers configuration file for the group entries
### Pre-requisites and Dependencies
* Python 2.7.5
* ansible 2.2.0.0

## Usage Information
Installation

* install the epel-release RPM if needed on CentOS, RHEL, or Scientific Linux
$ sudo yum install ansible

* Ubuntu machines
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible

Genearting hosts File

Please follow the steps in below document:
https://reancloud.atlassian.net/wiki/display/ENG/Ansible+playbook+for+Instance+Facts

Steps 

	*Clone the repo to your local machine.
	*Edit the hosts file with all linux instanced need to Installed with sar package.
	*Run the ansible playbook with the below command :
		ansible-playbook -i hosts reload.yml

### Release Notes

Initial version of the playbook.
