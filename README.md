
![Lint Ansible Roles](https://github.com/tenantcloud/ansible-role-cert-gen/workflows/Lint%20Ansible%20Roles/badge.svg?branch-master)

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
nginx_ssl_directory:
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
    work_domain: "example.com"
    root_cert_name: "example-rootCA"
    root_email_address: "admin@example.com"
  roles:
    - tenantcloud.cert_gen
```

License
-------

BSD

Author Information
------------------

TenantCloud DevOps Team
