# Ansible Role Template

iManage Security Operations
<secops@imanage.com>

# Defaults

If you find you're setting the same variables over and over, consider placing them into file(s) in here.

Official docs: [https://docs.ansible.com/ansible/latest/user_guide/playbooks_module_defaults.html](https://docs.ansible.com/ansible/latest/user_guide/playbooks_module_defaults.html)

If multiple variables of the same name are defined in different places, they win in a certain order, which is:

* extra vars (-e in the command line) always win
* then comes connection variables defined in inventory (ansible_ssh_user, etc)
* then comes "most everything else" (command line switches, vars in play, included vars, role vars, etc)
* then comes the rest of the variables defined in inventory
* then comes facts discovered about a system
* then "role defaults", which are the most "defaulty" and lose in priority to everything.
