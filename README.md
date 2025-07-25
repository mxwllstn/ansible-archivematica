# Archivematica playbook

The provided playbook installs Archivematica on a local server

Adapted from: https://github.com/artefactual/deploy-pub/tree/master/playbooks/archivematica-jammy

## Requirements

- Ansible 2.2 or newer

## How to use


1. Download the Ansible roles:
  ```
  $ ansible-galaxy install -f -p roles/ -r requirements.yml
  ```

2. Run ansible playbook:
  ```
  $ ansible-playbook -i inventory/hosts.yml singlenode.yml
  ```

# Login and credentials

If you are using the default values in vars-singlenode-XXXX.yml and Vagrantfile files, the login URLS are:

* Dashboard:       http://127.0.0.1
* Storage Service: http://127.0.0.1:8000

Credentials:

* user: admin
* password: archivematica

For more archivematica development information, see: https://github.com/artefactual/archivematica/tree/qa/1.x/hack#archivematica-development-on-docker-compose
