# Ansible playbook

this is the collection of ansible playbooks used in [open-infrastructure.de](https://open-infrastructure.de)

## Setup

```
git submodule init
git submodule update --recursive
```

## Playbooks

### [base.yml](base.yml)

This is the base playbook to setup the hosts

```
ansible-playbook prometheus.yml -i inventory/devops.yml --vault-password-file secret.txt
```


### [ipsec_gateway.yml](ipsec_gateway.yml)

The IPsec playbook to setup the VPN infrastructure

```
ansible-playbook prometheus.yml -i inventory/vpn.yml --vault-password-file secret.txt
```


### [jitsi.yml](jitsi.yml)

This playbook automates the [jitsi.rocks](https://jitsi.rocks) infrastructure (or at least the monitoring)

```
ansible-playbook prometheus.yml -i inventory/jitsirocks.yml --vault-password-file secret.txt
```


### [monitoring.yml](monitoring.yml)

This playbook deploys the prometheus based monitoring

```
ansible-playbook monitoring.yml -i inventory/devops.yml --vault-password-file secret.txt
```


