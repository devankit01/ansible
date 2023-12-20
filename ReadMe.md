# Ansible 

This repository contains Ansible playbooks for deploying a Python app with Docker on AWS EC2.

## Prerequisites

- Ansible installed
- AWS EC2 instance with SSH access
- Python on the target server

## Playbooks


1. **Ping EC2 Instance**
   ```bash
   ansible-playbook playbooks/ping_ec2.yaml -i inventory.ini --private-key /path/to/private-key.pem
   ```

2. **Install Dependencies**
   ```bash
   ansible-playbook playbooks/install_dependency.yaml -i inventory.ini --private-key /path/to/private-key.pem
   ```

3. **Deploy Python App**
   ```bash
   ansible-playbook playbooks/deploy_app.yaml -i inventory.ini --private-key /path/to/private-key.pem
   ```

## Inventory and Variables

- Update `inventory/ec2_hosts.ini` and `vars/vault.yaml` with your details.

## Notes

- Ensure SSH access to your EC2 instance.
- Replace `/path/to/private-key.pem` with your private key path.


