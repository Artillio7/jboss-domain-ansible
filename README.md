# Ansible Playbook for JBoss Domain Mode (WildFly) Management

This repository provides a reusable Ansible playbook to automate the setup and management of JBoss servers in domain mode (WildFly 24).

## Features
- Create a server group
- Add a server instance and start it
- Deploy a `.war` application
- Set JVM heap size and max
- Restart the server conditionally

## Structure
```
jboss-domain-ansible/
├── inventory/
│   ├── inventory.yml
│   ├── group_vars/
│   └── host_vars/
├── vars/
│   ├── connection_vars.yml
│   └── app_vars.yml
├── playbook.yml
└── README.md
```

## Usage
```bash
ansible-playbook -i inventory/inventory.yml playbook.yml
```
Make sure to fill in your variable values in `vars/` and `host_vars/`.
