# Ansible/Monit
A nice little server monitoring and documentation example

## Preparation

- [Install Ansible](http://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-pip)
- Be sure you can connect with your hosts and become root without password on them `ssh blog.entwicklerbier.org sudo -n`. If you want to know more about privilege escalation with ansible, I recommend reading [this](http://docs.ansible.com/ansible/become.html).

## Usage
You need to write/generate your own `hosts`, `host_vars/*`, `.group_vars/all/mail_credentials.yml` and `.vault_passphrase` for this to work.
Have a look at the commit history of this repo for further explanation.

### All Hosts
```
ansible-playbook playbook.yml
```

### Specific Host
```
ansible-playbook -l blog.entwicklerbier.org playbook.yml
```
