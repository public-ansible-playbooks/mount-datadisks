mount-datadisks
=========

A playbook to create partitions and mount for additional data managed disks at Azure VMs

Requirements
------------

Only testd with the condition below:
- OS: CentOS7 and RHEL7
- Ansible 2.8 should be installled

sshpass should be installed at ansible executor host

Dependencies
------------

None

How to use
----------------
1. Set appropriate mount points to group_vars/all.yml
2. Call ansible roles to setup
```shell
$ ansible-galaxy install -r requirements.yml -p roles
``` 
3. Execute ansible playbook
```shell
$ ansible-playbook -i hosts site.yml -k -K
```
