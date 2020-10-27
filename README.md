
![Ansible Lint](https://github.com/tenantcloud/ansible-role-cert-gen/workflows/Ansible%20Lint/badge.svg?branch-master)
![Yaml Lint](https://github.com/tenantcloud/ansible-role-cert-gen/workflows/Yaml%20Lint/badge.svg?branch-master)

tenantcloud.cert_gen
=========

Ansible role for generating custom certificates

  - tenantcloud_cert_gen

Requirements
------------

Install tenantcloud.dashboard
Install tenantcloud.promo

Role Variables
--------------

ansible_user: "user"
work_dir: "/usr/local/etc/nginx/ssl/"
work_domain: 
root_cert_name: 
root_email_address: 

Dependencies
------------

  - python@3
  - ansible

Example Playbook
----------------

```yaml
- hosts: localhost
  become: no
  vars:
    ansible_user: "user"
    work_dir: "/usr/local/etc/nginx/ssl"
    work_domain: 
    root_cert_name: 
    root_email_address: 
  roles:
    - tenantcloud.cert_gen
```

License
-------

BSD

Author Information
------------------

TenantCloud DevOps Team
