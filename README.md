# k3s Cluster Automated Deployment with Ansible

This project automates the deployment of a highly-available k3s Kubernetes cluster using Ansible. It is designed to be modular, configurable, and easy to extend.

## Project Structure

```
cluster_deploy/
├── ansible.cfg
├── inventory/
│   └── hosts.ini
├── group_vars/
│   ├── all.yml
│   ├── controllers.yml
│   └── workers.yml
├── roles/
│   ├── common/
│   ├── k3s_controller/
│   └── k3s_worker/
├── playbooks/
│   ├── site.yml
│   ├── preflight.yml
│   └── postflight.yml
├── files/
├── templates/
└── README.md
```

## Getting Started

1. **Edit the inventory file**: Add your node IPs and hostnames to `inventory/hosts.ini`.
2. **Configure variables**: Adjust settings in `group_vars/` as needed.
3. **Run the playbook**: Execute the main playbook to deploy your cluster.

## Requirements
- Ansible 2.10+
- SSH access to all nodes

## Next Steps
We will iteratively build out each component, starting with the inventory and group variables. 