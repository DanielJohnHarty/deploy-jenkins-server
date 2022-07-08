# Deploy Jenkins Server

Use the ansible role `ansible-jenkins-role` to deploy to a parameterised server.

## Usage

First clone this repo and init the git submodules:

```bash
git clone https://github.com/DanielJohnHarty/deploy-jenkins-server.git
cd deploy-jenkins-server
git submodule update --init --recursive
```

Deploy the jenkins server with:
```bash
ansible-playbook deploy-jenkins.yml
```

> There is currently a manual step to create the first Jenkins user. Ansible will print the instructions to the console and pause while you perform the actions.
