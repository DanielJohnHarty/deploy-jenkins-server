# Deploy Jenkins Server

Use the ansible role `ansible-jenkins-role` to deploy to a parameterised server.

## Usage

Optionally generate an ansible hosts file from the variables defined in `inventory/group_vars/all.yml`:

```bash
ansible-playbook generate-ansible-hosts-file.yml
```

Then deploy the jenkins server with:

```bash
ansible-playbook deploy-jenkins.yml
```

After the playbook is complete, navigate to the server using the url `http://<JENKINS_SERVER_IP>:<JENKINS_PORT>/login`. A temporary administrator password fetched from your Jenkins server after installation and is written to the local file `./files/initialAdministratorPassword`. Use this password to initially login.

You'll be promted to perform some post installation steps manually after which you can begin using using Jenkins.


