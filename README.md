# Ansible Splunk Connect For Syslog (SC4S)

iManage Security Operations
<secops@imanage.com>

# Overview

Install all the needed pieces for the SC4S parts.

# Contents
```
defaults
defaults/main.yml
defaults/README.md
files
files/README.md
handlers
handlers/main.yml
handlers/README.md
meta
meta/main.yml
meta/README.md
README.md
tasks/
tasks/envfile.yml
tasks/systemd.yml
tasks/docker-repo.yml
tasks/basedirs.yml
tasks/sc4s-start.yml
tasks/yum-utils.yml
tasks/docker-volume.yml
tasks/docker-packages.yml
tasks/firewalld.yml
tasks/docker-start.yml
tasks/main.yml
tasks/diskvols.yml
tasks/README.md
vars
vars/main.yml
vars/README.md
templates
templates/README.md
```


# Usage

From a playbook:

```
- hosts: localhost
  become: yes
  tasks:

    - include_role:
        name: splunk-sc4s
```

From the command line:

```
ansible -i <inventory> <target> -m include_role -a name=role_template
```

If the role needs to 'become' (root) for privileged operations:

```
ansible -i <inventory> <target> -m include_role -a name=role_template -b
```