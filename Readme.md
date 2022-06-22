Ansible Role Packer
=========

Installs Packer-cli on Debian/Ubuntu servers. 

Role Variables
--------------

```
# Packer Version to install
packer_version: ""

# Toggling this will uninstall from the server
uninstall: false
```

Example Playbooks
----------------

Minimal:
```
- name: Install Packer
  hosts: all
  roles:
    - role: exzeo.packer
```

Specific Version:
```
- name: Install Packer
  hosts: all
  roles:
    - role: exzeo.packer
      vars:
        packer_version: ""
```

Uninstall:
```
- name: Install Packer
  hosts: all
  roles:
    - role: exzeo.packer
      vars:
        uninstall: true
```