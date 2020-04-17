# Ansible Role Template

iManage Security Operations
<secops@imanage.com>

# Meta

There's one file used here: main.yml

# Sample File

```
---
###############################################################################
#
# meta/main.yml
#
# Ansible Galaxy package metadata file for splunk-sc4s
#
###############################################################################

galaxy_info:
  role_name: role_template
  author: iManage Security Operations <secops@imanage.com>
  description: Standard Role Template
  company: iManage, LLC
  license: BSD
  min_ansible_version: 2.4
  issue_tracker_url: http://git.ch3.imanage.work/secops/secops/issues
  platforms:
    - name: 'Ubuntu'
      versions:
        - 'xenial'
        - 'bionic'
    - name: 'Debian'
      versions:
        - 'stretch'
    - name: 'EL'
      versions:
        - '7'
        - '8'
    - name: 'Amazon'
      versions:
        - '2017.12'
        - 'Candidate'

  galaxy_tags:
    - 'development'
    - 'system'
    - 'packaging'
```
