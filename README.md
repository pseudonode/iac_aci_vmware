# iac_aci_vmware

This repo contains Ansible roles and playbooks to orchestrate end to end network and virtualization infrastructure.

This collection allows for the creation of Cisco ACI constructs as well as VMWARE vSphere constructs.

The repository consists of two roles:
- aci
- vsphere



# ACI Role

The aci role contains a /tasks playbook that allows for the creation of the following ACI primitives:

- Tenant
- Application Profile
- Bridge Domains
- Bridge Domain subnet
- Bridge Domain association with L3Out
- Endpoint Groups
- Endpoint Group Association with VMM Domain
- Endpoint Group association with security contracts

The ACI data model is defined inside of the group_vars folder of the project.

# VSPHERE Role

The vsphere role contains a /tasks playbook that allows for the creation of one or multiple VMs from a VM Template leveraging the vmware_guest module

VM data is defined inside of host_vars and VM hostnames are defined inside if the inventory file

The vSphere data model is defined inside of the host_vars folder of the project
