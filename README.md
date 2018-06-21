# Ansible's Playbooks
Playbook to build Infra with:
- Pip
- Docker
- Sonar Docker Container & MySQL
- Nexus Docker Container

Before running the playbook
- Create hosts file with Server name inside
```
echo "[host]
[HOST IP] >> /etc/ansible/hosts
```

TODO
----
- Login - default credentials are admin admin123

TO RUN PLAYBOOK
```
ansible-playbook site.yml
```