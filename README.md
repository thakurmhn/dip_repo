Usage:

ansible-playbook playbooks/run_one_role.yml -e "target=localhost" -e "role=linux-hardening" --check


Ansible vault

set environment variable

export ANSIBLE_VAULT_PASSWORD_FILE=/etc/.vault_password

ansible-vault edit playbook/group_vars/all/secret.yml


ansible-vault edit playbook/group_vars/all/secret.yml  --vault-password-file=/etc/.vault_password


Run on single node without inventory

ansible-playbook -i server1 playbooks/run_one_role.yml -e "target=server1" -e "role=linux_hardening"
