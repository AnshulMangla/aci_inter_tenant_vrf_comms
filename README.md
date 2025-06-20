# Cisco ACI Inter VRF/Tenant Route Leaking

## Summary

This repository contains a set of different examples of ansible playbooks for automating Cisco ACI.
Ansible Playbook to Automate creation of VRFs &amp; associated objects for communication between VRF/Tenants.

## Inventory & variables

Update the variable of inventory.yaml & variables.csv based on your environment with APIC IP and credential.


## Instructions

These playbooks has been tested with Ansible 2.10 and Cisco ACI collection 2.0.0.

Cisco ACI ansible collection can be installed using the following command:

```
$ ansible-galaxy collection install cisco.aci
```

Cisco ACI ansible collection can be upgraded using either --force option or --upgrade option (available in 2.10+):

```
$ ansible-galaxy collection install cisco.aci --force
```

Before using these playbooks, ansible inventory needs to modified according to your environment. Demo01 has the password hard-coded in the playbook, it has been removed from the repository.

To run the playbooks:

```
$ ansible-playbook -i inventory.yaml demoXX/demoXX.yaml
```

