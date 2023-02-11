# HAproxy-load-balancer 2

An Ansible role that install/manage haproxy-load-balancer to CENTOS 7/8, Rocky9 and Ubuntu.[link](hhttps://www.haproxy.com/)

## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

The Role also use `community.general collection` module. To install it, use: `ansible-galaxy collection install community.general`. 

## Tasks descriptionsa

- main.yml - Run the OS check and run the relevant playbook
- rhel-install-haproxy-lb.yml - Deploy HAproxy-load-balancer on Rhel
- run-config-haproxy-lb.yml - Configure HAproxy-load-balancer svc
- ubuntu-install-haproxy-lb.yml - Deploy HAproxy-load-balancer on Ubuntu


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-haproxy-lb
```

## Maintainer Information
Lee | 2023