Role Name
=========

exports all projects from a group.

Requirements
------------

No requirements.

Role Variables
--------------

```yaml
ca_certificates_trust_file: files/CA.crt
```

Dependencies
------------

No dependencies.

Example Playbook
----------------

Including an example of how to use your role :

```yaml
- hosts: all
  tasks:
    - name: export projects from gitlab
      include_role:
        name: export-group-gitlab
      vars:
        gitlab_url: "https://gitlab.com"
        gitlab_api_token: "xxxxxxxxxxxxxxxx"
        gitlab_group_name: "default"
        local_download_folder: "export"
```

License
-------

Apache v2.0

Author Information
------------------

Mikaël LE BERRE
