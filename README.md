# Ansible AWS Automation

Ansible playbooks to manage AWS EC2 instances and Docker installation.

## AWS Credentials
- AWS keys are stored securely using **Ansible Vault**.
- Use `--vault-password-file vault.pass` to run playbooks.

## Playbooks
- `create_instance.yml` → Launch EC2 instances with optional EBS.
- `install_docker.yml` → Install Docker on Ubuntu/AWS Linux.
- `stop_ubuntu.yml` → Stop Ubuntu servers.

## Usage
```bash
ansible-playbook -i inventory.ini playbooks/<playbook>.yml --vault-password-file vault.pass
