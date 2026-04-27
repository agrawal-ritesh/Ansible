# What is Ansible

### Its a tool to Automate the tasks across multiple computers at once. (Servers, Cloud VMs)

### What it actually does.

- Install Softwares
- Configure systems
- Deploy applications
- Manage multiple servers

### You write a simple file called Playbooks in Ansible. 

* Example:
```yaml
- hosts: servers
  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present
```

- Ansible Command:
ansible-playbook playbook.yml


> Hosts are the target machines.
> Servers are the names of machines from the inventory files.
> Task defines what to do on those machines
> -name: Install nginx is just the label which helps to read output
> apt: -> this is a module. (Modules are basically the tools used by ansible to do the job.)
> other examples are like, yum, copy services - There are the modules in ansible.
> nginx - tells which packages needs to be installed.
> State present -> defines the desired state.
> become: yes -> Installing software needs sudo/root access