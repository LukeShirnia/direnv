Ansible Role: direnv
=========

This deploys the latest version of direnv to a Linux machine and adds the appropriate lines into .bashrc to load and view the directory enviroment


Role Variables
--------------
Update var to include the user in the "bashrc_direnv_update.yml" and "show_loaded_env.yml" tasks
```
user: "default"
```


Example Playbook
----------------

```
---
- hosts: all
  become: yes
  roles:
    - direnv
  vars:
    user: luke
```

License
-------

apache

Author Information
------------------

This role was created by [Luke Shirnia](https://shirnia.com)