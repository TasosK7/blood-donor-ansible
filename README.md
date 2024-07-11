
# Project set up for VM servers

## Ensure that the VMs are reachable by Ansible

```bash
ansible -m ping all
```
## Postgres VM

```bash
ansible-playbook playbooks/postgres.yaml -l azure-db-server
```
## Backend(Spring) VM

```bash
ansible-playbook playbooks/spring.yaml -l azure-backend-server
```
## Frontend(Vuejs) VM

```bash
ansible-playbook playbooks/vuejs.yaml -l azure-frontend-server
```
## Docker VM

```bash
ansible-playbook playbooks/docker-app.yaml -l azure-docker-server
```

