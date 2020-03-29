# Ansible playbook

this is the collection of ansible playbooks used in [open-infrastructure.de](https://open-infrastructure.de)

## Setup

```
git submodule init
git submodule update --recursive
```

## Playbooks

### [main.yml](main.yml)

This is the main playbook to run all roles on all machines

### [base.yml](base.yml0

This is the base playbook to setup the hosts

### [ipsec_gateway.yml](ipsec_gateway.yml)

The IPsec playbook to setup the VPN infrastructure

### [jitsi.yml](jitsi.yml)

This playbook automates the [jitsi.rocks](https://jitsi.rocks) infrastructure (or at least the monitoring)

### [prometheus.yml](prometheus.yml)

This playbook deploys the prometheus based monitoring
