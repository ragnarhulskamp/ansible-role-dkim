# ansible-role-dkim
Ansible role for opendkim on CentOS

### Example playbook
```yaml
---
- hosts: testingnodes
  user: centos
  sudo: True
  vars:
      admin_email: admin@example.com
  roles:
    - role: ansible-role-dkim
      dkim_selector: default
      dkim_domains:
       - example.com
       - example.org
```
