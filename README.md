# Ansible's playbook Docker Nexus
Playbook to build nexus server running on docker

Before running the playbook
- Create hosts file with Server name inside
```
echo "[nexus]
[HOST IP] >> /etc/ansible/hosts
```

TODO
----
- Login - default credentials are admin admin123

TO RUN PLAYBOOK
```
ansible-playbook nexus_playbook.yml
```

### To start nexus docker container manually
```
mkdir /nexus-data && chown -R 200 /nexus-data
docker run -v /nexus-data:/nexus-data:rw -p 38081:8081 -p 5000:5000 --restart always -d sonatype/nexus3
```
