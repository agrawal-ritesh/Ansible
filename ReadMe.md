# What is Ansible

### Its a tool to Automate the tasks across multiple computers at once. (Servers, Cloud VMs)

### What it actually does.

- Install Softwares
- Configure systems
- Deploy applications
- Manage multiple servers

### You write a simple file called Playbooks in Ansible. 

* Example:
<!--
- hosts: servers
  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present
-->

- Ansible Command:
ansible-playbook playbook.yml