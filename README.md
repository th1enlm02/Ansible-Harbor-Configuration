# Install and configure Harbor using Ansible

## About

This is a setup for installing and managing configurations of [**Harbor**](https://goharbor.io/). The setup is only configured for HTTP access (port 80). For HTTPs access, you need to follow this [**link**](https://goharbor.io/docs/2.0.0/install-config/) to see the detailed instructions.

## Preriquisites

1. **Ansible host**: Of course you need to install Ansible first &rarr; [Here](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)
2. **Harbor server**:
    - [Docker](https://docs.docker.com/engine/install/)
    - [Docker Compose](https://docs.docker.com/compose/install/)

> :memo: The Harbor's version will be installed is v2.11.0 and I will use the offline installer.

## Let's go

1. **Clone the repo**:

```bash
git clone https://github.com/th1enlm02/Ansible-Harbor-Configuration.git
cd Ansible-Harbor-Configuration
```
2. **In the Ansible host**:

```bash
ansible-playbook -i inventory site.yml
```
### 
> :warning: This setup is a example and just suitable for my context. You should update some variables if you want to use it.