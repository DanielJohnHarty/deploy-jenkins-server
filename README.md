# Deploy Jenkins Server

Use the ansible role `ansible-jenkins-role` to deploy to a parameterised server.

## Usage

Optionally generate an ansible hosts file from the variables defined in `inventory/group_vars/all.yml`:

```
ansible-playbook generate-ansible-hosts-file.yml
```

Then deploy the jenkins server with:

```
ansible-playbook deploy-jenkins.yml
```