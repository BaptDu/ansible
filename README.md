Ansible
=========

Allows, depending on the configuration, to automate the configuration of the server and install everything needed for its commissioning.

Prerequisite
------------
```bash
python get-pip.py
python -m pip install ansible
```

Requirements
------------

For the proper functioning of the role, you will have to create a `hosts.yml` and `playbook.yml` file and copy the information from `hosts.example` , `playbook.example` and fill in the information in it.


Hosts Variables
--------------

```yml
all:
  hosts:
    name_for_serveur:
      ansible_host: ip for host
      ansible_port: number for host
      ansible_user: user for host
      ansible_ssh_private_key_file: path for key id_rsa (optional)
      ansible_python_interpreter: /usr/bin/python3
      ansible_sudo_pass: password sudo for execute command
    # ...
```

Playbook Variables
--------------

```yml
- hosts: name_for_serveur
  roles:
    - dependencies
    - role : docker
```

Launch ansible
--------------

```bash
ansible-playbook -i hosts.yml playbook.yml
```


Author Information
------------------
* **DUMONT Baptiste** _alias_ [@BaptDu](https://github.com/BaptDu)
