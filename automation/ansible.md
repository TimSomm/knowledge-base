# Ansible

Ansible: Open-source automation platform for simplified configuration management and deployment tasks.

[**Documentation**](https://docs.ansible.com/)

---
## Running Playbooks

```bash
# Execute playbook on remote hosts
ansible-playbook playbook.yml

# Execute playbook with specific inventory file
ansible-playbook -i inventory_file playbook.yml

# Execute playbook with verbose output
ansible-playbook -v playbook.yml

# Limit playbook execution to specific hosts or groups
ansible-playbook -l host_or_group playbook.yml

# Execute playbook with tags
ansible-playbook --tags "tag1,tag2" playbook.yml
```
---

## Ansible Vault

```bash
# Encrypt a file using a password file
ansible-vault encrypt --vault-password-file=<password_file> <file_path>

# Decrypt an encrypted file
ansible-vault decrypt --vault-password-file=<password_file> <file_path>

# Edit an encrypted file
ansible-vault edit --vault-password-file=<password_file> <file_path>

# View the contents of an encrypted file
ansible-vault view --vault-password-file=<password_file> <file_path>
```
---

## Other Useful Commands

```bash
# Check connectivity to hosts
ansible all -m ping

# Copy files to remote hosts
ansible all -m copy -a "src=file.txt dest=/path/to/destination/"

# Restart services
ansible all -m service -a "name=httpd state=restarted"

# Install packages
ansible all -m yum -a "name=<package_name> state=present" -b

# Execute a shell command
ansible all -m shell -a "echo 'Hello, World!'"

# Check playbook execution without making any changes
ansible-playbook --check playbook.yml

#Execute playbook with become privileges
ansible-playbook playbook.yml -b
```
---